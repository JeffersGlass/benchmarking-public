
# Results vs. 3.11.0

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: windows-amd64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.10x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 233 ms: 1.09x slower                                                      |
| chameleon      | 5.26 ms                                                     | 5.67 ms: 1.08x slower                                                     |
| docutils       | 1.64 sec                                                    | 1.82 sec: 1.11x slower                                                    |
| html5lib       | 38.9 ms                                                     | 45.8 ms: 1.18x slower                                                     |
| tornado_http   | 92.8 ms                                                     | 108 ms: 1.16x slower                                                      |
| Geometric mean | (ref)                                                       | 1.12x slower                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 530 ms                                                      | 598 ms: 1.13x slower                                                      |
| async_tree_memoization  | 399 ms                                                      | 481 ms: 1.21x slower                                                      |
| async_tree_none         | 332 ms                                                      | 414 ms: 1.25x slower                                                      |
| async_tree_io           | 808 ms                                                      | 1.04 sec: 1.28x slower                                                    |
| Geometric mean          | (ref)                                                       | 1.21x slower                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                      |
| nbody          | 70.3 ms                                                     | 75.5 ms: 1.07x slower                                                     |
| float          | 54.4 ms                                                     | 60.7 ms: 1.12x slower                                                     |
| Geometric mean | (ref)                                                       | 1.05x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                     |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                     |
| regex_dna      | 116 ms                                                      | 129 ms: 1.11x slower                                                      |
| regex_compile  | 91.0 ms                                                     | 102 ms: 1.12x slower                                                      |
| Geometric mean | (ref)                                                       | 1.08x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| xml_etree_iterparse  | 65.6 ms                                                     | 63.4 ms: 1.03x faster                                                     |
| xml_etree_parse      | 97.6 ms                                                     | 96.4 ms: 1.01x faster                                                     |
| pickle_dict          | 18.5 us                                                     | 18.7 us: 1.01x slower                                                     |
| unpickle_list        | 2.59 us                                                     | 2.66 us: 1.03x slower                                                     |
| xml_etree_generate   | 52.5 ms                                                     | 54.3 ms: 1.03x slower                                                     |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                                     |
| pickle_list          | 2.70 us                                                     | 2.86 us: 1.06x slower                                                     |
| json_dumps           | 8.09 ms                                                     | 8.90 ms: 1.10x slower                                                     |
| pickle               | 6.64 us                                                     | 7.34 us: 1.11x slower                                                     |
| unpickle_pure_python | 157 us                                                      | 177 us: 1.13x slower                                                      |
| xml_etree_process    | 37.2 ms                                                     | 43.5 ms: 1.17x slower                                                     |
| unpickle             | 7.57 us                                                     | 9.30 us: 1.23x slower                                                     |
| pickle_pure_python   | 208 us                                                      | 266 us: 1.28x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.09x slower                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.6 ms: 1.08x faster                                                     |
| python_startup         | 19.8 ms                                                     | 21.1 ms: 1.06x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.01x faster                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| genshi_xml      | 39.9 ms                                                     | 39.1 ms: 1.02x faster                                                     |
| genshi_text     | 18.4 ms                                                     | 18.8 ms: 1.02x slower                                                     |
| mako            | 7.58 ms                                                     | 8.76 ms: 1.15x slower                                                     |
| django_template | 24.4 ms                                                     | 28.9 ms: 1.18x slower                                                     |
| Geometric mean  | (ref)                                                       | 1.08x slower                                                              |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 42.1 ns: 1.11x faster                                                     |
| coverage                | 43.4 ms                                                     | 39.2 ms: 1.11x faster                                                     |
| logging_simple          | 6.86 us                                                     | 6.28 us: 1.09x faster                                                     |
| python_startup_no_site  | 16.8 ms                                                     | 15.6 ms: 1.08x faster                                                     |
| logging_format          | 7.16 us                                                     | 6.76 us: 1.06x faster                                                     |
| generators              | 34.0 ms                                                     | 32.1 ms: 1.06x faster                                                     |
| gc_traversal            | 1.49 ms                                                     | 1.42 ms: 1.05x faster                                                     |
| bench_mp_pool           | 63.2 ms                                                     | 60.4 ms: 1.05x faster                                                     |
| meteor_contest          | 75.2 ms                                                     | 72.1 ms: 1.04x faster                                                     |
| telco                   | 4.06 ms                                                     | 3.93 ms: 1.03x faster                                                     |
| xml_etree_iterparse     | 65.6 ms                                                     | 63.4 ms: 1.03x faster                                                     |
| pidigits                | 150 ms                                                      | 147 ms: 1.02x faster                                                      |
| genshi_xml              | 39.9 ms                                                     | 39.1 ms: 1.02x faster                                                     |
| xml_etree_parse         | 97.6 ms                                                     | 96.4 ms: 1.01x faster                                                     |
| nqueens                 | 68.3 ms                                                     | 67.5 ms: 1.01x faster                                                     |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                    |
| pickle_dict             | 18.5 us                                                     | 18.7 us: 1.01x slower                                                     |
| sympy_str               | 185 ms                                                      | 188 ms: 1.02x slower                                                      |
| genshi_text             | 18.4 ms                                                     | 18.8 ms: 1.02x slower                                                     |
| dulwich_log             | 46.4 ms                                                     | 47.6 ms: 1.03x slower                                                     |
| unpickle_list           | 2.59 us                                                     | 2.66 us: 1.03x slower                                                     |
| regex_v8                | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                     |
| xml_etree_generate      | 52.5 ms                                                     | 54.3 ms: 1.03x slower                                                     |
| deepcopy_reduce         | 2.06 us                                                     | 2.13 us: 1.04x slower                                                     |
| asyncio_tcp             | 726 ms                                                      | 755 ms: 1.04x slower                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.84 us: 1.04x slower                                                     |
| sympy_sum               | 100 ms                                                      | 105 ms: 1.04x slower                                                      |
| sympy_expand            | 299 ms                                                      | 312 ms: 1.05x slower                                                      |
| coroutines              | 15.0 ms                                                     | 15.7 ms: 1.05x slower                                                     |
| pathlib                 | 70.9 ms                                                     | 74.4 ms: 1.05x slower                                                     |
| sympy_integrate         | 14.0 ms                                                     | 14.8 ms: 1.05x slower                                                     |
| pylint                  | 323 ms                                                      | 341 ms: 1.05x slower                                                      |
| json_loads              | 13.0 us                                                     | 13.7 us: 1.06x slower                                                     |
| deepcopy                | 246 us                                                      | 260 us: 1.06x slower                                                      |
| sqlglot_normalize       | 190 ms                                                      | 202 ms: 1.06x slower                                                      |
| pickle_list             | 2.70 us                                                     | 2.86 us: 1.06x slower                                                     |
| bench_thread_pool       | 872 us                                                      | 928 us: 1.06x slower                                                      |
| python_startup          | 19.8 ms                                                     | 21.1 ms: 1.06x slower                                                     |
| sqlalchemy_imperative   | 10.4 ms                                                     | 11.1 ms: 1.07x slower                                                     |
| regex_effbot            | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                     |
| nbody                   | 70.3 ms                                                     | 75.5 ms: 1.07x slower                                                     |
| mdp                     | 1.59 sec                                                    | 1.71 sec: 1.07x slower                                                    |
| chameleon               | 5.26 ms                                                     | 5.67 ms: 1.08x slower                                                     |
| aiohttp                 | 883 us                                                      | 962 us: 1.09x slower                                                      |
| create_gc_cycles        | 713 us                                                      | 777 us: 1.09x slower                                                      |
| 2to3                    | 214 ms                                                      | 233 ms: 1.09x slower                                                      |
| fannkuch                | 253 ms                                                      | 276 ms: 1.09x slower                                                      |
| pprint_pformat          | 1.09 sec                                                    | 1.19 sec: 1.10x slower                                                    |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.83 ms: 1.10x slower                                                     |
| json_dumps              | 8.09 ms                                                     | 8.90 ms: 1.10x slower                                                     |
| deepcopy_memo           | 26.0 us                                                     | 28.6 us: 1.10x slower                                                     |
| pprint_safe_repr        | 529 ms                                                      | 584 ms: 1.10x slower                                                      |
| pickle                  | 6.64 us                                                     | 7.34 us: 1.11x slower                                                     |
| dask                    | 273 ms                                                      | 303 ms: 1.11x slower                                                      |
| regex_dna               | 116 ms                                                      | 129 ms: 1.11x slower                                                      |
| docutils                | 1.64 sec                                                    | 1.82 sec: 1.11x slower                                                    |
| sqlglot_optimize        | 34.5 ms                                                     | 38.5 ms: 1.12x slower                                                     |
| float                   | 54.4 ms                                                     | 60.7 ms: 1.12x slower                                                     |
| sqlalchemy_declarative  | 85.6 ms                                                     | 95.8 ms: 1.12x slower                                                     |
| regex_compile           | 91.0 ms                                                     | 102 ms: 1.12x slower                                                      |
| async_tree_cpu_io_mixed | 530 ms                                                      | 598 ms: 1.13x slower                                                      |
| unpickle_pure_python    | 157 us                                                      | 177 us: 1.13x slower                                                      |
| scimark_fft             | 179 ms                                                      | 203 ms: 1.13x slower                                                      |
| mako                    | 7.58 ms                                                     | 8.76 ms: 1.15x slower                                                     |
| tornado_http            | 92.8 ms                                                     | 108 ms: 1.16x slower                                                      |
| pycparser               | 720 ms                                                      | 839 ms: 1.17x slower                                                      |
| xml_etree_process       | 37.2 ms                                                     | 43.5 ms: 1.17x slower                                                     |
| html5lib                | 38.9 ms                                                     | 45.8 ms: 1.18x slower                                                     |
| django_template         | 24.4 ms                                                     | 28.9 ms: 1.18x slower                                                     |
| hexiom                  | 4.55 ms                                                     | 5.40 ms: 1.19x slower                                                     |
| spectral_norm           | 68.3 ms                                                     | 81.4 ms: 1.19x slower                                                     |
| async_tree_memoization  | 399 ms                                                      | 481 ms: 1.21x slower                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.42 ms: 1.22x slower                                                     |
| chaos                   | 48.4 ms                                                     | 59.2 ms: 1.22x slower                                                     |
| unpickle                | 7.57 us                                                     | 9.30 us: 1.23x slower                                                     |
| async_generators        | 177 ms                                                      | 218 ms: 1.23x slower                                                      |
| sqlglot_parse           | 953 us                                                      | 1.19 ms: 1.24x slower                                                     |
| async_tree_none         | 332 ms                                                      | 414 ms: 1.25x slower                                                      |
| pyflate                 | 312 ms                                                      | 391 ms: 1.25x slower                                                      |
| raytrace                | 213 ms                                                      | 271 ms: 1.27x slower                                                      |
| thrift                  | 494 us                                                      | 629 us: 1.27x slower                                                      |
| pickle_pure_python      | 208 us                                                      | 266 us: 1.28x slower                                                      |
| async_tree_io           | 808 ms                                                      | 1.04 sec: 1.28x slower                                                    |
| crypto_pyaes            | 48.9 ms                                                     | 63.2 ms: 1.29x slower                                                     |
| scimark_monte_carlo     | 45.3 ms                                                     | 58.9 ms: 1.30x slower                                                     |
| richards                | 31.4 ms                                                     | 40.9 ms: 1.30x slower                                                     |
| scimark_lu              | 62.8 ms                                                     | 84.5 ms: 1.34x slower                                                     |
| go                      | 101 ms                                                      | 137 ms: 1.35x slower                                                      |
| logging_silent          | 71.8 ns                                                     | 97.2 ns: 1.35x slower                                                     |
| scimark_sor             | 78.1 ms                                                     | 107 ms: 1.37x slower                                                      |
| deltablue               | 2.70 ms                                                     | 4.11 ms: 1.52x slower                                                     |
| Geometric mean          | (ref)                                                       | 1.10x slower                                                              |

Benchmark hidden because not significant (2): comprehensions, json
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.08x
- 95% likely to have a slowdown of 1.08x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: unknown