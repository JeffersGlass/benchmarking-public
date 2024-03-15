
# Results vs. 3.11.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-x86
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 235 ms: 1.20x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.74 ms: 1.41x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.74 sec: 1.21x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.2 ms: 1.22x faster                                                           |
| Geometric mean | (ref)                                                           | 1.26x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 240 ms: 1.43x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 302 ms: 1.35x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 572 ms: 1.31x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 231 ms: 1.31x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 290 ms: 1.30x faster                                                            |
| async_tree_io              | 754 ms                                                          | 588 ms: 1.28x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 496 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 485 ms: 1.19x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.29x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 81.8 ms: 1.54x faster                                                           |
| float          | 76.1 ms                                                         | 54.8 ms: 1.39x faster                                                           |
| pidigits       | 203 ms                                                          | 198 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                           | 1.30x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 96.3 ms: 1.53x faster                                                           |
| regex_dna      | 122 ms                                                          | 118 ms: 1.03x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.91 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.09x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 140 us: 1.66x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 204 us: 1.51x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.75 ms: 1.45x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.61 sec: 1.44x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 40.9 ms: 1.34x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 58.8 ms: 1.22x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 65.0 ms: 1.16x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.91 us: 1.13x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 108 ms: 1.06x faster                                                            |
| pickle               | 7.99 us                                                         | 7.72 us: 1.03x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.7 us: 1.02x faster                                                           |
| unpickle             | 9.23 us                                                         | 9.91 us: 1.07x slower                                                           |
| pickle_list          | 3.27 us                                                         | 3.64 us: 1.12x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.18x faster                                                                    |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.6 ms: 1.09x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 6.96 ms: 1.48x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 90.6 us: 5.28x faster                                                           |
| generators                 | 52.2 ms                                                         | 22.3 ms: 2.34x faster                                                           |
| logging_silent             | 119 ns                                                          | 55.9 ns: 2.13x faster                                                           |
| comprehensions             | 22.1 us                                                         | 11.6 us: 1.91x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.19 ms: 1.87x faster                                                           |
| spectral_norm              | 122 ms                                                          | 66.5 ms: 1.83x faster                                                           |
| richards_super             | 58.7 ms                                                         | 32.8 ms: 1.79x faster                                                           |
| chaos                      | 84.4 ms                                                         | 47.7 ms: 1.77x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 852 us: 1.75x faster                                                            |
| hexiom                     | 7.51 ms                                                         | 4.31 ms: 1.74x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 38.1 ns: 1.71x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 60.3 ms: 1.70x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 23.8 us: 1.68x faster                                                           |
| richards                   | 48.8 ms                                                         | 29.2 ms: 1.67x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 140 us: 1.66x faster                                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.09 ms: 1.64x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.5 ms: 1.63x faster                                                           |
| raytrace                   | 327 ms                                                          | 201 ms: 1.63x faster                                                            |
| scimark_sor                | 135 ms                                                          | 83.7 ms: 1.62x faster                                                           |
| nqueens                    | 111 ms                                                          | 70.9 ms: 1.57x faster                                                           |
| nbody                      | 126 ms                                                          | 81.8 ms: 1.54x faster                                                           |
| regex_compile              | 148 ms                                                          | 96.3 ms: 1.53x faster                                                           |
| scimark_monte_carlo        | 70.8 ms                                                         | 46.3 ms: 1.53x faster                                                           |
| pyflate                    | 471 ms                                                          | 310 ms: 1.52x faster                                                            |
| pickle_pure_python         | 309 us                                                          | 204 us: 1.51x faster                                                            |
| go                         | 147 ms                                                          | 97.6 ms: 1.51x faster                                                           |
| crypto_pyaes               | 79.4 ms                                                         | 53.4 ms: 1.49x faster                                                           |
| fannkuch                   | 399 ms                                                          | 269 ms: 1.48x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 101 ms: 1.48x faster                                                            |
| mako                       | 10.3 ms                                                         | 6.96 ms: 1.48x faster                                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 2.91 ms: 1.46x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.75 ms: 1.45x faster                                                           |
| sympy_str                  | 283 ms                                                          | 196 ms: 1.44x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.61 sec: 1.44x faster                                                          |
| pprint_pformat             | 1.70 sec                                                        | 1.19 sec: 1.43x faster                                                          |
| deepcopy                   | 381 us                                                          | 267 us: 1.43x faster                                                            |
| async_tree_none            | 343 ms                                                          | 240 ms: 1.43x faster                                                            |
| scimark_fft                | 291 ms                                                          | 206 ms: 1.42x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.35 us: 1.41x faster                                                           |
| logging_simple             | 10.8 us                                                         | 7.66 us: 1.41x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 5.74 ms: 1.41x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 582 ms: 1.41x faster                                                            |
| float                      | 76.1 ms                                                         | 54.8 ms: 1.39x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.36 us: 1.37x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 14.5 ms: 1.37x faster                                                           |
| sympy_expand               | 462 ms                                                          | 340 ms: 1.36x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 302 ms: 1.35x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 38.6 ms: 1.34x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 40.9 ms: 1.34x faster                                                           |
| pycparser                  | 1.04 sec                                                        | 793 ms: 1.32x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.58 sec: 1.31x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 572 ms: 1.31x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 231 ms: 1.31x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 290 ms: 1.30x faster                                                            |
| async_tree_io              | 754 ms                                                          | 588 ms: 1.28x faster                                                            |
| tornado_http               | 118 ms                                                          | 97.2 ms: 1.22x faster                                                           |
| xml_etree_generate         | 71.6 ms                                                         | 58.8 ms: 1.22x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.74 sec: 1.21x faster                                                          |
| 2to3                       | 282 ms                                                          | 235 ms: 1.20x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 75.7 ms: 1.20x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 659 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 496 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 485 ms: 1.19x faster                                                            |
| dask                       | 355 ms                                                          | 299 ms: 1.18x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.83 us: 1.17x faster                                                           |
| json                       | 4.78 ms                                                         | 4.10 ms: 1.17x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 65.0 ms: 1.16x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.91 us: 1.13x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.03 ms: 1.10x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 108 ms: 1.06x faster                                                            |
| pickle                     | 7.99 us                                                         | 7.72 us: 1.03x faster                                                           |
| regex_dna                  | 122 ms                                                          | 118 ms: 1.03x faster                                                            |
| pidigits                   | 203 ms                                                          | 198 ms: 1.02x faster                                                            |
| pickle_dict                | 20.1 us                                                         | 19.7 us: 1.02x faster                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 71.6 ms: 1.01x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.39 ms: 1.01x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.3 sec: 1.01x slower                                                          |
| async_generators           | 260 ms                                                          | 266 ms: 1.02x slower                                                            |
| python_startup             | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.91 ms: 1.04x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 654 us: 1.06x slower                                                            |
| unpickle                   | 9.23 us                                                         | 9.91 us: 1.07x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.76 ms: 1.09x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.6 ms: 1.09x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 87.5 ms: 1.10x slower                                                           |
| pickle_list                | 3.27 us                                                         | 3.64 us: 1.12x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 199 ms: 1.76x slower                                                            |
| coverage                   | 58.0 ms                                                         | 474 ms: 8.16x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.30x faster                                                                    |

Benchmark hidden because not significant (1): json_loads
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.28x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: unknown