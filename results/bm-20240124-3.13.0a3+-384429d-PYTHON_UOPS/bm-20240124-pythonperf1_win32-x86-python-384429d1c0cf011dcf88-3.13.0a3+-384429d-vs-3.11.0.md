
# Results vs. 3.11.0

- fork: python
- ref: 384429d1c0cf011dcf88
- machine: windows-x86
- commit hash: 384429d
- commit date: 2024-01-24
- overall geometric mean: 1.23x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 246 ms: 1.15x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.79 ms: 1.40x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.84 sec: 1.14x faster                                                          |
| tornado_http   | 118 ms                                                          | 99.1 ms: 1.19x faster                                                           |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 261 ms: 1.31x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 328 ms: 1.25x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 603 ms: 1.24x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 310 ms: 1.22x faster                                                            |
| async_tree_io              | 754 ms                                                          | 628 ms: 1.20x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 511 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 504 ms: 1.15x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 88.5 ms: 1.42x faster                                                           |
| float          | 76.1 ms                                                         | 59.3 ms: 1.28x faster                                                           |
| pidigits       | 203 ms                                                          | 200 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 107 ms: 1.38x faster                                                            |
| regex_dna      | 122 ms                                                          | 119 ms: 1.02x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 150 us: 1.54x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.51 ms: 1.51x faster                                                           |
| pickle_pure_python   | 309 us                                                          | 208 us: 1.48x faster                                                            |
| tomli_loads          | 2.31 sec                                                        | 1.68 sec: 1.38x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 42.2 ms: 1.30x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 61.7 ms: 1.16x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 3.07 us: 1.07x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 71.1 ms: 1.06x faster                                                           |
| pickle               | 7.99 us                                                         | 7.74 us: 1.03x faster                                                           |
| json_loads           | 20.0 us                                                         | 19.7 us: 1.02x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.8 us: 1.01x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 113 ms: 1.01x faster                                                            |
| unpickle             | 9.23 us                                                         | 9.57 us: 1.04x slower                                                           |
| pickle_list          | 3.27 us                                                         | 3.74 us: 1.15x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.2 ms: 1.06x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.7 ms: 1.10x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 8.03 ms: 1.28x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 93.5 us: 5.12x faster                                                           |
| generators                 | 52.2 ms                                                         | 23.6 ms: 2.21x faster                                                           |
| logging_silent             | 119 ns                                                          | 61.8 ns: 1.93x faster                                                           |
| richards_super             | 58.7 ms                                                         | 33.0 ms: 1.78x faster                                                           |
| richards                   | 48.8 ms                                                         | 28.9 ms: 1.69x faster                                                           |
| scimark_sor                | 135 ms                                                          | 81.0 ms: 1.67x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 24.0 us: 1.67x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 62.3 ms: 1.64x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 910 us: 1.64x faster                                                            |
| coroutines                 | 23.7 ms                                                         | 14.5 ms: 1.63x faster                                                           |
| chaos                      | 84.4 ms                                                         | 53.0 ms: 1.59x faster                                                           |
| comprehensions             | 22.1 us                                                         | 14.0 us: 1.58x faster                                                           |
| raytrace                   | 327 ms                                                          | 210 ms: 1.56x faster                                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.15 ms: 1.55x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 150 us: 1.54x faster                                                            |
| unpack_sequence            | 65.2 ns                                                         | 42.6 ns: 1.53x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.51 ms: 1.51x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 208 us: 1.48x faster                                                            |
| deltablue                  | 4.10 ms                                                         | 2.80 ms: 1.46x faster                                                           |
| spectral_norm              | 122 ms                                                          | 84.6 ms: 1.44x faster                                                           |
| nbody                      | 126 ms                                                          | 88.5 ms: 1.42x faster                                                           |
| deepcopy                   | 381 us                                                          | 268 us: 1.42x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.34 us: 1.42x faster                                                           |
| nqueens                    | 111 ms                                                          | 79.8 ms: 1.40x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 5.79 ms: 1.40x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 5.41 ms: 1.39x faster                                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.22 sec: 1.39x faster                                                          |
| go                         | 147 ms                                                          | 106 ms: 1.39x faster                                                            |
| regex_compile              | 148 ms                                                          | 107 ms: 1.38x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.68 sec: 1.38x faster                                                          |
| pyflate                    | 471 ms                                                          | 342 ms: 1.38x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 108 ms: 1.38x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 57.7 ms: 1.38x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 598 ms: 1.37x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 52.7 ms: 1.34x faster                                                           |
| sympy_str                  | 283 ms                                                          | 211 ms: 1.34x faster                                                            |
| logging_simple             | 10.8 us                                                         | 8.08 us: 1.34x faster                                                           |
| async_tree_none            | 343 ms                                                          | 261 ms: 1.31x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.77 us: 1.31x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 42.2 ms: 1.30x faster                                                           |
| scimark_fft                | 291 ms                                                          | 225 ms: 1.30x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 15.4 ms: 1.29x faster                                                           |
| float                      | 76.1 ms                                                         | 59.3 ms: 1.28x faster                                                           |
| mako                       | 10.3 ms                                                         | 8.03 ms: 1.28x faster                                                           |
| fannkuch                   | 399 ms                                                          | 314 ms: 1.27x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.35 ms: 1.26x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.64 sec: 1.26x faster                                                          |
| sqlglot_optimize           | 51.8 ms                                                         | 41.1 ms: 1.26x faster                                                           |
| sympy_expand               | 462 ms                                                          | 367 ms: 1.26x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 328 ms: 1.25x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 839 ms: 1.24x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 603 ms: 1.24x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 310 ms: 1.22x faster                                                            |
| async_tree_io              | 754 ms                                                          | 628 ms: 1.20x faster                                                            |
| json                       | 4.78 ms                                                         | 3.98 ms: 1.20x faster                                                           |
| tornado_http               | 118 ms                                                          | 99.1 ms: 1.19x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 1.85 us: 1.16x faster                                                           |
| xml_etree_generate         | 71.6 ms                                                         | 61.7 ms: 1.16x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 680 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 511 ms: 1.16x faster                                                            |
| 2to3                       | 282 ms                                                          | 246 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 504 ms: 1.15x faster                                                            |
| dask                       | 355 ms                                                          | 311 ms: 1.14x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.84 sec: 1.14x faster                                                          |
| meteor_contest             | 90.9 ms                                                         | 80.1 ms: 1.13x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.06 ms: 1.07x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 3.07 us: 1.07x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 71.1 ms: 1.06x faster                                                           |
| pickle                     | 7.99 us                                                         | 7.74 us: 1.03x faster                                                           |
| regex_dna                  | 122 ms                                                          | 119 ms: 1.02x faster                                                            |
| json_loads                 | 20.0 us                                                         | 19.7 us: 1.02x faster                                                           |
| pidigits                   | 203 ms                                                          | 200 ms: 1.02x faster                                                            |
| pickle_dict                | 20.1 us                                                         | 19.8 us: 1.01x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 113 ms: 1.01x faster                                                            |
| bench_mp_pool              | 70.9 ms                                                         | 73.0 ms: 1.03x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.42 ms: 1.03x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.6 sec: 1.03x slower                                                          |
| unpickle                   | 9.23 us                                                         | 9.57 us: 1.04x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| async_generators           | 260 ms                                                          | 273 ms: 1.05x slower                                                            |
| python_startup             | 22.0 ms                                                         | 23.2 ms: 1.06x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 655 us: 1.06x slower                                                            |
| python_startup_no_site     | 18.8 ms                                                         | 20.7 ms: 1.10x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 89.2 ms: 1.12x slower                                                           |
| pickle_list                | 3.27 us                                                         | 3.74 us: 1.15x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.23 ms: 1.18x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 211 ms: 1.87x slower                                                            |
| coverage                   | 58.0 ms                                                         | 477 ms: 8.21x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                    |
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: unknown