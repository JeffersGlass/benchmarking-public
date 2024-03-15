
# Results vs. 3.11.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.32x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.26x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 229 ms: 1.23x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.63 ms: 1.43x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.69 sec: 1.24x faster                                                          |
| tornado_http   | 118 ms                                                          | 93.9 ms: 1.26x faster                                                           |
| Geometric mean | (ref)                                                           | 1.29x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 241 ms: 1.42x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 300 ms: 1.36x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 228 ms: 1.32x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 288 ms: 1.31x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 570 ms: 1.31x faster                                                            |
| async_tree_io              | 754 ms                                                          | 582 ms: 1.30x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 486 ms: 1.21x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 477 ms: 1.21x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.30x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 76.1 ms: 1.66x faster                                                           |
| float          | 76.1 ms                                                         | 54.9 ms: 1.39x faster                                                           |
| pidigits       | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.33x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 94.6 ms: 1.56x faster                                                           |
| regex_dna      | 122 ms                                                          | 120 ms: 1.02x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 15.9 ms: 1.05x slower                                                           |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 143 us: 1.62x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.45 ms: 1.52x faster                                                           |
| pickle_pure_python   | 309 us                                                          | 205 us: 1.51x faster                                                            |
| tomli_loads          | 2.31 sec                                                        | 1.62 sec: 1.43x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 40.2 ms: 1.37x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 57.6 ms: 1.24x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.78 us: 1.18x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 64.8 ms: 1.17x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 108 ms: 1.06x faster                                                            |
| json_loads           | 20.0 us                                                         | 19.6 us: 1.02x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.22 us: 1.01x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.9 us: 1.01x faster                                                           |
| unpickle             | 9.23 us                                                         | 9.96 us: 1.08x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.20x faster                                                                    |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.4 ms: 1.02x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.2 ms: 1.07x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 6.94 ms: 1.48x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 88.7 us: 5.39x faster                                                           |
| generators                 | 52.2 ms                                                         | 21.7 ms: 2.40x faster                                                           |
| logging_silent             | 119 ns                                                          | 58.5 ns: 2.04x faster                                                           |
| comprehensions             | 22.1 us                                                         | 11.5 us: 1.92x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.20 ms: 1.86x faster                                                           |
| spectral_norm              | 122 ms                                                          | 65.4 ms: 1.86x faster                                                           |
| chaos                      | 84.4 ms                                                         | 47.2 ms: 1.79x faster                                                           |
| richards_super             | 58.7 ms                                                         | 33.4 ms: 1.76x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 4.28 ms: 1.75x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 58.7 ms: 1.74x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 23.1 us: 1.74x faster                                                           |
| raytrace                   | 327 ms                                                          | 191 ms: 1.71x faster                                                            |
| richards                   | 48.8 ms                                                         | 28.6 ms: 1.71x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 876 us: 1.70x faster                                                            |
| unpack_sequence            | 65.2 ns                                                         | 39.0 ns: 1.67x faster                                                           |
| nbody                      | 126 ms                                                          | 76.1 ms: 1.66x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.4 ms: 1.65x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 143 us: 1.62x faster                                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.11 ms: 1.61x faster                                                           |
| scimark_sor                | 135 ms                                                          | 83.8 ms: 1.61x faster                                                           |
| regex_compile              | 148 ms                                                          | 94.6 ms: 1.56x faster                                                           |
| nqueens                    | 111 ms                                                          | 71.7 ms: 1.55x faster                                                           |
| scimark_monte_carlo        | 70.8 ms                                                         | 45.8 ms: 1.54x faster                                                           |
| go                         | 147 ms                                                          | 95.3 ms: 1.54x faster                                                           |
| pyflate                    | 471 ms                                                          | 309 ms: 1.53x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 52.2 ms: 1.52x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.45 ms: 1.52x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 205 us: 1.51x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 100 ms: 1.49x faster                                                            |
| mako                       | 10.3 ms                                                         | 6.94 ms: 1.48x faster                                                           |
| scimark_fft                | 291 ms                                                          | 197 ms: 1.48x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.15 sec: 1.47x faster                                                          |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 2.87 ms: 1.47x faster                                                           |
| deepcopy                   | 381 us                                                          | 263 us: 1.45x faster                                                            |
| pprint_safe_repr           | 819 ms                                                          | 565 ms: 1.45x faster                                                            |
| fannkuch                   | 399 ms                                                          | 276 ms: 1.45x faster                                                            |
| logging_simple             | 10.8 us                                                         | 7.48 us: 1.45x faster                                                           |
| sympy_str                  | 283 ms                                                          | 196 ms: 1.44x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.63 ms: 1.43x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.62 sec: 1.43x faster                                                          |
| async_tree_none            | 343 ms                                                          | 241 ms: 1.42x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.10 us: 1.41x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 14.2 ms: 1.40x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.37 us: 1.40x faster                                                           |
| float                      | 76.1 ms                                                         | 54.9 ms: 1.39x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 40.2 ms: 1.37x faster                                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 38.1 ms: 1.36x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 300 ms: 1.36x faster                                                            |
| sympy_expand               | 462 ms                                                          | 343 ms: 1.35x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 228 ms: 1.32x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 288 ms: 1.31x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 570 ms: 1.31x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 805 ms: 1.30x faster                                                            |
| async_tree_io              | 754 ms                                                          | 582 ms: 1.30x faster                                                            |
| tornado_http               | 118 ms                                                          | 93.9 ms: 1.26x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.65 sec: 1.25x faster                                                          |
| xml_etree_generate         | 71.6 ms                                                         | 57.6 ms: 1.24x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.69 sec: 1.24x faster                                                          |
| 2to3                       | 282 ms                                                          | 229 ms: 1.23x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 639 ms: 1.23x faster                                                            |
| dask                       | 355 ms                                                          | 291 ms: 1.22x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 486 ms: 1.21x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 477 ms: 1.21x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 75.6 ms: 1.20x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.78 us: 1.18x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 64.8 ms: 1.17x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 982 us: 1.16x faster                                                            |
| json                       | 4.78 ms                                                         | 4.13 ms: 1.16x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 1.87 us: 1.15x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 108 ms: 1.06x faster                                                            |
| pidigits                   | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| json_loads                 | 20.0 us                                                         | 19.6 us: 1.02x faster                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.02x faster                                                          |
| regex_dna                  | 122 ms                                                          | 120 ms: 1.02x faster                                                            |
| pickle_list                | 3.27 us                                                         | 3.22 us: 1.01x faster                                                           |
| pickle_dict                | 20.1 us                                                         | 19.9 us: 1.01x faster                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 71.5 ms: 1.01x slower                                                           |
| python_startup             | 22.0 ms                                                         | 22.4 ms: 1.02x slower                                                           |
| async_generators           | 260 ms                                                          | 267 ms: 1.03x slower                                                            |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 641 us: 1.04x slower                                                            |
| regex_v8                   | 15.2 ms                                                         | 15.9 ms: 1.05x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 84.0 ms: 1.05x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.2 ms: 1.07x slower                                                           |
| unpickle                   | 9.23 us                                                         | 9.96 us: 1.08x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.84 ms: 1.10x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 194 ms: 1.71x slower                                                            |
| coverage                   | 58.0 ms                                                         | 463 ms: 7.99x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.32x faster                                                                    |

Benchmark hidden because not significant (2): pickle, gc_traversal
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.29x
- 95% likely to have a speedup of 1.28x
- 99% likely to have a speedup of 1.26x


# Memory

- memory change: unknown