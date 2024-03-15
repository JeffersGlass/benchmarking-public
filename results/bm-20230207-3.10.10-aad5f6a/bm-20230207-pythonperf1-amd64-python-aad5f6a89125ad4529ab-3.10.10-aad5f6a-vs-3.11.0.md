
# Results vs. 3.11.0

- fork: python
- ref: aad5f6a89125ad4529ab
- machine: windows-amd64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.10x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 231 ms: 1.08x slower                                                      |
| chameleon      | 5.26 ms                                                     | 5.49 ms: 1.04x slower                                                     |
| docutils       | 1.64 sec                                                    | 1.84 sec: 1.12x slower                                                    |
| html5lib       | 38.9 ms                                                     | 48.2 ms: 1.24x slower                                                     |
| tornado_http   | 92.8 ms                                                     | 109 ms: 1.18x slower                                                      |
| Geometric mean | (ref)                                                       | 1.13x slower                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 530 ms                                                      | 615 ms: 1.16x slower                                                      |
| async_tree_memoization  | 399 ms                                                      | 490 ms: 1.23x slower                                                      |
| async_tree_none         | 332 ms                                                      | 417 ms: 1.25x slower                                                      |
| async_tree_io           | 808 ms                                                      | 1.05 sec: 1.29x slower                                                    |
| Geometric mean          | (ref)                                                       | 1.23x slower                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.01x faster                                                      |
| nbody          | 70.3 ms                                                     | 71.9 ms: 1.02x slower                                                     |
| float          | 54.4 ms                                                     | 60.6 ms: 1.11x slower                                                     |
| Geometric mean | (ref)                                                       | 1.04x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 15.0 ms: 1.06x slower                                                     |
| regex_compile  | 91.0 ms                                                     | 103 ms: 1.13x slower                                                      |
| regex_dna      | 116 ms                                                      | 132 ms: 1.14x slower                                                      |
| regex_effbot   | 1.50 ms                                                     | 1.81 ms: 1.21x slower                                                     |
| Geometric mean | (ref)                                                       | 1.13x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| xml_etree_iterparse  | 65.6 ms                                                     | 64.4 ms: 1.02x faster                                                     |
| xml_etree_parse      | 97.6 ms                                                     | 96.6 ms: 1.01x faster                                                     |
| xml_etree_generate   | 52.5 ms                                                     | 53.3 ms: 1.01x slower                                                     |
| pickle_dict          | 18.5 us                                                     | 19.1 us: 1.03x slower                                                     |
| unpickle_list        | 2.59 us                                                     | 2.73 us: 1.05x slower                                                     |
| pickle               | 6.64 us                                                     | 7.00 us: 1.05x slower                                                     |
| pickle_list          | 2.70 us                                                     | 2.91 us: 1.08x slower                                                     |
| json_loads           | 13.0 us                                                     | 14.2 us: 1.09x slower                                                     |
| json_dumps           | 8.09 ms                                                     | 8.93 ms: 1.10x slower                                                     |
| xml_etree_process    | 37.2 ms                                                     | 42.7 ms: 1.15x slower                                                     |
| unpickle_pure_python | 157 us                                                      | 180 us: 1.15x slower                                                      |
| unpickle             | 7.57 us                                                     | 9.05 us: 1.19x slower                                                     |
| pickle_pure_python   | 208 us                                                      | 267 us: 1.28x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.09x slower                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.0 ms: 1.12x faster                                                     |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                              |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| genshi_xml      | 39.9 ms                                                     | 39.0 ms: 1.02x faster                                                     |
| genshi_text     | 18.4 ms                                                     | 18.3 ms: 1.01x faster                                                     |
| mako            | 7.58 ms                                                     | 8.84 ms: 1.17x slower                                                     |
| django_template | 24.4 ms                                                     | 29.2 ms: 1.20x slower                                                     |
| Geometric mean  | (ref)                                                       | 1.08x slower                                                              |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 40.8 ns: 1.15x faster                                                     |
| python_startup_no_site  | 16.8 ms                                                     | 15.0 ms: 1.12x faster                                                     |
| coverage                | 43.4 ms                                                     | 40.0 ms: 1.09x faster                                                     |
| asyncio_tcp             | 726 ms                                                      | 678 ms: 1.07x faster                                                      |
| gc_traversal            | 1.49 ms                                                     | 1.40 ms: 1.07x faster                                                     |
| logging_simple          | 6.86 us                                                     | 6.45 us: 1.06x faster                                                     |
| bench_mp_pool           | 63.2 ms                                                     | 60.0 ms: 1.05x faster                                                     |
| logging_format          | 7.16 us                                                     | 6.81 us: 1.05x faster                                                     |
| telco                   | 4.06 ms                                                     | 3.88 ms: 1.05x faster                                                     |
| nqueens                 | 68.3 ms                                                     | 65.3 ms: 1.05x faster                                                     |
| generators              | 34.0 ms                                                     | 32.5 ms: 1.04x faster                                                     |
| meteor_contest          | 75.2 ms                                                     | 72.9 ms: 1.03x faster                                                     |
| genshi_xml              | 39.9 ms                                                     | 39.0 ms: 1.02x faster                                                     |
| xml_etree_iterparse     | 65.6 ms                                                     | 64.4 ms: 1.02x faster                                                     |
| pidigits                | 150 ms                                                      | 148 ms: 1.01x faster                                                      |
| xml_etree_parse         | 97.6 ms                                                     | 96.6 ms: 1.01x faster                                                     |
| genshi_text             | 18.4 ms                                                     | 18.3 ms: 1.01x faster                                                     |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                    |
| xml_etree_generate      | 52.5 ms                                                     | 53.3 ms: 1.01x slower                                                     |
| nbody                   | 70.3 ms                                                     | 71.9 ms: 1.02x slower                                                     |
| fannkuch                | 253 ms                                                      | 259 ms: 1.02x slower                                                      |
| sympy_str               | 185 ms                                                      | 191 ms: 1.03x slower                                                      |
| pickle_dict             | 18.5 us                                                     | 19.1 us: 1.03x slower                                                     |
| deepcopy_reduce         | 2.06 us                                                     | 2.14 us: 1.04x slower                                                     |
| chameleon               | 5.26 ms                                                     | 5.49 ms: 1.04x slower                                                     |
| sympy_integrate         | 14.0 ms                                                     | 14.6 ms: 1.04x slower                                                     |
| deepcopy                | 246 us                                                      | 258 us: 1.05x slower                                                      |
| sympy_expand            | 299 ms                                                      | 314 ms: 1.05x slower                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.86 us: 1.05x slower                                                     |
| pylint                  | 323 ms                                                      | 340 ms: 1.05x slower                                                      |
| unpickle_list           | 2.59 us                                                     | 2.73 us: 1.05x slower                                                     |
| pickle                  | 6.64 us                                                     | 7.00 us: 1.05x slower                                                     |
| dulwich_log             | 46.4 ms                                                     | 49.0 ms: 1.06x slower                                                     |
| regex_v8                | 14.2 ms                                                     | 15.0 ms: 1.06x slower                                                     |
| pathlib                 | 70.9 ms                                                     | 75.0 ms: 1.06x slower                                                     |
| coroutines              | 15.0 ms                                                     | 15.9 ms: 1.06x slower                                                     |
| sympy_sum               | 100 ms                                                      | 106 ms: 1.06x slower                                                      |
| sqlglot_normalize       | 190 ms                                                      | 202 ms: 1.06x slower                                                      |
| mdp                     | 1.59 sec                                                    | 1.71 sec: 1.07x slower                                                    |
| pickle_list             | 2.70 us                                                     | 2.91 us: 1.08x slower                                                     |
| scimark_fft             | 179 ms                                                      | 194 ms: 1.08x slower                                                      |
| bench_thread_pool       | 872 us                                                      | 944 us: 1.08x slower                                                      |
| 2to3                    | 214 ms                                                      | 231 ms: 1.08x slower                                                      |
| pprint_pformat          | 1.09 sec                                                    | 1.18 sec: 1.09x slower                                                    |
| pprint_safe_repr        | 529 ms                                                      | 576 ms: 1.09x slower                                                      |
| create_gc_cycles        | 713 us                                                      | 776 us: 1.09x slower                                                      |
| json_loads              | 13.0 us                                                     | 14.2 us: 1.09x slower                                                     |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.82 ms: 1.09x slower                                                     |
| sqlalchemy_imperative   | 10.4 ms                                                     | 11.5 ms: 1.10x slower                                                     |
| json_dumps              | 8.09 ms                                                     | 8.93 ms: 1.10x slower                                                     |
| aiohttp                 | 883 us                                                      | 980 us: 1.11x slower                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 38.5 ms: 1.11x slower                                                     |
| float                   | 54.4 ms                                                     | 60.6 ms: 1.11x slower                                                     |
| deepcopy_memo           | 26.0 us                                                     | 29.1 us: 1.12x slower                                                     |
| docutils                | 1.64 sec                                                    | 1.84 sec: 1.12x slower                                                    |
| sqlalchemy_declarative  | 85.6 ms                                                     | 97.2 ms: 1.13x slower                                                     |
| regex_compile           | 91.0 ms                                                     | 103 ms: 1.13x slower                                                      |
| regex_dna               | 116 ms                                                      | 132 ms: 1.14x slower                                                      |
| xml_etree_process       | 37.2 ms                                                     | 42.7 ms: 1.15x slower                                                     |
| unpickle_pure_python    | 157 us                                                      | 180 us: 1.15x slower                                                      |
| dask                    | 273 ms                                                      | 314 ms: 1.15x slower                                                      |
| async_tree_cpu_io_mixed | 530 ms                                                      | 615 ms: 1.16x slower                                                      |
| mako                    | 7.58 ms                                                     | 8.84 ms: 1.17x slower                                                     |
| tornado_http            | 92.8 ms                                                     | 109 ms: 1.18x slower                                                      |
| hexiom                  | 4.55 ms                                                     | 5.38 ms: 1.18x slower                                                     |
| pycparser               | 720 ms                                                      | 855 ms: 1.19x slower                                                      |
| unpickle                | 7.57 us                                                     | 9.05 us: 1.19x slower                                                     |
| django_template         | 24.4 ms                                                     | 29.2 ms: 1.20x slower                                                     |
| chaos                   | 48.4 ms                                                     | 58.2 ms: 1.20x slower                                                     |
| spectral_norm           | 68.3 ms                                                     | 82.5 ms: 1.21x slower                                                     |
| regex_effbot            | 1.50 ms                                                     | 1.81 ms: 1.21x slower                                                     |
| scimark_monte_carlo     | 45.3 ms                                                     | 55.2 ms: 1.22x slower                                                     |
| thrift                  | 494 us                                                      | 605 us: 1.23x slower                                                      |
| async_tree_memoization  | 399 ms                                                      | 490 ms: 1.23x slower                                                      |
| html5lib                | 38.9 ms                                                     | 48.2 ms: 1.24x slower                                                     |
| raytrace                | 213 ms                                                      | 266 ms: 1.25x slower                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.45 ms: 1.25x slower                                                     |
| async_tree_none         | 332 ms                                                      | 417 ms: 1.25x slower                                                      |
| pyflate                 | 312 ms                                                      | 393 ms: 1.26x slower                                                      |
| async_generators        | 177 ms                                                      | 227 ms: 1.28x slower                                                      |
| pickle_pure_python      | 208 us                                                      | 267 us: 1.28x slower                                                      |
| sqlglot_parse           | 953 us                                                      | 1.23 ms: 1.29x slower                                                     |
| crypto_pyaes            | 48.9 ms                                                     | 63.1 ms: 1.29x slower                                                     |
| async_tree_io           | 808 ms                                                      | 1.05 sec: 1.29x slower                                                    |
| scimark_lu              | 62.8 ms                                                     | 83.2 ms: 1.32x slower                                                     |
| scimark_sor             | 78.1 ms                                                     | 104 ms: 1.33x slower                                                      |
| richards                | 31.4 ms                                                     | 42.3 ms: 1.35x slower                                                     |
| go                      | 101 ms                                                      | 138 ms: 1.37x slower                                                      |
| logging_silent          | 71.8 ns                                                     | 99.1 ns: 1.38x slower                                                     |
| deltablue               | 2.70 ms                                                     | 4.16 ms: 1.54x slower                                                     |
| Geometric mean          | (ref)                                                       | 1.10x slower                                                              |

Benchmark hidden because not significant (3): comprehensions, python_startup, json
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.08x
- 95% likely to have a slowdown of 1.07x
- 99% likely to have a slowdown of 1.06x


# Memory

- memory change: unknown