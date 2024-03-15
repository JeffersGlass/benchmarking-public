
# Results vs. 3.11.0

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-x86
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 247 ms: 1.14x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.87 ms: 1.38x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.80 sec: 1.17x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.9 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 255 ms: 1.35x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 319 ms: 1.28x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 596 ms: 1.25x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 305 ms: 1.24x faster                                                            |
| async_tree_io              | 754 ms                                                          | 623 ms: 1.21x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 489 ms: 1.18x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 506 ms: 1.17x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.24x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 84.7 ms: 1.49x faster                                                           |
| float          | 76.1 ms                                                         | 58.8 ms: 1.29x faster                                                           |
| pidigits       | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 106 ms: 1.39x faster                                                            |
| regex_dna      | 122 ms                                                          | 123 ms: 1.01x slower                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.92 ms: 1.05x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.5 ms: 1.09x slower                                                           |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 152 us: 1.52x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 214 us: 1.44x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.89 ms: 1.42x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.63 sec: 1.42x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 41.7 ms: 1.32x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 61.2 ms: 1.17x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.5 ms: 1.10x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| unpickle_list        | 3.28 us                                                         | 3.15 us: 1.04x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.28 us: 1.00x slower                                                           |
| unpickle             | 9.23 us                                                         | 9.83 us: 1.07x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.16x faster                                                                    |

Benchmark hidden because not significant (3): pickle_dict, pickle, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.4 ms: 1.06x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.6 ms: 1.09x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.70 ms: 1.33x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 96.1 us: 4.98x faster                                                           |
| generators                 | 52.2 ms                                                         | 23.1 ms: 2.26x faster                                                           |
| logging_silent             | 119 ns                                                          | 60.4 ns: 1.97x faster                                                           |
| richards_super             | 58.7 ms                                                         | 32.5 ms: 1.80x faster                                                           |
| comprehensions             | 22.1 us                                                         | 13.0 us: 1.70x faster                                                           |
| richards                   | 48.8 ms                                                         | 29.4 ms: 1.66x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 904 us: 1.65x faster                                                            |
| deepcopy_memo              | 40.0 us                                                         | 24.8 us: 1.62x faster                                                           |
| chaos                      | 84.4 ms                                                         | 52.3 ms: 1.61x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 64.0 ms: 1.60x faster                                                           |
| scimark_sor                | 135 ms                                                          | 84.9 ms: 1.59x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.9 ms: 1.59x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 42.0 ns: 1.55x faster                                                           |
| raytrace                   | 327 ms                                                          | 211 ms: 1.55x faster                                                            |
| deltablue                  | 4.10 ms                                                         | 2.66 ms: 1.54x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.16 ms: 1.54x faster                                                           |
| spectral_norm              | 122 ms                                                          | 79.7 ms: 1.53x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 152 us: 1.52x faster                                                            |
| nbody                      | 126 ms                                                          | 84.7 ms: 1.49x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 214 us: 1.44x faster                                                            |
| hexiom                     | 7.51 ms                                                         | 5.21 ms: 1.44x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.89 ms: 1.42x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.63 sec: 1.42x faster                                                          |
| deepcopy                   | 381 us                                                          | 269 us: 1.42x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 50.3 ms: 1.41x faster                                                           |
| pyflate                    | 471 ms                                                          | 337 ms: 1.40x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 57.1 ms: 1.39x faster                                                           |
| regex_compile              | 148 ms                                                          | 106 ms: 1.39x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.22 sec: 1.39x faster                                                          |
| chameleon                  | 8.08 ms                                                         | 5.87 ms: 1.38x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 108 ms: 1.37x faster                                                            |
| go                         | 147 ms                                                          | 107 ms: 1.37x faster                                                            |
| nqueens                    | 111 ms                                                          | 81.8 ms: 1.36x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 604 ms: 1.36x faster                                                            |
| async_tree_none            | 343 ms                                                          | 255 ms: 1.35x faster                                                            |
| fannkuch                   | 399 ms                                                          | 299 ms: 1.34x faster                                                            |
| mako                       | 10.3 ms                                                         | 7.70 ms: 1.33x faster                                                           |
| sympy_str                  | 283 ms                                                          | 213 ms: 1.33x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.51 us: 1.32x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 41.7 ms: 1.32x faster                                                           |
| logging_simple             | 10.8 us                                                         | 8.24 us: 1.31x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.75 us: 1.31x faster                                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.25 ms: 1.30x faster                                                           |
| scimark_fft                | 291 ms                                                          | 225 ms: 1.30x faster                                                            |
| float                      | 76.1 ms                                                         | 58.8 ms: 1.29x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 319 ms: 1.28x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 15.6 ms: 1.28x faster                                                           |
| sympy_expand               | 462 ms                                                          | 367 ms: 1.26x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 596 ms: 1.25x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 41.7 ms: 1.24x faster                                                           |
| async_tree_memoization_tg  | 378 ms                                                          | 305 ms: 1.24x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.68 sec: 1.23x faster                                                          |
| pycparser                  | 1.04 sec                                                        | 858 ms: 1.22x faster                                                            |
| async_tree_io              | 754 ms                                                          | 623 ms: 1.21x faster                                                            |
| tornado_http               | 118 ms                                                          | 97.9 ms: 1.21x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 660 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 489 ms: 1.18x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 61.2 ms: 1.17x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.80 sec: 1.17x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 506 ms: 1.17x faster                                                            |
| dask                       | 355 ms                                                          | 308 ms: 1.15x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.88 us: 1.14x faster                                                           |
| 2to3                       | 282 ms                                                          | 247 ms: 1.14x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 80.0 ms: 1.14x faster                                                           |
| json                       | 4.78 ms                                                         | 4.22 ms: 1.13x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.5 ms: 1.10x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.08 ms: 1.06x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| unpickle_list              | 3.28 us                                                         | 3.15 us: 1.04x faster                                                           |
| pidigits                   | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| pickle_list                | 3.27 us                                                         | 3.28 us: 1.00x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.39 ms: 1.01x slower                                                           |
| regex_dna                  | 122 ms                                                          | 123 ms: 1.01x slower                                                            |
| bench_mp_pool              | 70.9 ms                                                         | 73.1 ms: 1.03x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| regex_effbot               | 1.82 ms                                                         | 1.92 ms: 1.05x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 655 us: 1.06x slower                                                            |
| python_startup             | 22.0 ms                                                         | 23.4 ms: 1.06x slower                                                           |
| unpickle                   | 9.23 us                                                         | 9.83 us: 1.07x slower                                                           |
| async_generators           | 260 ms                                                          | 279 ms: 1.07x slower                                                            |
| regex_v8                   | 15.2 ms                                                         | 16.5 ms: 1.09x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.6 ms: 1.09x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 89.2 ms: 1.12x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.92 ms: 1.12x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 212 ms: 1.87x slower                                                            |
| coverage                   | 58.0 ms                                                         | 489 ms: 8.43x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.24x faster                                                                    |

Benchmark hidden because not significant (3): pickle_dict, pickle, json_loads
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: unknown