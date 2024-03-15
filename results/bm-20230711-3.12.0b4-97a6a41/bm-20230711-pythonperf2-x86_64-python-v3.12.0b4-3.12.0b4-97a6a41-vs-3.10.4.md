
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b4
- machine: linux-x86_64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 285 ms: 1.23x faster                                             |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                           |
| tornado_http   | 157 ms                                                       | 120 ms: 1.31x faster                                             |
| Geometric mean | (ref)                                                        | 1.24x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                           |
| async_tree_none         | 692 ms                                                       | 458 ms: 1.51x faster                                             |
| async_tree_memoization  | 819 ms                                                       | 551 ms: 1.49x faster                                             |
| async_tree_cpu_io_mixed | 936 ms                                                       | 700 ms: 1.34x faster                                             |
| Geometric mean          | (ref)                                                        | 1.46x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 85.5 ms: 1.57x faster                                            |
| float          | 111 ms                                                       | 77.8 ms: 1.43x faster                                            |
| pidigits       | 271 ms                                                       | 260 ms: 1.04x faster                                             |
| Geometric mean | (ref)                                                        | 1.33x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 144 ms: 1.32x faster                                             |
| regex_v8       | 27.2 ms                                                      | 23.7 ms: 1.14x faster                                            |
| regex_dna      | 261 ms                                                       | 236 ms: 1.11x faster                                             |
| regex_effbot   | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                            |
| Geometric mean | (ref)                                                        | 1.10x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 207 us: 1.50x faster                                             |
| pickle_pure_python   | 455 us                                                       | 319 us: 1.43x faster                                             |
| json_dumps           | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                            |
| tomli_loads          | 2.92 sec                                                     | 2.18 sec: 1.34x faster                                           |
| xml_etree_process    | 75.9 ms                                                      | 58.2 ms: 1.31x faster                                            |
| json_loads           | 30.3 us                                                      | 25.1 us: 1.21x faster                                            |
| xml_etree_generate   | 92.3 ms                                                      | 85.2 ms: 1.08x faster                                            |
| xml_etree_parse      | 160 ms                                                       | 151 ms: 1.06x faster                                             |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.04x faster                                             |
| unpickle_list        | 4.65 us                                                      | 4.74 us: 1.02x slower                                            |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                            |
| pickle_list          | 4.12 us                                                      | 4.44 us: 1.08x slower                                            |
| unpickle             | 13.5 us                                                      | 14.6 us: 1.09x slower                                            |
| pickle_dict          | 29.5 us                                                      | 33.2 us: 1.12x slower                                            |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup_no_site | 7.33 ms                                                      | 8.52 ms: 1.16x slower                                            |
| Geometric mean         | (ref)                                                        | 1.08x slower                                                     |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 9.88 ms: 1.49x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 151 us: 3.55x faster                                             |
| deltablue                | 7.50 ms                                                      | 3.19 ms: 2.35x faster                                            |
| asyncio_tcp              | 779 ms                                                       | 383 ms: 2.03x faster                                             |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                           |
| go                       | 262 ms                                                       | 145 ms: 1.80x faster                                             |
| logging_silent           | 167 ns                                                       | 93.5 ns: 1.79x faster                                            |
| richards_super           | 90.6 ms                                                      | 51.0 ms: 1.78x faster                                            |
| chaos                    | 109 ms                                                       | 62.5 ms: 1.74x faster                                            |
| scimark_lu               | 167 ms                                                       | 96.5 ms: 1.73x faster                                            |
| richards                 | 75.1 ms                                                      | 44.4 ms: 1.69x faster                                            |
| scimark_sor              | 180 ms                                                       | 107 ms: 1.68x faster                                             |
| raytrace                 | 489 ms                                                       | 300 ms: 1.63x faster                                             |
| hexiom                   | 9.42 ms                                                      | 5.84 ms: 1.61x faster                                            |
| pyflate                  | 733 ms                                                       | 457 ms: 1.60x faster                                             |
| sqlglot_parse            | 2.24 ms                                                      | 1.40 ms: 1.60x faster                                            |
| generators               | 57.3 ms                                                      | 36.2 ms: 1.58x faster                                            |
| nbody                    | 134 ms                                                       | 85.5 ms: 1.57x faster                                            |
| scimark_monte_carlo      | 107 ms                                                       | 69.3 ms: 1.55x faster                                            |
| spectral_norm            | 139 ms                                                       | 91.5 ms: 1.52x faster                                            |
| async_tree_io            | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                           |
| async_tree_none          | 692 ms                                                       | 458 ms: 1.51x faster                                             |
| unpickle_pure_python     | 312 us                                                       | 207 us: 1.50x faster                                             |
| sqlglot_transpile        | 2.68 ms                                                      | 1.79 ms: 1.50x faster                                            |
| mako                     | 14.7 ms                                                      | 9.88 ms: 1.49x faster                                            |
| async_tree_memoization   | 819 ms                                                       | 551 ms: 1.49x faster                                             |
| crypto_pyaes             | 119 ms                                                       | 81.1 ms: 1.47x faster                                            |
| float                    | 111 ms                                                       | 77.8 ms: 1.43x faster                                            |
| pickle_pure_python       | 455 us                                                       | 319 us: 1.43x faster                                             |
| json_dumps               | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                            |
| fannkuch                 | 483 ms                                                       | 342 ms: 1.41x faster                                             |
| deepcopy_memo            | 49.8 us                                                      | 36.2 us: 1.37x faster                                            |
| pycparser                | 1.67 sec                                                     | 1.23 sec: 1.36x faster                                           |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 700 ms: 1.34x faster                                             |
| tomli_loads              | 2.92 sec                                                     | 2.18 sec: 1.34x faster                                           |
| logging_simple           | 8.88 us                                                      | 6.64 us: 1.34x faster                                            |
| pprint_pformat           | 2.15 sec                                                     | 1.62 sec: 1.33x faster                                           |
| pprint_safe_repr         | 1.05 sec                                                     | 789 ms: 1.33x faster                                             |
| regex_compile            | 190 ms                                                       | 144 ms: 1.32x faster                                             |
| logging_format           | 9.64 us                                                      | 7.31 us: 1.32x faster                                            |
| tornado_http             | 157 ms                                                       | 120 ms: 1.31x faster                                             |
| xml_etree_process        | 75.9 ms                                                      | 58.2 ms: 1.31x faster                                            |
| nqueens                  | 115 ms                                                       | 89.7 ms: 1.28x faster                                            |
| coroutines               | 30.3 ms                                                      | 23.7 ms: 1.28x faster                                            |
| deepcopy                 | 468 us                                                       | 372 us: 1.26x faster                                             |
| sqlglot_normalize        | 144 ms                                                       | 115 ms: 1.25x faster                                             |
| 2to3                     | 350 ms                                                       | 285 ms: 1.23x faster                                             |
| dulwich_log              | 81.1 ms                                                      | 66.3 ms: 1.22x faster                                            |
| sqlglot_optimize         | 70.1 ms                                                      | 57.4 ms: 1.22x faster                                            |
| comprehensions           | 26.7 us                                                      | 21.9 us: 1.22x faster                                            |
| bench_thread_pool        | 1.14 ms                                                      | 942 us: 1.21x faster                                             |
| json_loads               | 30.3 us                                                      | 25.1 us: 1.21x faster                                            |
| scimark_fft              | 361 ms                                                       | 302 ms: 1.20x faster                                             |
| mdp                      | 3.01 sec                                                     | 2.51 sec: 1.20x faster                                           |
| unpack_sequence          | 59.9 ns                                                      | 50.2 ns: 1.19x faster                                            |
| deepcopy_reduce          | 4.01 us                                                      | 3.38 us: 1.19x faster                                            |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                           |
| bench_mp_pool            | 6.37 ms                                                      | 5.44 ms: 1.17x faster                                            |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.36 ms: 1.16x faster                                            |
| regex_v8                 | 27.2 ms                                                      | 23.7 ms: 1.14x faster                                            |
| json                     | 5.86 ms                                                      | 5.19 ms: 1.13x faster                                            |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.13x faster                                            |
| regex_dna                | 261 ms                                                       | 236 ms: 1.11x faster                                             |
| sqlite_synth             | 2.99 us                                                      | 2.75 us: 1.09x faster                                            |
| meteor_contest           | 138 ms                                                       | 127 ms: 1.09x faster                                             |
| xml_etree_generate       | 92.3 ms                                                      | 85.2 ms: 1.08x faster                                            |
| async_generators         | 421 ms                                                       | 390 ms: 1.08x faster                                             |
| create_gc_cycles         | 1.76 ms                                                      | 1.65 ms: 1.07x faster                                            |
| xml_etree_parse          | 160 ms                                                       | 151 ms: 1.06x faster                                             |
| pidigits                 | 271 ms                                                       | 260 ms: 1.04x faster                                             |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.04x faster                                             |
| telco                    | 7.23 ms                                                      | 7.13 ms: 1.01x faster                                            |
| unpickle_list            | 4.65 us                                                      | 4.74 us: 1.02x slower                                            |
| gc_traversal             | 3.42 ms                                                      | 3.52 ms: 1.03x slower                                            |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                            |
| pickle_list              | 4.12 us                                                      | 4.44 us: 1.08x slower                                            |
| unpickle                 | 13.5 us                                                      | 14.6 us: 1.09x slower                                            |
| pickle_dict              | 29.5 us                                                      | 33.2 us: 1.12x slower                                            |
| regex_effbot             | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                            |
| python_startup_no_site   | 7.33 ms                                                      | 8.52 ms: 1.16x slower                                            |
| dask                     | 472 ms                                                       | 558 ms: 1.18x slower                                             |
| coverage                 | 63.3 ms                                                      | 91.3 ms: 1.44x slower                                            |
| Geometric mean           | (ref)                                                        | 1.30x faster                                                     |

Benchmark hidden because not significant (1): python_startup
Ignored benchmarks (18) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.27x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.26x