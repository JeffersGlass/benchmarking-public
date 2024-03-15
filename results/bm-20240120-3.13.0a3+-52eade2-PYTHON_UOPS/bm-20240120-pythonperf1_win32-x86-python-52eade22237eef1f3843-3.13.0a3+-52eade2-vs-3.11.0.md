
# Results vs. 3.11.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-x86
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.26x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 241 ms: 1.17x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.80 ms: 1.39x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.80 sec: 1.16x faster                                                          |
| tornado_http   | 118 ms                                                          | 101 ms: 1.18x faster                                                            |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 252 ms: 1.36x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 316 ms: 1.29x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 588 ms: 1.27x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 238 ms: 1.26x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 300 ms: 1.26x faster                                                            |
| async_tree_io              | 754 ms                                                          | 605 ms: 1.25x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 510 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 503 ms: 1.15x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 85.3 ms: 1.48x faster                                                           |
| float          | 76.1 ms                                                         | 57.4 ms: 1.33x faster                                                           |
| pidigits       | 203 ms                                                          | 197 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.26x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 103 ms: 1.43x faster                                                            |
| regex_dna      | 122 ms                                                          | 116 ms: 1.05x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.87 ms: 1.03x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 15.9 ms: 1.05x slower                                                           |
| Geometric mean | (ref)                                                           | 1.09x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 153 us: 1.51x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 212 us: 1.46x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.75 ms: 1.45x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.61 sec: 1.44x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 41.0 ms: 1.34x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 59.2 ms: 1.21x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.94 us: 1.11x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.4 ms: 1.11x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pickle               | 7.99 us                                                         | 7.67 us: 1.04x faster                                                           |
| json_loads           | 20.0 us                                                         | 19.7 us: 1.02x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.22 us: 1.02x faster                                                           |
| unpickle             | 9.23 us                                                         | 9.68 us: 1.05x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.18x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.6 ms: 1.10x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.57 ms: 1.36x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 91.6 us: 5.22x faster                                                           |
| generators                 | 52.2 ms                                                         | 22.4 ms: 2.33x faster                                                           |
| logging_silent             | 119 ns                                                          | 60.6 ns: 1.97x faster                                                           |
| richards_super             | 58.7 ms                                                         | 32.8 ms: 1.79x faster                                                           |
| richards                   | 48.8 ms                                                         | 28.5 ms: 1.71x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 887 us: 1.68x faster                                                            |
| coroutines                 | 23.7 ms                                                         | 14.2 ms: 1.67x faster                                                           |
| comprehensions             | 22.1 us                                                         | 13.2 us: 1.67x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 62.2 ms: 1.64x faster                                                           |
| chaos                      | 84.4 ms                                                         | 51.4 ms: 1.64x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 24.5 us: 1.63x faster                                                           |
| raytrace                   | 327 ms                                                          | 201 ms: 1.63x faster                                                            |
| unpack_sequence            | 65.2 ns                                                         | 40.4 ns: 1.61x faster                                                           |
| scimark_sor                | 135 ms                                                          | 84.1 ms: 1.61x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.13 ms: 1.58x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.63 ms: 1.56x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 153 us: 1.51x faster                                                            |
| hexiom                     | 7.51 ms                                                         | 5.07 ms: 1.48x faster                                                           |
| nbody                      | 126 ms                                                          | 85.3 ms: 1.48x faster                                                           |
| crypto_pyaes               | 79.4 ms                                                         | 53.8 ms: 1.48x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 212 us: 1.46x faster                                                            |
| json_dumps                 | 9.80 ms                                                         | 6.75 ms: 1.45x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.61 sec: 1.44x faster                                                          |
| nqueens                    | 111 ms                                                          | 77.8 ms: 1.43x faster                                                           |
| regex_compile              | 148 ms                                                          | 103 ms: 1.43x faster                                                            |
| spectral_norm              | 122 ms                                                          | 85.7 ms: 1.42x faster                                                           |
| go                         | 147 ms                                                          | 104 ms: 1.41x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 50.1 ms: 1.41x faster                                                           |
| deepcopy                   | 381 us                                                          | 271 us: 1.40x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 106 ms: 1.40x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.22 sec: 1.39x faster                                                          |
| pyflate                    | 471 ms                                                          | 338 ms: 1.39x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.80 ms: 1.39x faster                                                           |
| logging_simple             | 10.8 us                                                         | 7.79 us: 1.39x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 596 ms: 1.37x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.34 us: 1.37x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.43 us: 1.36x faster                                                           |
| async_tree_none            | 343 ms                                                          | 252 ms: 1.36x faster                                                            |
| sympy_str                  | 283 ms                                                          | 208 ms: 1.36x faster                                                            |
| mako                       | 10.3 ms                                                         | 7.57 ms: 1.36x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 41.0 ms: 1.34x faster                                                           |
| float                      | 76.1 ms                                                         | 57.4 ms: 1.33x faster                                                           |
| scimark_fft                | 291 ms                                                          | 220 ms: 1.33x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.21 ms: 1.32x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 15.1 ms: 1.32x faster                                                           |
| fannkuch                   | 399 ms                                                          | 305 ms: 1.31x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 39.6 ms: 1.31x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 608 ms: 1.29x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 316 ms: 1.29x faster                                                            |
| sympy_expand               | 462 ms                                                          | 359 ms: 1.29x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 816 ms: 1.28x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.62 sec: 1.28x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 588 ms: 1.27x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 238 ms: 1.26x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 300 ms: 1.26x faster                                                            |
| async_tree_io              | 754 ms                                                          | 605 ms: 1.25x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 59.2 ms: 1.21x faster                                                           |
| tornado_http               | 118 ms                                                          | 101 ms: 1.18x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 77.3 ms: 1.18x faster                                                           |
| json                       | 4.78 ms                                                         | 4.06 ms: 1.18x faster                                                           |
| dask                       | 355 ms                                                          | 302 ms: 1.18x faster                                                            |
| 2to3                       | 282 ms                                                          | 241 ms: 1.17x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.84 us: 1.17x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.80 sec: 1.16x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 510 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 503 ms: 1.15x faster                                                            |
| unpickle_list              | 3.28 us                                                         | 2.94 us: 1.11x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.4 ms: 1.11x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.04 ms: 1.09x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| regex_dna                  | 122 ms                                                          | 116 ms: 1.05x faster                                                            |
| pickle                     | 7.99 us                                                         | 7.67 us: 1.04x faster                                                           |
| pidigits                   | 203 ms                                                          | 197 ms: 1.03x faster                                                            |
| json_loads                 | 20.0 us                                                         | 19.7 us: 1.02x faster                                                           |
| pickle_list                | 3.27 us                                                         | 3.22 us: 1.02x faster                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.4 sec: 1.02x slower                                                          |
| bench_mp_pool              | 70.9 ms                                                         | 72.5 ms: 1.02x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.87 ms: 1.03x slower                                                           |
| async_generators           | 260 ms                                                          | 268 ms: 1.03x slower                                                            |
| python_startup             | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 15.9 ms: 1.05x slower                                                           |
| unpickle                   | 9.23 us                                                         | 9.68 us: 1.05x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 655 us: 1.06x slower                                                            |
| pathlib                    | 79.9 ms                                                         | 87.6 ms: 1.10x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.6 ms: 1.10x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.82 ms: 1.10x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 202 ms: 1.79x slower                                                            |
| coverage                   | 58.0 ms                                                         | 474 ms: 8.17x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.26x faster                                                                    |

Benchmark hidden because not significant (2): pickle_dict, gc_traversal
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: unknown