
# Results vs. 3.11.0

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.04x faster \*
- HPT reliability: 78.56%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 300 ms: 1.05x slower                                            |
| chameleon      | 7.92 ms                                                      | 7.22 ms: 1.10x faster                                           |
| docutils       | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                          |
| Geometric mean | (ref)                                                        | 1.01x faster                                                    |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 438 ms: 1.18x faster                                            |
| async_tree_memoization     | 629 ms                                                       | 548 ms: 1.15x faster                                            |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                          |
| async_tree_memoization_tg  | 600 ms                                                       | 552 ms: 1.09x faster                                            |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 700 ms: 1.08x faster                                            |
| async_tree_none_tg         | 474 ms                                                       | 441 ms: 1.07x faster                                            |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                          |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 706 ms: 1.06x faster                                            |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                            |
| float          | 74.9 ms                                                      | 81.2 ms: 1.08x slower                                           |
| nbody          | 92.9 ms                                                      | 107 ms: 1.15x slower                                            |
| Geometric mean | (ref)                                                        | 1.09x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 145 ms: 1.08x faster                                            |
| regex_v8       | 24.4 ms                                                      | 25.2 ms: 1.03x slower                                           |
| regex_effbot   | 3.34 ms                                                      | 3.57 ms: 1.07x slower                                           |
| regex_dna      | 227 ms                                                       | 244 ms: 1.07x slower                                            |
| Geometric mean | (ref)                                                        | 1.02x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                           |
| json_loads           | 28.9 us                                                      | 25.1 us: 1.15x faster                                           |
| unpickle_pure_python | 238 us                                                       | 227 us: 1.05x faster                                            |
| pickle_pure_python   | 316 us                                                       | 306 us: 1.03x faster                                            |
| xml_etree_parse      | 155 ms                                                       | 150 ms: 1.03x faster                                            |
| xml_etree_iterparse  | 107 ms                                                       | 106 ms: 1.01x faster                                            |
| pickle_dict          | 32.3 us                                                      | 32.7 us: 1.01x slower                                           |
| tomli_loads          | 2.25 sec                                                     | 2.29 sec: 1.02x slower                                          |
| unpickle_list        | 4.60 us                                                      | 4.72 us: 1.03x slower                                           |
| xml_etree_process    | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                           |
| xml_etree_generate   | 79.7 ms                                                      | 84.9 ms: 1.07x slower                                           |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                           |
| pickle_list          | 3.94 us                                                      | 4.38 us: 1.11x slower                                           |
| unpickle             | 13.3 us                                                      | 15.0 us: 1.13x slower                                           |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                           |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                           |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 11.7 ms: 1.06x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 119 us: 4.49x faster                                            |
| asyncio_tcp                | 747 ms                                                       | 373 ms: 2.00x faster                                            |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.95x faster                                          |
| generators                 | 54.6 ms                                                      | 33.5 ms: 1.63x faster                                           |
| comprehensions             | 25.1 us                                                      | 19.4 us: 1.29x faster                                           |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                           |
| coroutines                 | 27.8 ms                                                      | 22.5 ms: 1.23x faster                                           |
| gc_traversal               | 4.15 ms                                                      | 3.43 ms: 1.21x faster                                           |
| async_tree_none            | 518 ms                                                       | 438 ms: 1.18x faster                                            |
| sympy_sum                  | 186 ms                                                       | 158 ms: 1.17x faster                                            |
| json_loads                 | 28.9 us                                                      | 25.1 us: 1.15x faster                                           |
| scimark_lu                 | 114 ms                                                       | 99.3 ms: 1.15x faster                                           |
| async_tree_memoization     | 629 ms                                                       | 548 ms: 1.15x faster                                            |
| sympy_str                  | 337 ms                                                       | 299 ms: 1.13x faster                                            |
| richards_super             | 63.6 ms                                                      | 56.5 ms: 1.13x faster                                           |
| unpack_sequence            | 45.7 ns                                                      | 41.2 ns: 1.11x faster                                           |
| logging_simple             | 7.24 us                                                      | 6.55 us: 1.11x faster                                           |
| raytrace                   | 309 ms                                                       | 280 ms: 1.11x faster                                            |
| chameleon                  | 7.92 ms                                                      | 7.22 ms: 1.10x faster                                           |
| sympy_expand               | 553 ms                                                       | 506 ms: 1.09x faster                                            |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                          |
| async_tree_memoization_tg  | 600 ms                                                       | 552 ms: 1.09x faster                                            |
| sympy_integrate            | 25.8 ms                                                      | 23.8 ms: 1.08x faster                                           |
| mdp                        | 2.77 sec                                                     | 2.56 sec: 1.08x faster                                          |
| regex_compile              | 156 ms                                                       | 145 ms: 1.08x faster                                            |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 700 ms: 1.08x faster                                            |
| sqlglot_parse              | 1.51 ms                                                      | 1.41 ms: 1.08x faster                                           |
| async_tree_none_tg         | 474 ms                                                       | 441 ms: 1.07x faster                                            |
| logging_format             | 7.71 us                                                      | 7.18 us: 1.07x faster                                           |
| chaos                      | 74.9 ms                                                      | 69.8 ms: 1.07x faster                                           |
| nqueens                    | 103 ms                                                       | 95.7 ms: 1.07x faster                                           |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                          |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 706 ms: 1.06x faster                                            |
| deepcopy                   | 391 us                                                       | 370 us: 1.06x faster                                            |
| json                       | 5.58 ms                                                      | 5.29 ms: 1.05x faster                                           |
| deltablue                  | 3.97 ms                                                      | 3.78 ms: 1.05x faster                                           |
| sqlglot_transpile          | 1.91 ms                                                      | 1.82 ms: 1.05x faster                                           |
| unpickle_pure_python       | 238 us                                                       | 227 us: 1.05x faster                                            |
| crypto_pyaes               | 83.3 ms                                                      | 79.9 ms: 1.04x faster                                           |
| create_gc_cycles           | 1.58 ms                                                      | 1.52 ms: 1.04x faster                                           |
| logging_silent             | 100 ns                                                       | 96.7 ns: 1.04x faster                                           |
| sqlglot_normalize          | 122 ms                                                       | 118 ms: 1.03x faster                                            |
| pickle_pure_python         | 316 us                                                       | 306 us: 1.03x faster                                            |
| xml_etree_parse            | 155 ms                                                       | 150 ms: 1.03x faster                                            |
| deepcopy_memo              | 37.5 us                                                      | 36.6 us: 1.03x faster                                           |
| deepcopy_reduce            | 3.40 us                                                      | 3.36 us: 1.01x faster                                           |
| fannkuch                   | 416 ms                                                       | 412 ms: 1.01x faster                                            |
| xml_etree_iterparse        | 107 ms                                                       | 106 ms: 1.01x faster                                            |
| meteor_contest             | 131 ms                                                       | 130 ms: 1.00x faster                                            |
| docutils                   | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                          |
| pickle_dict                | 32.3 us                                                      | 32.7 us: 1.01x slower                                           |
| richards                   | 49.7 ms                                                      | 50.3 ms: 1.01x slower                                           |
| tomli_loads                | 2.25 sec                                                     | 2.29 sec: 1.02x slower                                          |
| unpickle_list              | 4.60 us                                                      | 4.72 us: 1.03x slower                                           |
| sqlglot_optimize           | 59.0 ms                                                      | 60.6 ms: 1.03x slower                                           |
| dulwich_log                | 67.4 ms                                                      | 69.4 ms: 1.03x slower                                           |
| regex_v8                   | 24.4 ms                                                      | 25.2 ms: 1.03x slower                                           |
| xml_etree_process          | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                           |
| pprint_pformat             | 1.67 sec                                                     | 1.74 sec: 1.04x slower                                          |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                            |
| 2to3                       | 287 ms                                                       | 300 ms: 1.05x slower                                            |
| pprint_safe_repr           | 805 ms                                                       | 848 ms: 1.05x slower                                            |
| go                         | 158 ms                                                       | 166 ms: 1.05x slower                                            |
| mako                       | 11.0 ms                                                      | 11.7 ms: 1.06x slower                                           |
| xml_etree_generate         | 79.7 ms                                                      | 84.9 ms: 1.07x slower                                           |
| regex_effbot               | 3.34 ms                                                      | 3.57 ms: 1.07x slower                                           |
| regex_dna                  | 227 ms                                                       | 244 ms: 1.07x slower                                            |
| pickle                     | 9.89 us                                                      | 10.6 us: 1.07x slower                                           |
| float                      | 74.9 ms                                                      | 81.2 ms: 1.08x slower                                           |
| sqlite_synth               | 2.52 us                                                      | 2.74 us: 1.09x slower                                           |
| scimark_monte_carlo        | 69.8 ms                                                      | 76.6 ms: 1.10x slower                                           |
| hexiom                     | 6.98 ms                                                      | 7.66 ms: 1.10x slower                                           |
| pickle_list                | 3.94 us                                                      | 4.38 us: 1.11x slower                                           |
| unpickle                   | 13.3 us                                                      | 15.0 us: 1.13x slower                                           |
| async_generators           | 322 ms                                                       | 363 ms: 1.13x slower                                            |
| nbody                      | 92.9 ms                                                      | 107 ms: 1.15x slower                                            |
| mypy2                      | 762 ms                                                       | 889 ms: 1.17x slower                                            |
| coverage                   | 66.1 ms                                                      | 77.6 ms: 1.17x slower                                           |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                           |
| spectral_norm              | 95.1 ms                                                      | 113 ms: 1.19x slower                                            |
| telco                      | 6.81 ms                                                      | 8.17 ms: 1.20x slower                                           |
| pyflate                    | 449 ms                                                       | 546 ms: 1.22x slower                                            |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 5.01 ms: 1.23x slower                                           |
| scimark_fft                | 281 ms                                                       | 348 ms: 1.24x slower                                            |
| scimark_sor                | 110 ms                                                       | 141 ms: 1.29x slower                                            |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                           |
| Geometric mean             | (ref)                                                        | 1.04x faster                                                    |

Benchmark hidden because not significant (7): bench_thread_pool, dask, tornado_http, pathlib, asyncio_websockets, pycparser, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 78.56% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x