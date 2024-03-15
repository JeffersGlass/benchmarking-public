
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.23x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 250 ms: 1.13x faster                                                                      |
| chameleon      | 8.08 ms                                                         | 5.82 ms: 1.39x faster                                                                     |
| docutils       | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                                    |
| tornado_http   | 118 ms                                                          | 98.8 ms: 1.20x faster                                                                     |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 255 ms: 1.34x faster                                                                      |
| async_tree_memoization     | 408 ms                                                          | 316 ms: 1.29x faster                                                                      |
| async_tree_io_tg           | 746 ms                                                          | 595 ms: 1.25x faster                                                                      |
| async_tree_memoization_tg  | 378 ms                                                          | 306 ms: 1.23x faster                                                                      |
| async_tree_none_tg         | 301 ms                                                          | 244 ms: 1.23x faster                                                                      |
| async_tree_io              | 754 ms                                                          | 620 ms: 1.22x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 505 ms: 1.14x faster                                                                      |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 521 ms: 1.13x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 87.0 ms: 1.45x faster                                                                     |
| float          | 76.1 ms                                                         | 61.2 ms: 1.24x faster                                                                     |
| pidigits       | 203 ms                                                          | 204 ms: 1.00x slower                                                                      |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 108 ms: 1.37x faster                                                                      |
| regex_dna      | 122 ms                                                          | 123 ms: 1.01x slower                                                                      |
| regex_effbot   | 1.82 ms                                                         | 1.92 ms: 1.05x slower                                                                     |
| regex_v8       | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 153 us: 1.51x faster                                                                      |
| pickle_pure_python   | 309 us                                                          | 209 us: 1.48x faster                                                                      |
| json_dumps           | 9.80 ms                                                         | 6.87 ms: 1.43x faster                                                                     |
| tomli_loads          | 2.31 sec                                                        | 1.65 sec: 1.40x faster                                                                    |
| xml_etree_process    | 55.0 ms                                                         | 42.2 ms: 1.30x faster                                                                     |
| xml_etree_generate   | 71.6 ms                                                         | 61.2 ms: 1.17x faster                                                                     |
| unpickle_list        | 3.28 us                                                         | 3.05 us: 1.07x faster                                                                     |
| xml_etree_iterparse  | 75.6 ms                                                         | 70.5 ms: 1.07x faster                                                                     |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                                      |
| pickle               | 7.99 us                                                         | 7.78 us: 1.03x faster                                                                     |
| pickle_dict          | 20.1 us                                                         | 20.2 us: 1.00x slower                                                                     |
| unpickle             | 9.23 us                                                         | 9.90 us: 1.07x slower                                                                     |
| pickle_list          | 3.27 us                                                         | 3.69 us: 1.13x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                              |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.8 ms: 1.08x slower                                                                     |
| python_startup_no_site | 18.8 ms                                                         | 21.5 ms: 1.14x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.11x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 8.34 ms: 1.23x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 95.4 us: 5.02x faster                                                                     |
| generators                 | 52.2 ms                                                         | 23.2 ms: 2.25x faster                                                                     |
| logging_silent             | 119 ns                                                          | 60.2 ns: 1.98x faster                                                                     |
| richards_super             | 58.7 ms                                                         | 33.1 ms: 1.78x faster                                                                     |
| sqlglot_parse              | 1.49 ms                                                         | 883 us: 1.69x faster                                                                      |
| coroutines                 | 23.7 ms                                                         | 14.2 ms: 1.67x faster                                                                     |
| richards                   | 48.8 ms                                                         | 29.4 ms: 1.66x faster                                                                     |
| scimark_sor                | 135 ms                                                          | 82.3 ms: 1.64x faster                                                                     |
| scimark_lu                 | 102 ms                                                          | 62.6 ms: 1.63x faster                                                                     |
| deepcopy_memo              | 40.0 us                                                         | 24.6 us: 1.63x faster                                                                     |
| chaos                      | 84.4 ms                                                         | 52.1 ms: 1.62x faster                                                                     |
| sqlglot_transpile          | 1.78 ms                                                         | 1.13 ms: 1.58x faster                                                                     |
| comprehensions             | 22.1 us                                                         | 14.0 us: 1.58x faster                                                                     |
| unpack_sequence            | 65.2 ns                                                         | 41.4 ns: 1.57x faster                                                                     |
| raytrace                   | 327 ms                                                          | 209 ms: 1.56x faster                                                                      |
| unpickle_pure_python       | 231 us                                                          | 153 us: 1.51x faster                                                                      |
| pickle_pure_python         | 309 us                                                          | 209 us: 1.48x faster                                                                      |
| nbody                      | 126 ms                                                          | 87.0 ms: 1.45x faster                                                                     |
| nqueens                    | 111 ms                                                          | 77.5 ms: 1.44x faster                                                                     |
| spectral_norm              | 122 ms                                                          | 85.0 ms: 1.43x faster                                                                     |
| json_dumps                 | 9.80 ms                                                         | 6.87 ms: 1.43x faster                                                                     |
| deltablue                  | 4.10 ms                                                         | 2.89 ms: 1.42x faster                                                                     |
| tomli_loads                | 2.31 sec                                                        | 1.65 sec: 1.40x faster                                                                    |
| crypto_pyaes               | 79.4 ms                                                         | 56.7 ms: 1.40x faster                                                                     |
| chameleon                  | 8.08 ms                                                         | 5.82 ms: 1.39x faster                                                                     |
| go                         | 147 ms                                                          | 106 ms: 1.39x faster                                                                      |
| deepcopy                   | 381 us                                                          | 275 us: 1.39x faster                                                                      |
| fannkuch                   | 399 ms                                                          | 288 ms: 1.39x faster                                                                      |
| deepcopy_reduce            | 3.32 us                                                         | 2.39 us: 1.39x faster                                                                     |
| pyflate                    | 471 ms                                                          | 341 ms: 1.38x faster                                                                      |
| hexiom                     | 7.51 ms                                                         | 5.47 ms: 1.37x faster                                                                     |
| regex_compile              | 148 ms                                                          | 108 ms: 1.37x faster                                                                      |
| scimark_monte_carlo        | 70.8 ms                                                         | 52.2 ms: 1.36x faster                                                                     |
| sympy_sum                  | 149 ms                                                          | 110 ms: 1.35x faster                                                                      |
| async_tree_none            | 343 ms                                                          | 255 ms: 1.34x faster                                                                      |
| scimark_fft                | 291 ms                                                          | 217 ms: 1.34x faster                                                                      |
| pprint_pformat             | 1.70 sec                                                        | 1.26 sec: 1.34x faster                                                                    |
| sympy_str                  | 283 ms                                                          | 214 ms: 1.32x faster                                                                      |
| pprint_safe_repr           | 819 ms                                                          | 622 ms: 1.32x faster                                                                      |
| logging_format             | 11.5 us                                                         | 8.72 us: 1.31x faster                                                                     |
| logging_simple             | 10.8 us                                                         | 8.28 us: 1.31x faster                                                                     |
| xml_etree_process          | 55.0 ms                                                         | 42.2 ms: 1.30x faster                                                                     |
| sympy_integrate            | 19.9 ms                                                         | 15.4 ms: 1.29x faster                                                                     |
| async_tree_memoization     | 408 ms                                                          | 316 ms: 1.29x faster                                                                      |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.37 ms: 1.26x faster                                                                     |
| mdp                        | 2.07 sec                                                        | 1.65 sec: 1.26x faster                                                                    |
| pycparser                  | 1.04 sec                                                        | 832 ms: 1.25x faster                                                                      |
| async_tree_io_tg           | 746 ms                                                          | 595 ms: 1.25x faster                                                                      |
| sympy_expand               | 462 ms                                                          | 369 ms: 1.25x faster                                                                      |
| sqlglot_optimize           | 51.8 ms                                                         | 41.7 ms: 1.24x faster                                                                     |
| float                      | 76.1 ms                                                         | 61.2 ms: 1.24x faster                                                                     |
| async_tree_memoization_tg  | 378 ms                                                          | 306 ms: 1.23x faster                                                                      |
| mako                       | 10.3 ms                                                         | 8.34 ms: 1.23x faster                                                                     |
| async_tree_none_tg         | 301 ms                                                          | 244 ms: 1.23x faster                                                                      |
| async_tree_io              | 754 ms                                                          | 620 ms: 1.22x faster                                                                      |
| tornado_http               | 118 ms                                                          | 98.8 ms: 1.20x faster                                                                     |
| xml_etree_generate         | 71.6 ms                                                         | 61.2 ms: 1.17x faster                                                                     |
| json                       | 4.78 ms                                                         | 4.10 ms: 1.17x faster                                                                     |
| docutils                   | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                                    |
| asyncio_tcp                | 787 ms                                                          | 680 ms: 1.16x faster                                                                      |
| dask                       | 355 ms                                                          | 308 ms: 1.15x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 505 ms: 1.14x faster                                                                      |
| meteor_contest             | 90.9 ms                                                         | 80.0 ms: 1.14x faster                                                                     |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 521 ms: 1.13x faster                                                                      |
| 2to3                       | 282 ms                                                          | 250 ms: 1.13x faster                                                                      |
| sqlite_synth               | 2.15 us                                                         | 1.90 us: 1.13x faster                                                                     |
| unpickle_list              | 3.28 us                                                         | 3.05 us: 1.07x faster                                                                     |
| xml_etree_iterparse        | 75.6 ms                                                         | 70.5 ms: 1.07x faster                                                                     |
| bench_thread_pool          | 1.14 ms                                                         | 1.08 ms: 1.06x faster                                                                     |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                                      |
| pickle                     | 7.99 us                                                         | 7.78 us: 1.03x faster                                                                     |
| pickle_dict                | 20.1 us                                                         | 20.2 us: 1.00x slower                                                                     |
| pidigits                   | 203 ms                                                          | 204 ms: 1.00x slower                                                                      |
| regex_dna                  | 122 ms                                                          | 123 ms: 1.01x slower                                                                      |
| gc_traversal               | 1.38 ms                                                         | 1.40 ms: 1.02x slower                                                                     |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.5 sec: 1.03x slower                                                                    |
| bench_mp_pool              | 70.9 ms                                                         | 74.6 ms: 1.05x slower                                                                     |
| regex_effbot               | 1.82 ms                                                         | 1.92 ms: 1.05x slower                                                                     |
| async_generators           | 260 ms                                                          | 275 ms: 1.06x slower                                                                      |
| regex_v8                   | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                                     |
| unpickle                   | 9.23 us                                                         | 9.90 us: 1.07x slower                                                                     |
| python_startup             | 22.0 ms                                                         | 23.8 ms: 1.08x slower                                                                     |
| create_gc_cycles           | 618 us                                                          | 671 us: 1.09x slower                                                                      |
| telco                      | 5.29 ms                                                         | 5.75 ms: 1.09x slower                                                                     |
| pathlib                    | 79.9 ms                                                         | 89.5 ms: 1.12x slower                                                                     |
| pickle_list                | 3.27 us                                                         | 3.69 us: 1.13x slower                                                                     |
| python_startup_no_site     | 18.8 ms                                                         | 21.5 ms: 1.14x slower                                                                     |
| sqlglot_normalize          | 113 ms                                                          | 213 ms: 1.88x slower                                                                      |
| coverage                   | 58.0 ms                                                         | 505 ms: 8.71x slower                                                                      |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                              |

Benchmark hidden because not significant (1): json_loads
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: unknown