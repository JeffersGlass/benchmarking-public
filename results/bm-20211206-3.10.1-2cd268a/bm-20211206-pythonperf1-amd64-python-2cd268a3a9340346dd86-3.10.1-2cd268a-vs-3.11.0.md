
# Results vs. 3.11.0

- fork: python
- ref: 2cd268a3a9340346dd86
- machine: windows-amd64
- commit hash: 2cd268a
- commit date: 2021-12-06
- overall geometric mean: 1.10x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 232 ms: 1.09x slower                                                     |
| chameleon      | 5.26 ms                                                     | 5.89 ms: 1.12x slower                                                    |
| docutils       | 1.64 sec                                                    | 1.88 sec: 1.14x slower                                                   |
| html5lib       | 38.9 ms                                                     | 48.7 ms: 1.25x slower                                                    |
| tornado_http   | 92.8 ms                                                     | 109 ms: 1.18x slower                                                     |
| Geometric mean | (ref)                                                       | 1.15x slower                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 530 ms                                                      | 615 ms: 1.16x slower                                                     |
| async_tree_memoization  | 399 ms                                                      | 484 ms: 1.21x slower                                                     |
| async_tree_none         | 332 ms                                                      | 417 ms: 1.26x slower                                                     |
| async_tree_io           | 808 ms                                                      | 1.03 sec: 1.27x slower                                                   |
| Geometric mean          | (ref)                                                       | 1.22x slower                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 149 ms: 1.01x faster                                                     |
| nbody          | 70.3 ms                                                     | 77.2 ms: 1.10x slower                                                    |
| float          | 54.4 ms                                                     | 61.8 ms: 1.14x slower                                                    |
| Geometric mean | (ref)                                                       | 1.07x slower                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 15.0 ms: 1.06x slower                                                    |
| regex_dna      | 116 ms                                                      | 129 ms: 1.11x slower                                                     |
| regex_compile  | 91.0 ms                                                     | 103 ms: 1.13x slower                                                     |
| regex_effbot   | 1.50 ms                                                     | 1.74 ms: 1.16x slower                                                    |
| Geometric mean | (ref)                                                       | 1.11x slower                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| pickle_dict          | 18.5 us                                                     | 17.0 us: 1.09x faster                                                    |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.6 ms: 1.02x faster                                                    |
| unpickle_list        | 2.59 us                                                     | 2.64 us: 1.02x slower                                                    |
| pickle               | 6.64 us                                                     | 6.84 us: 1.03x slower                                                    |
| json_dumps           | 8.09 ms                                                     | 8.45 ms: 1.04x slower                                                    |
| xml_etree_generate   | 52.5 ms                                                     | 55.0 ms: 1.05x slower                                                    |
| unpickle             | 7.57 us                                                     | 8.17 us: 1.08x slower                                                    |
| unpickle_pure_python | 157 us                                                      | 177 us: 1.13x slower                                                     |
| json_loads           | 13.0 us                                                     | 15.0 us: 1.15x slower                                                    |
| xml_etree_process    | 37.2 ms                                                     | 44.0 ms: 1.18x slower                                                    |
| pickle_pure_python   | 208 us                                                      | 267 us: 1.28x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.06x slower                                                             |

