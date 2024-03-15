
# Results vs. 3.10.4

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.26x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 300 ms: 1.17x faster                                            |
| chameleon      | 9.44 ms                                                      | 7.22 ms: 1.31x faster                                           |
| docutils       | 3.41 sec                                                     | 2.87 sec: 1.19x faster                                          |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                            |
| Geometric mean | (ref)                                                        | 1.23x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 438 ms: 1.58x faster                                            |
| async_tree_memoization  | 819 ms                                                       | 548 ms: 1.49x faster                                            |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                          |
| async_tree_cpu_io_mixed | 936 ms                                                       | 700 ms: 1.34x faster                                            |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 111 ms                                                       | 81.2 ms: 1.37x faster                                           |
| nbody          | 134 ms                                                       | 107 ms: 1.25x faster                                            |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                            |
| Geometric mean | (ref)                                                        | 1.21x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 145 ms: 1.31x faster                                            |
| regex_v8       | 27.2 ms                                                      | 25.2 ms: 1.08x faster                                           |
| regex_dna      | 261 ms                                                       | 244 ms: 1.07x faster                                            |
| regex_effbot   | 3.09 ms                                                      | 3.57 ms: 1.16x slower                                           |
| Geometric mean | (ref)                                                        | 1.07x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 306 us: 1.49x faster                                            |
| unpickle_pure_python | 312 us                                                       | 227 us: 1.37x faster                                            |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                           |
| xml_etree_process    | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                           |
| tomli_loads          | 2.92 sec                                                     | 2.29 sec: 1.27x faster                                          |
| json_loads           | 30.3 us                                                      | 25.1 us: 1.21x faster                                           |
| xml_etree_generate   | 92.3 ms                                                      | 84.9 ms: 1.09x faster                                           |
| xml_etree_parse      | 160 ms                                                       | 150 ms: 1.07x faster                                            |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.04x faster                                            |
| unpickle_list        | 4.65 us                                                      | 4.72 us: 1.01x slower                                           |
| pickle_list          | 4.12 us                                                      | 4.38 us: 1.06x slower                                           |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                           |
| pickle_dict          | 29.5 us                                                      | 32.7 us: 1.11x slower                                           |
| unpickle             | 13.5 us                                                      | 15.0 us: 1.11x slower                                           |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                           |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                           |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 11.7 ms: 1.26x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 119 us: 4.52x faster                                            |
| asyncio_tcp              | 779 ms                                                       | 373 ms: 2.09x faster                                            |
| deltablue                | 7.50 ms                                                      | 3.78 ms: 1.98x faster                                           |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                          |
| raytrace                 | 489 ms                                                       | 280 ms: 1.75x faster                                            |
| logging_silent           | 167 ns                                                       | 96.7 ns: 1.73x faster                                           |
| generators               | 57.3 ms                                                      | 33.5 ms: 1.71x faster                                           |
| scimark_lu               | 167 ms                                                       | 99.3 ms: 1.68x faster                                           |
| richards_super           | 90.6 ms                                                      | 56.5 ms: 1.60x faster                                           |
| sqlglot_parse            | 2.24 ms                                                      | 1.41 ms: 1.59x faster                                           |
| async_tree_none          | 692 ms                                                       | 438 ms: 1.58x faster                                            |
| go                       | 262 ms                                                       | 166 ms: 1.57x faster                                            |
| chaos                    | 109 ms                                                       | 69.8 ms: 1.56x faster                                           |
| async_tree_memoization   | 819 ms                                                       | 548 ms: 1.49x faster                                            |
| crypto_pyaes             | 119 ms                                                       | 79.9 ms: 1.49x faster                                           |
| richards                 | 75.1 ms                                                      | 50.3 ms: 1.49x faster                                           |
| pickle_pure_python       | 455 us                                                       | 306 us: 1.49x faster                                            |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                          |
| sqlglot_transpile        | 2.68 ms                                                      | 1.82 ms: 1.47x faster                                           |
| unpack_sequence          | 59.9 ns                                                      | 41.2 ns: 1.46x faster                                           |
| scimark_monte_carlo      | 107 ms                                                       | 76.6 ms: 1.40x faster                                           |
| comprehensions           | 26.7 us                                                      | 19.4 us: 1.37x faster                                           |
| unpickle_pure_python     | 312 us                                                       | 227 us: 1.37x faster                                            |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                           |
| float                    | 111 ms                                                       | 81.2 ms: 1.37x faster                                           |
| deepcopy_memo            | 49.8 us                                                      | 36.6 us: 1.36x faster                                           |
| logging_simple           | 8.88 us                                                      | 6.55 us: 1.35x faster                                           |
| coroutines               | 30.3 ms                                                      | 22.5 ms: 1.35x faster                                           |
| logging_format           | 9.64 us                                                      | 7.18 us: 1.34x faster                                           |
| pyflate                  | 733 ms                                                       | 546 ms: 1.34x faster                                            |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 700 ms: 1.34x faster                                            |
| bench_mp_pool            | 6.37 ms                                                      | 4.77 ms: 1.34x faster                                           |
| regex_compile            | 190 ms                                                       | 145 ms: 1.31x faster                                            |
| chameleon                | 9.44 ms                                                      | 7.22 ms: 1.31x faster                                           |
| xml_etree_process        | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                           |
| pycparser                | 1.67 sec                                                     | 1.31 sec: 1.28x faster                                          |
| scimark_sor              | 180 ms                                                       | 141 ms: 1.28x faster                                            |
| tomli_loads              | 2.92 sec                                                     | 2.29 sec: 1.27x faster                                          |
| deepcopy                 | 468 us                                                       | 370 us: 1.26x faster                                            |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                            |
| mako                     | 14.7 ms                                                      | 11.7 ms: 1.26x faster                                           |
| nbody                    | 134 ms                                                       | 107 ms: 1.25x faster                                            |
| pprint_pformat           | 2.15 sec                                                     | 1.74 sec: 1.24x faster                                          |
| pprint_safe_repr         | 1.05 sec                                                     | 848 ms: 1.24x faster                                            |
| hexiom                   | 9.42 ms                                                      | 7.66 ms: 1.23x faster                                           |
| spectral_norm            | 139 ms                                                       | 113 ms: 1.23x faster                                            |
| sqlglot_normalize        | 144 ms                                                       | 118 ms: 1.22x faster                                            |
| sympy_sum                | 193 ms                                                       | 158 ms: 1.22x faster                                            |
| json_loads               | 30.3 us                                                      | 25.1 us: 1.21x faster                                           |
| sympy_str                | 360 ms                                                       | 299 ms: 1.20x faster                                            |
| nqueens                  | 115 ms                                                       | 95.7 ms: 1.20x faster                                           |
| deepcopy_reduce          | 4.01 us                                                      | 3.36 us: 1.19x faster                                           |
| docutils                 | 3.41 sec                                                     | 2.87 sec: 1.19x faster                                          |
| sympy_expand             | 600 ms                                                       | 506 ms: 1.19x faster                                            |
| sympy_integrate          | 28.2 ms                                                      | 23.8 ms: 1.18x faster                                           |
| mdp                      | 3.01 sec                                                     | 2.56 sec: 1.17x faster                                          |
| fannkuch                 | 483 ms                                                       | 412 ms: 1.17x faster                                            |
| dulwich_log              | 81.1 ms                                                      | 69.4 ms: 1.17x faster                                           |
| 2to3                     | 350 ms                                                       | 300 ms: 1.17x faster                                            |
| create_gc_cycles         | 1.76 ms                                                      | 1.52 ms: 1.16x faster                                           |
| async_generators         | 421 ms                                                       | 363 ms: 1.16x faster                                            |
| sqlglot_optimize         | 70.1 ms                                                      | 60.6 ms: 1.16x faster                                           |
| bench_thread_pool        | 1.14 ms                                                      | 986 us: 1.16x faster                                            |
| dask                     | 472 ms                                                       | 409 ms: 1.15x faster                                            |
| pathlib                  | 21.4 ms                                                      | 18.9 ms: 1.13x faster                                           |
| json                     | 5.86 ms                                                      | 5.29 ms: 1.11x faster                                           |
| sqlite_synth             | 2.99 us                                                      | 2.74 us: 1.09x faster                                           |
| xml_etree_generate       | 92.3 ms                                                      | 84.9 ms: 1.09x faster                                           |
| regex_v8                 | 27.2 ms                                                      | 25.2 ms: 1.08x faster                                           |
| regex_dna                | 261 ms                                                       | 244 ms: 1.07x faster                                            |
| xml_etree_parse          | 160 ms                                                       | 150 ms: 1.07x faster                                            |
| meteor_contest           | 138 ms                                                       | 130 ms: 1.06x faster                                            |
| xml_etree_iterparse      | 110 ms                                                       | 106 ms: 1.04x faster                                            |
| scimark_fft              | 361 ms                                                       | 348 ms: 1.04x faster                                            |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                            |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.01 ms: 1.01x faster                                           |
| unpickle_list            | 4.65 us                                                      | 4.72 us: 1.01x slower                                           |
| pickle_list              | 4.12 us                                                      | 4.38 us: 1.06x slower                                           |
| pickle                   | 9.89 us                                                      | 10.6 us: 1.07x slower                                           |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                           |
| pickle_dict              | 29.5 us                                                      | 32.7 us: 1.11x slower                                           |
| unpickle                 | 13.5 us                                                      | 15.0 us: 1.11x slower                                           |
| telco                    | 7.23 ms                                                      | 8.17 ms: 1.13x slower                                           |
| regex_effbot             | 3.09 ms                                                      | 3.57 ms: 1.16x slower                                           |
| coverage                 | 63.3 ms                                                      | 77.6 ms: 1.23x slower                                           |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                           |
| Geometric mean           | (ref)                                                        | 1.26x faster                                                    |

Benchmark hidden because not significant (3): mypy2, asyncio_websockets, gc_traversal
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-aaf8974-JIT/bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.11x