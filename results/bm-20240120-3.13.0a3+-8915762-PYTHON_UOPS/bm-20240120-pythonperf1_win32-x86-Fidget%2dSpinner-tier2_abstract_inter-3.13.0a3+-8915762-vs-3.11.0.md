
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: 8915762
- commit date: 2024-01-20
- overall geometric mean: 1.25x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 252 ms: 1.12x faster                                                                      |
| chameleon      | 8.08 ms                                                         | 5.67 ms: 1.43x faster                                                                     |
| docutils       | 2.10 sec                                                        | 1.83 sec: 1.15x faster                                                                    |
| tornado_http   | 118 ms                                                          | 101 ms: 1.18x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 249 ms: 1.38x faster                                                                      |
| async_tree_memoization     | 408 ms                                                          | 310 ms: 1.32x faster                                                                      |
| async_tree_io_tg           | 746 ms                                                          | 582 ms: 1.28x faster                                                                      |
| async_tree_none_tg         | 301 ms                                                          | 235 ms: 1.28x faster                                                                      |
| async_tree_memoization_tg  | 378 ms                                                          | 296 ms: 1.27x faster                                                                      |
| async_tree_io              | 754 ms                                                          | 600 ms: 1.26x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 493 ms: 1.17x faster                                                                      |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 505 ms: 1.17x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.26x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 85.9 ms: 1.47x faster                                                                     |
| float          | 76.1 ms                                                         | 56.2 ms: 1.35x faster                                                                     |
| pidigits       | 203 ms                                                          | 198 ms: 1.02x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.27x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 107 ms: 1.38x faster                                                                      |
| regex_dna      | 122 ms                                                          | 117 ms: 1.04x faster                                                                      |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.03x slower                                                                     |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.05x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 149 us: 1.55x faster                                                                      |
| pickle_pure_python   | 309 us                                                          | 209 us: 1.48x faster                                                                      |
| json_dumps           | 9.80 ms                                                         | 6.64 ms: 1.47x faster                                                                     |
| tomli_loads          | 2.31 sec                                                        | 1.62 sec: 1.43x faster                                                                    |
| xml_etree_process    | 55.0 ms                                                         | 41.9 ms: 1.31x faster                                                                     |
| xml_etree_generate   | 71.6 ms                                                         | 59.8 ms: 1.20x faster                                                                     |
| unpickle_list        | 3.28 us                                                         | 2.83 us: 1.16x faster                                                                     |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.1 ms: 1.11x faster                                                                     |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                                      |
| pickle               | 7.99 us                                                         | 7.86 us: 1.02x faster                                                                     |
| json_loads           | 20.0 us                                                         | 19.9 us: 1.01x faster                                                                     |
| pickle_list          | 3.27 us                                                         | 3.25 us: 1.01x faster                                                                     |
| pickle_dict          | 20.1 us                                                         | 20.2 us: 1.01x slower                                                                     |
| unpickle             | 9.23 us                                                         | 9.55 us: 1.04x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.18x faster                                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.7 ms: 1.03x slower                                                                     |
| python_startup_no_site | 18.8 ms                                                         | 20.6 ms: 1.10x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.74 ms: 1.33x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 92.3 us: 5.18x faster                                                                     |
| generators                 | 52.2 ms                                                         | 24.0 ms: 2.17x faster                                                                     |
| logging_silent             | 119 ns                                                          | 60.4 ns: 1.97x faster                                                                     |
| richards_super             | 58.7 ms                                                         | 33.3 ms: 1.76x faster                                                                     |
| richards                   | 48.8 ms                                                         | 29.6 ms: 1.65x faster                                                                     |
| scimark_lu                 | 102 ms                                                          | 62.0 ms: 1.65x faster                                                                     |
| scimark_sor                | 135 ms                                                          | 82.1 ms: 1.65x faster                                                                     |
| comprehensions             | 22.1 us                                                         | 13.5 us: 1.64x faster                                                                     |
| sqlglot_parse              | 1.49 ms                                                         | 913 us: 1.63x faster                                                                      |
| coroutines                 | 23.7 ms                                                         | 14.7 ms: 1.62x faster                                                                     |
| chaos                      | 84.4 ms                                                         | 52.5 ms: 1.61x faster                                                                     |
| deepcopy_memo              | 40.0 us                                                         | 25.1 us: 1.60x faster                                                                     |
| unpack_sequence            | 65.2 ns                                                         | 41.6 ns: 1.57x faster                                                                     |
| raytrace                   | 327 ms                                                          | 211 ms: 1.56x faster                                                                      |
| unpickle_pure_python       | 231 us                                                          | 149 us: 1.55x faster                                                                      |
| deltablue                  | 4.10 ms                                                         | 2.67 ms: 1.53x faster                                                                     |
| sqlglot_transpile          | 1.78 ms                                                         | 1.17 ms: 1.53x faster                                                                     |
| spectral_norm              | 122 ms                                                          | 79.8 ms: 1.52x faster                                                                     |
| pickle_pure_python         | 309 us                                                          | 209 us: 1.48x faster                                                                      |
| json_dumps                 | 9.80 ms                                                         | 6.64 ms: 1.47x faster                                                                     |
| nbody                      | 126 ms                                                          | 85.9 ms: 1.47x faster                                                                     |
| hexiom                     | 7.51 ms                                                         | 5.21 ms: 1.44x faster                                                                     |
| nqueens                    | 111 ms                                                          | 77.8 ms: 1.43x faster                                                                     |
| scimark_monte_carlo        | 70.8 ms                                                         | 49.6 ms: 1.43x faster                                                                     |
| tomli_loads                | 2.31 sec                                                        | 1.62 sec: 1.43x faster                                                                    |
| chameleon                  | 8.08 ms                                                         | 5.67 ms: 1.43x faster                                                                     |
| crypto_pyaes               | 79.4 ms                                                         | 55.7 ms: 1.42x faster                                                                     |
| pyflate                    | 471 ms                                                          | 333 ms: 1.42x faster                                                                      |
| scimark_fft                | 291 ms                                                          | 207 ms: 1.41x faster                                                                      |
| go                         | 147 ms                                                          | 105 ms: 1.40x faster                                                                      |
| fannkuch                   | 399 ms                                                          | 288 ms: 1.39x faster                                                                      |
| regex_compile              | 148 ms                                                          | 107 ms: 1.38x faster                                                                      |
| async_tree_none            | 343 ms                                                          | 249 ms: 1.38x faster                                                                      |
| pprint_pformat             | 1.70 sec                                                        | 1.24 sec: 1.37x faster                                                                    |
| pprint_safe_repr           | 819 ms                                                          | 599 ms: 1.37x faster                                                                      |
| deepcopy                   | 381 us                                                          | 279 us: 1.36x faster                                                                      |
| sympy_sum                  | 149 ms                                                          | 109 ms: 1.36x faster                                                                      |
| float                      | 76.1 ms                                                         | 56.2 ms: 1.35x faster                                                                     |
| logging_simple             | 10.8 us                                                         | 8.06 us: 1.34x faster                                                                     |
| deepcopy_reduce            | 3.32 us                                                         | 2.49 us: 1.33x faster                                                                     |
| mako                       | 10.3 ms                                                         | 7.74 ms: 1.33x faster                                                                     |
| sympy_str                  | 283 ms                                                          | 213 ms: 1.33x faster                                                                      |
| async_tree_memoization     | 408 ms                                                          | 310 ms: 1.32x faster                                                                      |
| logging_format             | 11.5 us                                                         | 8.71 us: 1.32x faster                                                                     |
| xml_etree_process          | 55.0 ms                                                         | 41.9 ms: 1.31x faster                                                                     |
| sympy_integrate            | 19.9 ms                                                         | 15.4 ms: 1.29x faster                                                                     |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.28 ms: 1.29x faster                                                                     |
| async_tree_io_tg           | 746 ms                                                          | 582 ms: 1.28x faster                                                                      |
| async_tree_none_tg         | 301 ms                                                          | 235 ms: 1.28x faster                                                                      |
| async_tree_memoization_tg  | 378 ms                                                          | 296 ms: 1.27x faster                                                                      |
| async_tree_io              | 754 ms                                                          | 600 ms: 1.26x faster                                                                      |
| pycparser                  | 1.04 sec                                                        | 837 ms: 1.25x faster                                                                      |
| asyncio_tcp                | 787 ms                                                          | 634 ms: 1.24x faster                                                                      |
| sqlglot_optimize           | 51.8 ms                                                         | 41.8 ms: 1.24x faster                                                                     |
| sympy_expand               | 462 ms                                                          | 376 ms: 1.23x faster                                                                      |
| mdp                        | 2.07 sec                                                        | 1.71 sec: 1.21x faster                                                                    |
| xml_etree_generate         | 71.6 ms                                                         | 59.8 ms: 1.20x faster                                                                     |
| tornado_http               | 118 ms                                                          | 101 ms: 1.18x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 493 ms: 1.17x faster                                                                      |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 505 ms: 1.17x faster                                                                      |
| json                       | 4.78 ms                                                         | 4.10 ms: 1.17x faster                                                                     |
| meteor_contest             | 90.9 ms                                                         | 78.1 ms: 1.16x faster                                                                     |
| dask                       | 355 ms                                                          | 307 ms: 1.16x faster                                                                      |
| unpickle_list              | 3.28 us                                                         | 2.83 us: 1.16x faster                                                                     |
| sqlite_synth               | 2.15 us                                                         | 1.86 us: 1.15x faster                                                                     |
| docutils                   | 2.10 sec                                                        | 1.83 sec: 1.15x faster                                                                    |
| 2to3                       | 282 ms                                                          | 252 ms: 1.12x faster                                                                      |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.1 ms: 1.11x faster                                                                     |
| bench_thread_pool          | 1.14 ms                                                         | 1.03 ms: 1.11x faster                                                                     |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                                      |
| regex_dna                  | 122 ms                                                          | 117 ms: 1.04x faster                                                                      |
| pidigits                   | 203 ms                                                          | 198 ms: 1.02x faster                                                                      |
| pickle                     | 7.99 us                                                         | 7.86 us: 1.02x faster                                                                     |
| json_loads                 | 20.0 us                                                         | 19.9 us: 1.01x faster                                                                     |
| pickle_list                | 3.27 us                                                         | 3.25 us: 1.01x faster                                                                     |
| pickle_dict                | 20.1 us                                                         | 20.2 us: 1.01x slower                                                                     |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.4 sec: 1.02x slower                                                                    |
| gc_traversal               | 1.38 ms                                                         | 1.41 ms: 1.02x slower                                                                     |
| python_startup             | 22.0 ms                                                         | 22.7 ms: 1.03x slower                                                                     |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.03x slower                                                                     |
| unpickle                   | 9.23 us                                                         | 9.55 us: 1.04x slower                                                                     |
| async_generators           | 260 ms                                                          | 270 ms: 1.04x slower                                                                      |
| create_gc_cycles           | 618 us                                                          | 642 us: 1.04x slower                                                                      |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.05x slower                                                                     |
| bench_mp_pool              | 70.9 ms                                                         | 74.9 ms: 1.06x slower                                                                     |
| python_startup_no_site     | 18.8 ms                                                         | 20.6 ms: 1.10x slower                                                                     |
| pathlib                    | 79.9 ms                                                         | 88.1 ms: 1.10x slower                                                                     |
| telco                      | 5.29 ms                                                         | 6.14 ms: 1.16x slower                                                                     |
| sqlglot_normalize          | 113 ms                                                          | 216 ms: 1.91x slower                                                                      |
| coverage                   | 58.0 ms                                                         | 487 ms: 8.40x slower                                                                      |
| Geometric mean             | (ref)                                                           | 1.25x faster                                                                              |
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: unknown