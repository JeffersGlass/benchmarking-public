
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.23x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 250 ms: 1.13x faster                                                                      |
| chameleon      | 8.08 ms                                                         | 5.86 ms: 1.38x faster                                                                     |
| docutils       | 2.10 sec                                                        | 1.83 sec: 1.15x faster                                                                    |
| tornado_http   | 118 ms                                                          | 101 ms: 1.18x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.20x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 261 ms: 1.32x faster                                                                      |
| async_tree_memoization     | 408 ms                                                          | 325 ms: 1.25x faster                                                                      |
| async_tree_none_tg         | 301 ms                                                          | 240 ms: 1.25x faster                                                                      |
| async_tree_io_tg           | 746 ms                                                          | 605 ms: 1.23x faster                                                                      |
| async_tree_memoization_tg  | 378 ms                                                          | 311 ms: 1.21x faster                                                                      |
| async_tree_io              | 754 ms                                                          | 628 ms: 1.20x faster                                                                      |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 522 ms: 1.13x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 514 ms: 1.12x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.21x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 85.2 ms: 1.48x faster                                                                     |
| float          | 76.1 ms                                                         | 58.5 ms: 1.30x faster                                                                     |
| pidigits       | 203 ms                                                          | 202 ms: 1.01x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 108 ms: 1.36x faster                                                                      |
| regex_dna      | 122 ms                                                          | 126 ms: 1.04x slower                                                                      |
| regex_effbot   | 1.82 ms                                                         | 1.91 ms: 1.05x slower                                                                     |
| regex_v8       | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 149 us: 1.55x faster                                                                      |
| pickle_pure_python   | 309 us                                                          | 209 us: 1.48x faster                                                                      |
| json_dumps           | 9.80 ms                                                         | 6.62 ms: 1.48x faster                                                                     |
| tomli_loads          | 2.31 sec                                                        | 1.64 sec: 1.41x faster                                                                    |
| xml_etree_process    | 55.0 ms                                                         | 41.3 ms: 1.33x faster                                                                     |
| xml_etree_generate   | 71.6 ms                                                         | 60.6 ms: 1.18x faster                                                                     |
| unpickle_list        | 3.28 us                                                         | 2.87 us: 1.14x faster                                                                     |
| xml_etree_iterparse  | 75.6 ms                                                         | 69.2 ms: 1.09x faster                                                                     |
| pickle               | 7.99 us                                                         | 7.64 us: 1.05x faster                                                                     |
| xml_etree_parse      | 114 ms                                                          | 110 ms: 1.04x faster                                                                      |
| json_loads           | 20.0 us                                                         | 19.9 us: 1.01x faster                                                                     |
| pickle_dict          | 20.1 us                                                         | 20.2 us: 1.00x slower                                                                     |
| pickle_list          | 3.27 us                                                         | 3.48 us: 1.07x slower                                                                     |
| unpickle             | 9.23 us                                                         | 9.88 us: 1.07x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.17x faster                                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.5 ms: 1.07x slower                                                                     |
| python_startup_no_site | 18.8 ms                                                         | 21.1 ms: 1.12x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.10x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.86 ms: 1.31x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 94.8 us: 5.05x faster                                                                     |
| generators                 | 52.2 ms                                                         | 23.2 ms: 2.25x faster                                                                     |
| logging_silent             | 119 ns                                                          | 59.5 ns: 2.00x faster                                                                     |
| richards_super             | 58.7 ms                                                         | 33.5 ms: 1.75x faster                                                                     |
| comprehensions             | 22.1 us                                                         | 13.2 us: 1.67x faster                                                                     |
| richards                   | 48.8 ms                                                         | 29.3 ms: 1.67x faster                                                                     |
| unpack_sequence            | 65.2 ns                                                         | 39.5 ns: 1.65x faster                                                                     |
| scimark_lu                 | 102 ms                                                          | 62.1 ms: 1.65x faster                                                                     |
| coroutines                 | 23.7 ms                                                         | 14.6 ms: 1.63x faster                                                                     |
| chaos                      | 84.4 ms                                                         | 52.1 ms: 1.62x faster                                                                     |
| sqlglot_parse              | 1.49 ms                                                         | 920 us: 1.62x faster                                                                      |
| scimark_sor                | 135 ms                                                          | 83.7 ms: 1.62x faster                                                                     |
| deepcopy_memo              | 40.0 us                                                         | 25.4 us: 1.58x faster                                                                     |
| deltablue                  | 4.10 ms                                                         | 2.65 ms: 1.55x faster                                                                     |
| unpickle_pure_python       | 231 us                                                          | 149 us: 1.55x faster                                                                      |
| sqlglot_transpile          | 1.78 ms                                                         | 1.17 ms: 1.52x faster                                                                     |
| raytrace                   | 327 ms                                                          | 216 ms: 1.52x faster                                                                      |
| spectral_norm              | 122 ms                                                          | 81.6 ms: 1.49x faster                                                                     |
| pickle_pure_python         | 309 us                                                          | 209 us: 1.48x faster                                                                      |
| json_dumps                 | 9.80 ms                                                         | 6.62 ms: 1.48x faster                                                                     |
| nbody                      | 126 ms                                                          | 85.2 ms: 1.48x faster                                                                     |
| hexiom                     | 7.51 ms                                                         | 5.18 ms: 1.45x faster                                                                     |
| nqueens                    | 111 ms                                                          | 77.0 ms: 1.45x faster                                                                     |
| tomli_loads                | 2.31 sec                                                        | 1.64 sec: 1.41x faster                                                                    |
| pyflate                    | 471 ms                                                          | 337 ms: 1.40x faster                                                                      |
| chameleon                  | 8.08 ms                                                         | 5.86 ms: 1.38x faster                                                                     |
| scimark_monte_carlo        | 70.8 ms                                                         | 51.3 ms: 1.38x faster                                                                     |
| go                         | 147 ms                                                          | 107 ms: 1.37x faster                                                                      |
| regex_compile              | 148 ms                                                          | 108 ms: 1.36x faster                                                                      |
| crypto_pyaes               | 79.4 ms                                                         | 58.3 ms: 1.36x faster                                                                     |
| deepcopy                   | 381 us                                                          | 280 us: 1.36x faster                                                                      |
| deepcopy_reduce            | 3.32 us                                                         | 2.45 us: 1.35x faster                                                                     |
| fannkuch                   | 399 ms                                                          | 296 ms: 1.35x faster                                                                      |
| pprint_pformat             | 1.70 sec                                                        | 1.26 sec: 1.35x faster                                                                    |
| sympy_sum                  | 149 ms                                                          | 111 ms: 1.34x faster                                                                      |
| scimark_fft                | 291 ms                                                          | 217 ms: 1.34x faster                                                                      |
| xml_etree_process          | 55.0 ms                                                         | 41.3 ms: 1.33x faster                                                                     |
| sympy_str                  | 283 ms                                                          | 214 ms: 1.32x faster                                                                      |
| pprint_safe_repr           | 819 ms                                                          | 621 ms: 1.32x faster                                                                      |
| async_tree_none            | 343 ms                                                          | 261 ms: 1.32x faster                                                                      |
| mako                       | 10.3 ms                                                         | 7.86 ms: 1.31x faster                                                                     |
| float                      | 76.1 ms                                                         | 58.5 ms: 1.30x faster                                                                     |
| logging_simple             | 10.8 us                                                         | 8.37 us: 1.29x faster                                                                     |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.30 ms: 1.28x faster                                                                     |
| sympy_integrate            | 19.9 ms                                                         | 15.6 ms: 1.28x faster                                                                     |
| logging_format             | 11.5 us                                                         | 8.99 us: 1.27x faster                                                                     |
| async_tree_memoization     | 408 ms                                                          | 325 ms: 1.25x faster                                                                      |
| async_tree_none_tg         | 301 ms                                                          | 240 ms: 1.25x faster                                                                      |
| sympy_expand               | 462 ms                                                          | 372 ms: 1.24x faster                                                                      |
| sqlglot_optimize           | 51.8 ms                                                         | 41.8 ms: 1.24x faster                                                                     |
| mdp                        | 2.07 sec                                                        | 1.67 sec: 1.24x faster                                                                    |
| async_tree_io_tg           | 746 ms                                                          | 605 ms: 1.23x faster                                                                      |
| pycparser                  | 1.04 sec                                                        | 854 ms: 1.22x faster                                                                      |
| async_tree_memoization_tg  | 378 ms                                                          | 311 ms: 1.21x faster                                                                      |
| async_tree_io              | 754 ms                                                          | 628 ms: 1.20x faster                                                                      |
| xml_etree_generate         | 71.6 ms                                                         | 60.6 ms: 1.18x faster                                                                     |
| tornado_http               | 118 ms                                                          | 101 ms: 1.18x faster                                                                      |
| meteor_contest             | 90.9 ms                                                         | 77.6 ms: 1.17x faster                                                                     |
| sqlite_synth               | 2.15 us                                                         | 1.84 us: 1.17x faster                                                                     |
| asyncio_tcp                | 787 ms                                                          | 673 ms: 1.17x faster                                                                      |
| json                       | 4.78 ms                                                         | 4.14 ms: 1.15x faster                                                                     |
| docutils                   | 2.10 sec                                                        | 1.83 sec: 1.15x faster                                                                    |
| unpickle_list              | 3.28 us                                                         | 2.87 us: 1.14x faster                                                                     |
| dask                       | 355 ms                                                          | 312 ms: 1.14x faster                                                                      |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 522 ms: 1.13x faster                                                                      |
| 2to3                       | 282 ms                                                          | 250 ms: 1.13x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 514 ms: 1.12x faster                                                                      |
| xml_etree_iterparse        | 75.6 ms                                                         | 69.2 ms: 1.09x faster                                                                     |
| bench_thread_pool          | 1.14 ms                                                         | 1.07 ms: 1.06x faster                                                                     |
| pickle                     | 7.99 us                                                         | 7.64 us: 1.05x faster                                                                     |
| xml_etree_parse            | 114 ms                                                          | 110 ms: 1.04x faster                                                                      |
| json_loads                 | 20.0 us                                                         | 19.9 us: 1.01x faster                                                                     |
| pidigits                   | 203 ms                                                          | 202 ms: 1.01x faster                                                                      |
| pickle_dict                | 20.1 us                                                         | 20.2 us: 1.00x slower                                                                     |
| gc_traversal               | 1.38 ms                                                         | 1.40 ms: 1.02x slower                                                                     |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                                                    |
| regex_dna                  | 122 ms                                                          | 126 ms: 1.04x slower                                                                      |
| async_generators           | 260 ms                                                          | 271 ms: 1.04x slower                                                                      |
| regex_effbot               | 1.82 ms                                                         | 1.91 ms: 1.05x slower                                                                     |
| create_gc_cycles           | 618 us                                                          | 647 us: 1.05x slower                                                                      |
| bench_mp_pool              | 70.9 ms                                                         | 75.5 ms: 1.06x slower                                                                     |
| pickle_list                | 3.27 us                                                         | 3.48 us: 1.07x slower                                                                     |
| regex_v8                   | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                                     |
| python_startup             | 22.0 ms                                                         | 23.5 ms: 1.07x slower                                                                     |
| unpickle                   | 9.23 us                                                         | 9.88 us: 1.07x slower                                                                     |
| pathlib                    | 79.9 ms                                                         | 88.7 ms: 1.11x slower                                                                     |
| python_startup_no_site     | 18.8 ms                                                         | 21.1 ms: 1.12x slower                                                                     |
| telco                      | 5.29 ms                                                         | 6.07 ms: 1.15x slower                                                                     |
| sqlglot_normalize          | 113 ms                                                          | 213 ms: 1.88x slower                                                                      |
| coverage                   | 58.0 ms                                                         | 485 ms: 8.36x slower                                                                      |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                              |
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: unknown