Benchmark hidden because not significant (2): pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.1 ms: 1.11x faster                                                    |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                             |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| genshi_xml      | 39.9 ms                                                     | 40.9 ms: 1.02x slower                                                    |
| genshi_text     | 18.4 ms                                                     | 19.6 ms: 1.06x slower                                                    |
| mako            | 7.58 ms                                                     | 8.56 ms: 1.13x slower                                                    |
| django_template | 24.4 ms                                                     | 29.2 ms: 1.19x slower                                                    |
| Geometric mean  | (ref)                                                       | 1.10x slower                                                             |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 40.5 ns: 1.16x faster                                                    |
| coverage                | 43.4 ms                                                     | 38.8 ms: 1.12x faster                                                    |
| python_startup_no_site  | 16.8 ms                                                     | 15.1 ms: 1.11x faster                                                    |
| generators              | 34.0 ms                                                     | 30.7 ms: 1.11x faster                                                    |
| logging_simple          | 6.86 us                                                     | 6.24 us: 1.10x faster                                                    |
| pickle_dict             | 18.5 us                                                     | 17.0 us: 1.09x faster                                                    |
| gc_traversal            | 1.49 ms                                                     | 1.37 ms: 1.09x faster                                                    |
| logging_format          | 7.16 us                                                     | 6.72 us: 1.07x faster                                                    |
| telco                   | 4.06 ms                                                     | 3.86 ms: 1.05x faster                                                    |
| bench_mp_pool           | 63.2 ms                                                     | 60.4 ms: 1.05x faster                                                    |
| nqueens                 | 68.3 ms                                                     | 65.5 ms: 1.04x faster                                                    |
| meteor_contest          | 75.2 ms                                                     | 73.2 ms: 1.03x faster                                                    |
| xml_etree_iterparse     | 65.6 ms                                                     | 64.6 ms: 1.02x faster                                                    |
| pidigits                | 150 ms                                                      | 149 ms: 1.01x faster                                                     |
| flaskblogging           | 2.03 sec                                                    | 2.04 sec: 1.01x slower                                                   |
| comprehensions          | 15.6 us                                                     | 15.8 us: 1.01x slower                                                    |
| unpickle_list           | 2.59 us                                                     | 2.64 us: 1.02x slower                                                    |
| genshi_xml              | 39.9 ms                                                     | 40.9 ms: 1.02x slower                                                    |
| pickle                  | 6.64 us                                                     | 6.84 us: 1.03x slower                                                    |
| deepcopy                | 246 us                                                      | 254 us: 1.03x slower                                                     |
| sympy_str               | 185 ms                                                      | 191 ms: 1.03x slower                                                     |
| sympy_sum               | 100 ms                                                      | 104 ms: 1.04x slower                                                     |
| deepcopy_reduce         | 2.06 us                                                     | 2.15 us: 1.04x slower                                                    |
| json_dumps              | 8.09 ms                                                     | 8.45 ms: 1.04x slower                                                    |
| xml_etree_generate      | 52.5 ms                                                     | 55.0 ms: 1.05x slower                                                    |
| sqlite_synth            | 1.77 us                                                     | 1.85 us: 1.05x slower                                                    |
| fannkuch                | 253 ms                                                      | 266 ms: 1.05x slower                                                     |
| dulwich_log             | 46.4 ms                                                     | 48.7 ms: 1.05x slower                                                    |
| json                    | 2.98 ms                                                     | 3.13 ms: 1.05x slower                                                    |
| sympy_expand            | 299 ms                                                      | 316 ms: 1.06x slower                                                     |
| regex_v8                | 14.2 ms                                                     | 15.0 ms: 1.06x slower                                                    |
| sympy_integrate         | 14.0 ms                                                     | 14.9 ms: 1.06x slower                                                    |
| genshi_text             | 18.4 ms                                                     | 19.6 ms: 1.06x slower                                                    |
| pylint                  | 323 ms                                                      | 343 ms: 1.06x slower                                                     |
| coroutines              | 15.0 ms                                                     | 15.9 ms: 1.06x slower                                                    |
| sqlglot_normalize       | 190 ms                                                      | 203 ms: 1.07x slower                                                     |
| pathlib                 | 70.9 ms                                                     | 75.9 ms: 1.07x slower                                                    |
| create_gc_cycles        | 713 us                                                      | 770 us: 1.08x slower                                                     |
| mdp                     | 1.59 sec                                                    | 1.72 sec: 1.08x slower                                                   |
| unpickle                | 7.57 us                                                     | 8.17 us: 1.08x slower                                                    |
| scimark_fft             | 179 ms                                                      | 195 ms: 1.09x slower                                                     |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.80 ms: 1.09x slower                                                    |
| 2to3                    | 214 ms                                                      | 232 ms: 1.09x slower                                                     |
| sqlalchemy_imperative   | 10.4 ms                                                     | 11.4 ms: 1.09x slower                                                    |
| nbody                   | 70.3 ms                                                     | 77.2 ms: 1.10x slower                                                    |
| deepcopy_memo           | 26.0 us                                                     | 28.7 us: 1.11x slower                                                    |
| bench_thread_pool       | 872 us                                                      | 965 us: 1.11x slower                                                     |
| regex_dna               | 116 ms                                                      | 129 ms: 1.11x slower                                                     |
| chameleon               | 5.26 ms                                                     | 5.89 ms: 1.12x slower                                                    |
| aiohttp                 | 883 us                                                      | 990 us: 1.12x slower                                                     |
| mako                    | 7.58 ms                                                     | 8.56 ms: 1.13x slower                                                    |
| unpickle_pure_python    | 157 us                                                      | 177 us: 1.13x slower                                                     |
| regex_compile           | 91.0 ms                                                     | 103 ms: 1.13x slower                                                     |
| sqlglot_optimize        | 34.5 ms                                                     | 39.2 ms: 1.13x slower                                                    |
| pprint_safe_repr        | 529 ms                                                      | 601 ms: 1.14x slower                                                     |
| float                   | 54.4 ms                                                     | 61.8 ms: 1.14x slower                                                    |
| docutils                | 1.64 sec                                                    | 1.88 sec: 1.14x slower                                                   |
| pprint_pformat          | 1.09 sec                                                    | 1.24 sec: 1.14x slower                                                   |
| sqlalchemy_declarative  | 85.6 ms                                                     | 98.4 ms: 1.15x slower                                                    |
| json_loads              | 13.0 us                                                     | 15.0 us: 1.15x slower                                                    |
| regex_effbot            | 1.50 ms                                                     | 1.74 ms: 1.16x slower                                                    |
| async_tree_cpu_io_mixed | 530 ms                                                      | 615 ms: 1.16x slower                                                     |
| spectral_norm           | 68.3 ms                                                     | 79.4 ms: 1.16x slower                                                    |
| dask                    | 273 ms                                                      | 319 ms: 1.17x slower                                                     |
| tornado_http            | 92.8 ms                                                     | 109 ms: 1.18x slower                                                     |
| xml_etree_process       | 37.2 ms                                                     | 44.0 ms: 1.18x slower                                                    |
| hexiom                  | 4.55 ms                                                     | 5.42 ms: 1.19x slower                                                    |
| django_template         | 24.4 ms                                                     | 29.2 ms: 1.19x slower                                                    |
| pycparser               | 720 ms                                                      | 861 ms: 1.20x slower                                                     |
| async_tree_memoization  | 399 ms                                                      | 484 ms: 1.21x slower                                                     |
| chaos                   | 48.4 ms                                                     | 59.4 ms: 1.23x slower                                                    |
| sqlglot_transpile       | 1.16 ms                                                     | 1.45 ms: 1.24x slower                                                    |
| html5lib                | 38.9 ms                                                     | 48.7 ms: 1.25x slower                                                    |
| scimark_monte_carlo     | 45.3 ms                                                     | 56.9 ms: 1.25x slower                                                    |
| async_tree_none         | 332 ms                                                      | 417 ms: 1.26x slower                                                     |
| async_generators        | 177 ms                                                      | 224 ms: 1.26x slower                                                     |
| pyflate                 | 312 ms                                                      | 394 ms: 1.26x slower                                                     |
| thrift                  | 494 us                                                      | 625 us: 1.27x slower                                                     |
| sqlglot_parse           | 953 us                                                      | 1.21 ms: 1.27x slower                                                    |
| async_tree_io           | 808 ms                                                      | 1.03 sec: 1.27x slower                                                   |
| raytrace                | 213 ms                                                      | 273 ms: 1.28x slower                                                     |
| pickle_pure_python      | 208 us                                                      | 267 us: 1.28x slower                                                     |
| richards                | 31.4 ms                                                     | 40.9 ms: 1.30x slower                                                    |
| scimark_lu              | 62.8 ms                                                     | 83.4 ms: 1.33x slower                                                    |
| crypto_pyaes            | 48.9 ms                                                     | 65.5 ms: 1.34x slower                                                    |
| scimark_sor             | 78.1 ms                                                     | 106 ms: 1.36x slower                                                     |
| go                      | 101 ms                                                      | 137 ms: 1.36x slower                                                     |
| logging_silent          | 71.8 ns                                                     | 98.0 ns: 1.37x slower                                                    |
| deltablue               | 2.70 ms                                                     | 4.13 ms: 1.53x slower                                                    |
| Geometric mean          | (ref)                                                       | 1.10x slower                                                             |

Benchmark hidden because not significant (4): asyncio_tcp, python_startup, pickle_list, xml_etree_parse
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.08x
- 95% likely to have a slowdown of 1.08x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: unknown