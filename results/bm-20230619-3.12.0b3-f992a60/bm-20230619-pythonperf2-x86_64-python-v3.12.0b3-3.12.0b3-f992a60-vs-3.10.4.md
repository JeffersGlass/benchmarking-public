
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b3
- machine: linux-x86_64
- commit hash: f992a60
- commit date: 2023-06-19
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 283 ms: 1.24x faster                                             |
| docutils       | 3.41 sec                                                     | 2.87 sec: 1.19x faster                                           |
| tornado_http   | 157 ms                                                       | 118 ms: 1.33x faster                                             |
| Geometric mean | (ref)                                                        | 1.25x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                           |
| async_tree_none         | 692 ms                                                       | 457 ms: 1.51x faster                                             |
| async_tree_memoization  | 819 ms                                                       | 551 ms: 1.49x faster                                             |
| async_tree_cpu_io_mixed | 936 ms                                                       | 704 ms: 1.33x faster                                             |
| Geometric mean          | (ref)                                                        | 1.46x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 84.2 ms: 1.59x faster                                            |
| float          | 111 ms                                                       | 78.8 ms: 1.41x faster                                            |
| pidigits       | 271 ms                                                       | 260 ms: 1.04x faster                                             |
| Geometric mean | (ref)                                                        | 1.33x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 144 ms: 1.32x faster                                             |
| regex_v8       | 27.2 ms                                                      | 23.9 ms: 1.14x faster                                            |
| regex_dna      | 261 ms                                                       | 238 ms: 1.10x faster                                             |
| regex_effbot   | 3.09 ms                                                      | 3.48 ms: 1.13x slower                                            |
| Geometric mean | (ref)                                                        | 1.10x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 209 us: 1.49x faster                                             |
| json_dumps           | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                            |
| pickle_pure_python   | 455 us                                                       | 326 us: 1.39x faster                                             |
| tomli_loads          | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                           |
| xml_etree_process    | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                            |
| json_loads           | 30.3 us                                                      | 24.7 us: 1.23x faster                                            |
| xml_etree_generate   | 92.3 ms                                                      | 85.3 ms: 1.08x faster                                            |
| xml_etree_parse      | 160 ms                                                       | 150 ms: 1.07x faster                                             |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.04x faster                                             |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                            |
| pickle_list          | 4.12 us                                                      | 4.43 us: 1.08x slower                                            |
| unpickle             | 13.5 us                                                      | 14.6 us: 1.08x slower                                            |
| pickle_dict          | 29.5 us                                                      | 33.6 us: 1.14x slower                                            |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                     |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.4 ms: 1.01x faster                                            |
| python_startup_no_site | 7.33 ms                                                      | 8.43 ms: 1.15x slower                                            |
| Geometric mean         | (ref)                                                        | 1.07x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.0 ms: 1.46x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 152 us: 3.53x faster                                             |
| deltablue                | 7.50 ms                                                      | 3.21 ms: 2.33x faster                                            |
| asyncio_tcp              | 779 ms                                                       | 377 ms: 2.07x faster                                             |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.56 sec: 1.98x faster                                           |
| logging_silent           | 167 ns                                                       | 91.8 ns: 1.82x faster                                            |
| go                       | 262 ms                                                       | 145 ms: 1.80x faster                                             |
| richards_super           | 90.6 ms                                                      | 50.8 ms: 1.79x faster                                            |
| scimark_lu               | 167 ms                                                       | 96.7 ms: 1.72x faster                                            |
| chaos                    | 109 ms                                                       | 63.4 ms: 1.71x faster                                            |
| scimark_sor              | 180 ms                                                       | 107 ms: 1.68x faster                                             |
| richards                 | 75.1 ms                                                      | 44.7 ms: 1.68x faster                                            |
| pyflate                  | 733 ms                                                       | 439 ms: 1.67x faster                                             |
| raytrace                 | 489 ms                                                       | 300 ms: 1.63x faster                                             |
| hexiom                   | 9.42 ms                                                      | 5.79 ms: 1.63x faster                                            |
| sqlglot_parse            | 2.24 ms                                                      | 1.39 ms: 1.61x faster                                            |
| nbody                    | 134 ms                                                       | 84.2 ms: 1.59x faster                                            |
| scimark_monte_carlo      | 107 ms                                                       | 67.8 ms: 1.59x faster                                            |
| generators               | 57.3 ms                                                      | 36.7 ms: 1.56x faster                                            |
| async_tree_io            | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                           |
| async_tree_none          | 692 ms                                                       | 457 ms: 1.51x faster                                             |
| unpickle_pure_python     | 312 us                                                       | 209 us: 1.49x faster                                             |
| sqlglot_transpile        | 2.68 ms                                                      | 1.80 ms: 1.49x faster                                            |
| spectral_norm            | 139 ms                                                       | 93.4 ms: 1.49x faster                                            |
| async_tree_memoization   | 819 ms                                                       | 551 ms: 1.49x faster                                             |
| crypto_pyaes             | 119 ms                                                       | 80.9 ms: 1.47x faster                                            |
| mako                     | 14.7 ms                                                      | 10.0 ms: 1.46x faster                                            |
| float                    | 111 ms                                                       | 78.8 ms: 1.41x faster                                            |
| fannkuch                 | 483 ms                                                       | 343 ms: 1.41x faster                                             |
| json_dumps               | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                            |
| pickle_pure_python       | 455 us                                                       | 326 us: 1.39x faster                                             |
| logging_simple           | 8.88 us                                                      | 6.49 us: 1.37x faster                                            |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                            |
| logging_format           | 9.64 us                                                      | 7.13 us: 1.35x faster                                            |
| tomli_loads              | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                           |
| deepcopy_memo            | 49.8 us                                                      | 37.4 us: 1.33x faster                                            |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 704 ms: 1.33x faster                                             |
| tornado_http             | 157 ms                                                       | 118 ms: 1.33x faster                                             |
| pprint_pformat           | 2.15 sec                                                     | 1.63 sec: 1.32x faster                                           |
| regex_compile            | 190 ms                                                       | 144 ms: 1.32x faster                                             |
| pprint_safe_repr         | 1.05 sec                                                     | 799 ms: 1.31x faster                                             |
| pycparser                | 1.67 sec                                                     | 1.27 sec: 1.31x faster                                           |
| xml_etree_process        | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                            |
| nqueens                  | 115 ms                                                       | 90.2 ms: 1.27x faster                                            |
| bench_mp_pool            | 6.37 ms                                                      | 5.05 ms: 1.26x faster                                            |
| deepcopy                 | 468 us                                                       | 376 us: 1.24x faster                                             |
| 2to3                     | 350 ms                                                       | 283 ms: 1.24x faster                                             |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                             |
| comprehensions           | 26.7 us                                                      | 21.7 us: 1.23x faster                                            |
| dulwich_log              | 81.1 ms                                                      | 66.1 ms: 1.23x faster                                            |
| json_loads               | 30.3 us                                                      | 24.7 us: 1.23x faster                                            |
| sqlglot_optimize         | 70.1 ms                                                      | 57.4 ms: 1.22x faster                                            |
| unpack_sequence          | 59.9 ns                                                      | 49.4 ns: 1.21x faster                                            |
| mdp                      | 3.01 sec                                                     | 2.49 sec: 1.21x faster                                           |
| bench_thread_pool        | 1.14 ms                                                      | 953 us: 1.20x faster                                             |
| docutils                 | 3.41 sec                                                     | 2.87 sec: 1.19x faster                                           |
| scimark_fft              | 361 ms                                                       | 304 ms: 1.19x faster                                             |
| deepcopy_reduce          | 4.01 us                                                      | 3.41 us: 1.18x faster                                            |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.43 ms: 1.15x faster                                            |
| regex_v8                 | 27.2 ms                                                      | 23.9 ms: 1.14x faster                                            |
| json                     | 5.86 ms                                                      | 5.18 ms: 1.13x faster                                            |
| pathlib                  | 21.4 ms                                                      | 19.2 ms: 1.11x faster                                            |
| meteor_contest           | 138 ms                                                       | 125 ms: 1.11x faster                                             |
| async_generators         | 421 ms                                                       | 382 ms: 1.10x faster                                             |
| sqlite_synth             | 2.99 us                                                      | 2.72 us: 1.10x faster                                            |
| regex_dna                | 261 ms                                                       | 238 ms: 1.10x faster                                             |
| xml_etree_generate       | 92.3 ms                                                      | 85.3 ms: 1.08x faster                                            |
| create_gc_cycles         | 1.76 ms                                                      | 1.64 ms: 1.08x faster                                            |
| xml_etree_parse          | 160 ms                                                       | 150 ms: 1.07x faster                                             |
| xml_etree_iterparse      | 110 ms                                                       | 106 ms: 1.04x faster                                             |
| pidigits                 | 271 ms                                                       | 260 ms: 1.04x faster                                             |
| telco                    | 7.23 ms                                                      | 7.07 ms: 1.02x faster                                            |
| python_startup           | 11.5 ms                                                      | 11.4 ms: 1.01x faster                                            |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.04x slower                                            |
| pickle_list              | 4.12 us                                                      | 4.43 us: 1.08x slower                                            |
| unpickle                 | 13.5 us                                                      | 14.6 us: 1.08x slower                                            |
| regex_effbot             | 3.09 ms                                                      | 3.48 ms: 1.13x slower                                            |
| pickle_dict              | 29.5 us                                                      | 33.6 us: 1.14x slower                                            |
| python_startup_no_site   | 7.33 ms                                                      | 8.43 ms: 1.15x slower                                            |
| dask                     | 472 ms                                                       | 562 ms: 1.19x slower                                             |
| gc_traversal             | 3.42 ms                                                      | 4.06 ms: 1.19x slower                                            |
| coverage                 | 63.3 ms                                                      | 89.0 ms: 1.41x slower                                            |
| Geometric mean           | (ref)                                                        | 1.30x faster                                                     |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (18) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.28x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.26x