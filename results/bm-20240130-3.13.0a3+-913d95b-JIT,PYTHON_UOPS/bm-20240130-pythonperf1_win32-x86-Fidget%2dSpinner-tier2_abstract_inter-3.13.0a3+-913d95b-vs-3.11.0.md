
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 268 ms: 1.06x faster                                                                      |
| chameleon      | 8.08 ms                                                         | 6.17 ms: 1.31x faster                                                                     |
| docutils       | 2.10 sec                                                        | 1.86 sec: 1.13x faster                                                                    |
| tornado_http   | 118 ms                                                          | 103 ms: 1.15x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.16x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 264 ms: 1.30x faster                                                                      |
| async_tree_memoization     | 408 ms                                                          | 330 ms: 1.24x faster                                                                      |
| async_tree_memoization_tg  | 378 ms                                                          | 314 ms: 1.20x faster                                                                      |
| async_tree_io_tg           | 746 ms                                                          | 625 ms: 1.19x faster                                                                      |
| async_tree_none_tg         | 301 ms                                                          | 253 ms: 1.19x faster                                                                      |
| async_tree_io              | 754 ms                                                          | 634 ms: 1.19x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 513 ms: 1.12x faster                                                                      |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 527 ms: 1.12x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.19x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 90.8 ms: 1.39x faster                                                                     |
| float          | 76.1 ms                                                         | 55.7 ms: 1.37x faster                                                                     |
| pidigits       | 203 ms                                                          | 201 ms: 1.01x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 113 ms: 1.31x faster                                                                      |
| regex_effbot   | 1.82 ms                                                         | 1.91 ms: 1.04x slower                                                                     |
| regex_v8       | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                              |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 157 us: 1.47x faster                                                                      |
| tomli_loads          | 2.31 sec                                                        | 1.64 sec: 1.41x faster                                                                    |
| json_dumps           | 9.80 ms                                                         | 7.14 ms: 1.37x faster                                                                     |
| pickle_pure_python   | 309 us                                                          | 227 us: 1.36x faster                                                                      |
| xml_etree_process    | 55.0 ms                                                         | 42.8 ms: 1.29x faster                                                                     |
| unpickle_list        | 3.28 us                                                         | 2.79 us: 1.17x faster                                                                     |
| xml_etree_generate   | 71.6 ms                                                         | 62.3 ms: 1.15x faster                                                                     |
| xml_etree_iterparse  | 75.6 ms                                                         | 67.2 ms: 1.12x faster                                                                     |
| xml_etree_parse      | 114 ms                                                          | 104 ms: 1.10x faster                                                                      |
| pickle               | 7.99 us                                                         | 8.07 us: 1.01x slower                                                                     |
| pickle_list          | 3.27 us                                                         | 3.31 us: 1.02x slower                                                                     |
| pickle_dict          | 20.1 us                                                         | 20.5 us: 1.02x slower                                                                     |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.09x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                              |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.6 ms: 1.07x slower                                                                     |
| python_startup_no_site | 18.8 ms                                                         | 21.1 ms: 1.12x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.10x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 8.01 ms: 1.28x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 97.9 us: 4.88x faster                                                                     |
| generators                 | 52.2 ms                                                         | 25.0 ms: 2.09x faster                                                                     |
| logging_silent             | 119 ns                                                          | 66.3 ns: 1.80x faster                                                                     |
| richards_super             | 58.7 ms                                                         | 35.3 ms: 1.66x faster                                                                     |
| spectral_norm              | 122 ms                                                          | 77.4 ms: 1.57x faster                                                                     |
| richards                   | 48.8 ms                                                         | 31.1 ms: 1.57x faster                                                                     |
| coroutines                 | 23.7 ms                                                         | 15.2 ms: 1.56x faster                                                                     |
| deltablue                  | 4.10 ms                                                         | 2.62 ms: 1.56x faster                                                                     |
| unpack_sequence            | 65.2 ns                                                         | 41.9 ns: 1.56x faster                                                                     |
| sqlglot_parse              | 1.49 ms                                                         | 965 us: 1.54x faster                                                                      |
| deepcopy_memo              | 40.0 us                                                         | 26.1 us: 1.54x faster                                                                     |
| scimark_lu                 | 102 ms                                                          | 68.7 ms: 1.49x faster                                                                     |
| unpickle_pure_python       | 231 us                                                          | 157 us: 1.47x faster                                                                      |
| chaos                      | 84.4 ms                                                         | 58.0 ms: 1.46x faster                                                                     |
| sqlglot_transpile          | 1.78 ms                                                         | 1.23 ms: 1.45x faster                                                                     |
| scimark_sor                | 135 ms                                                          | 93.2 ms: 1.45x faster                                                                     |
| tomli_loads                | 2.31 sec                                                        | 1.64 sec: 1.41x faster                                                                    |
| nbody                      | 126 ms                                                          | 90.8 ms: 1.39x faster                                                                     |
| comprehensions             | 22.1 us                                                         | 15.9 us: 1.39x faster                                                                     |
| json_dumps                 | 9.80 ms                                                         | 7.14 ms: 1.37x faster                                                                     |
| float                      | 76.1 ms                                                         | 55.7 ms: 1.37x faster                                                                     |
| raytrace                   | 327 ms                                                          | 240 ms: 1.36x faster                                                                      |
| pickle_pure_python         | 309 us                                                          | 227 us: 1.36x faster                                                                      |
| deepcopy_reduce            | 3.32 us                                                         | 2.45 us: 1.35x faster                                                                     |
| deepcopy                   | 381 us                                                          | 284 us: 1.34x faster                                                                      |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.23 ms: 1.31x faster                                                                     |
| regex_compile              | 148 ms                                                          | 113 ms: 1.31x faster                                                                      |
| chameleon                  | 8.08 ms                                                         | 6.17 ms: 1.31x faster                                                                     |
| async_tree_none            | 343 ms                                                          | 264 ms: 1.30x faster                                                                      |
| logging_simple             | 10.8 us                                                         | 8.37 us: 1.29x faster                                                                     |
| sympy_sum                  | 149 ms                                                          | 116 ms: 1.29x faster                                                                      |
| fannkuch                   | 399 ms                                                          | 310 ms: 1.29x faster                                                                      |
| xml_etree_process          | 55.0 ms                                                         | 42.8 ms: 1.29x faster                                                                     |
| mako                       | 10.3 ms                                                         | 8.01 ms: 1.28x faster                                                                     |
| sympy_str                  | 283 ms                                                          | 221 ms: 1.28x faster                                                                      |
| logging_format             | 11.5 us                                                         | 9.01 us: 1.27x faster                                                                     |
| asyncio_tcp                | 787 ms                                                          | 622 ms: 1.26x faster                                                                      |
| nqueens                    | 111 ms                                                          | 89.6 ms: 1.24x faster                                                                     |
| async_tree_memoization     | 408 ms                                                          | 330 ms: 1.24x faster                                                                      |
| pyflate                    | 471 ms                                                          | 383 ms: 1.23x faster                                                                      |
| crypto_pyaes               | 79.4 ms                                                         | 64.7 ms: 1.23x faster                                                                     |
| sympy_expand               | 462 ms                                                          | 378 ms: 1.22x faster                                                                      |
| go                         | 147 ms                                                          | 122 ms: 1.20x faster                                                                      |
| async_tree_memoization_tg  | 378 ms                                                          | 314 ms: 1.20x faster                                                                      |
| pycparser                  | 1.04 sec                                                        | 869 ms: 1.20x faster                                                                      |
| async_tree_io_tg           | 746 ms                                                          | 625 ms: 1.19x faster                                                                      |
| async_tree_none_tg         | 301 ms                                                          | 253 ms: 1.19x faster                                                                      |
| async_tree_io              | 754 ms                                                          | 634 ms: 1.19x faster                                                                      |
| unpickle_list              | 3.28 us                                                         | 2.79 us: 1.17x faster                                                                     |
| sqlglot_optimize           | 51.8 ms                                                         | 44.3 ms: 1.17x faster                                                                     |
| pprint_pformat             | 1.70 sec                                                        | 1.46 sec: 1.16x faster                                                                    |
| sympy_integrate            | 19.9 ms                                                         | 17.2 ms: 1.16x faster                                                                     |
| sqlite_synth               | 2.15 us                                                         | 1.86 us: 1.16x faster                                                                     |
| tornado_http               | 118 ms                                                          | 103 ms: 1.15x faster                                                                      |
| pprint_safe_repr           | 819 ms                                                          | 711 ms: 1.15x faster                                                                      |
| xml_etree_generate         | 71.6 ms                                                         | 62.3 ms: 1.15x faster                                                                     |
| dask                       | 355 ms                                                          | 311 ms: 1.14x faster                                                                      |
| scimark_fft                | 291 ms                                                          | 257 ms: 1.13x faster                                                                      |
| docutils                   | 2.10 sec                                                        | 1.86 sec: 1.13x faster                                                                    |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 513 ms: 1.12x faster                                                                      |
| xml_etree_iterparse        | 75.6 ms                                                         | 67.2 ms: 1.12x faster                                                                     |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 527 ms: 1.12x faster                                                                      |
| mdp                        | 2.07 sec                                                        | 1.87 sec: 1.11x faster                                                                    |
| xml_etree_parse            | 114 ms                                                          | 104 ms: 1.10x faster                                                                      |
| bench_thread_pool          | 1.14 ms                                                         | 1.07 ms: 1.06x faster                                                                     |
| hexiom                     | 7.51 ms                                                         | 7.09 ms: 1.06x faster                                                                     |
| 2to3                       | 282 ms                                                          | 268 ms: 1.06x faster                                                                      |
| meteor_contest             | 90.9 ms                                                         | 88.3 ms: 1.03x faster                                                                     |
| scimark_monte_carlo        | 70.8 ms                                                         | 70.3 ms: 1.01x faster                                                                     |
| pidigits                   | 203 ms                                                          | 201 ms: 1.01x faster                                                                      |
| pickle                     | 7.99 us                                                         | 8.07 us: 1.01x slower                                                                     |
| pickle_list                | 3.27 us                                                         | 3.31 us: 1.02x slower                                                                     |
| pickle_dict                | 20.1 us                                                         | 20.5 us: 1.02x slower                                                                     |
| gc_traversal               | 1.38 ms                                                         | 1.41 ms: 1.03x slower                                                                     |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.8 sec: 1.04x slower                                                                    |
| regex_effbot               | 1.82 ms                                                         | 1.91 ms: 1.04x slower                                                                     |
| regex_v8                   | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                                     |
| python_startup             | 22.0 ms                                                         | 23.6 ms: 1.07x slower                                                                     |
| bench_mp_pool              | 70.9 ms                                                         | 76.3 ms: 1.08x slower                                                                     |
| create_gc_cycles           | 618 us                                                          | 668 us: 1.08x slower                                                                      |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.09x slower                                                                     |
| pathlib                    | 79.9 ms                                                         | 89.2 ms: 1.12x slower                                                                     |
| python_startup_no_site     | 18.8 ms                                                         | 21.1 ms: 1.12x slower                                                                     |
| async_generators           | 260 ms                                                          | 303 ms: 1.17x slower                                                                      |
| telco                      | 5.29 ms                                                         | 6.44 ms: 1.22x slower                                                                     |
| sqlglot_normalize          | 113 ms                                                          | 227 ms: 2.01x slower                                                                      |
| coverage                   | 58.0 ms                                                         | 483 ms: 8.32x slower                                                                      |
| Geometric mean             | (ref)                                                           | 1.18x faster                                                                              |

Benchmark hidden because not significant (3): json, json_loads, regex_dna
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown