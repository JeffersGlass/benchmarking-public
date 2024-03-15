
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b1
- machine: linux-x86_64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 284 ms: 1.23x faster                                             |
| docutils       | 3.41 sec                                                     | 2.87 sec: 1.19x faster                                           |
| tornado_http   | 157 ms                                                       | 115 ms: 1.36x faster                                             |
| Geometric mean | (ref)                                                        | 1.26x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.05 sec: 1.53x faster                                           |
| async_tree_none         | 692 ms                                                       | 453 ms: 1.53x faster                                             |
| async_tree_memoization  | 819 ms                                                       | 544 ms: 1.51x faster                                             |
| async_tree_cpu_io_mixed | 936 ms                                                       | 696 ms: 1.35x faster                                             |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 84.7 ms: 1.58x faster                                            |
| float          | 111 ms                                                       | 78.6 ms: 1.41x faster                                            |
| pidigits       | 271 ms                                                       | 261 ms: 1.04x faster                                             |
| Geometric mean | (ref)                                                        | 1.32x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 143 ms: 1.33x faster                                             |
| regex_v8       | 27.2 ms                                                      | 22.8 ms: 1.19x faster                                            |
| regex_dna      | 261 ms                                                       | 237 ms: 1.10x faster                                             |
| regex_effbot   | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                            |
| Geometric mean | (ref)                                                        | 1.11x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 204 us: 1.53x faster                                             |
| json_dumps           | 14.5 ms                                                      | 10.2 ms: 1.43x faster                                            |
| pickle_pure_python   | 455 us                                                       | 325 us: 1.40x faster                                             |
| tomli_loads          | 2.92 sec                                                     | 2.12 sec: 1.37x faster                                           |
| xml_etree_process    | 75.9 ms                                                      | 59.0 ms: 1.29x faster                                            |
| json_loads           | 30.3 us                                                      | 24.2 us: 1.25x faster                                            |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                             |
| xml_etree_generate   | 92.3 ms                                                      | 86.8 ms: 1.06x faster                                            |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.04x faster                                             |
| unpickle_list        | 4.65 us                                                      | 4.72 us: 1.02x slower                                            |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                            |
| pickle_list          | 4.12 us                                                      | 4.37 us: 1.06x slower                                            |
| unpickle             | 13.5 us                                                      | 14.4 us: 1.07x slower                                            |
| pickle_dict          | 29.5 us                                                      | 33.2 us: 1.13x slower                                            |
| Geometric mean       | (ref)                                                        | 1.14x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup_no_site | 7.33 ms                                                      | 8.50 ms: 1.16x slower                                            |
| Geometric mean         | (ref)                                                        | 1.08x slower                                                     |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 9.94 ms: 1.48x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 149 us: 3.60x faster                                             |
| deltablue                | 7.50 ms                                                      | 3.22 ms: 2.33x faster                                            |
| asyncio_tcp              | 779 ms                                                       | 380 ms: 2.05x faster                                             |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.98x faster                                           |
| logging_silent           | 167 ns                                                       | 93.0 ns: 1.80x faster                                            |
| richards_super           | 90.6 ms                                                      | 51.1 ms: 1.77x faster                                            |
| go                       | 262 ms                                                       | 148 ms: 1.77x faster                                             |
| scimark_lu               | 167 ms                                                       | 98.0 ms: 1.70x faster                                            |
| chaos                    | 109 ms                                                       | 64.0 ms: 1.70x faster                                            |
| richards                 | 75.1 ms                                                      | 45.0 ms: 1.67x faster                                            |
| pyflate                  | 733 ms                                                       | 443 ms: 1.66x faster                                             |
| scimark_sor              | 180 ms                                                       | 109 ms: 1.65x faster                                             |
| raytrace                 | 489 ms                                                       | 297 ms: 1.65x faster                                             |
| generators               | 57.3 ms                                                      | 35.1 ms: 1.63x faster                                            |
| sqlglot_parse            | 2.24 ms                                                      | 1.38 ms: 1.62x faster                                            |
| hexiom                   | 9.42 ms                                                      | 5.88 ms: 1.60x faster                                            |
| nbody                    | 134 ms                                                       | 84.7 ms: 1.58x faster                                            |
| scimark_monte_carlo      | 107 ms                                                       | 68.2 ms: 1.57x faster                                            |
| unpickle_pure_python     | 312 us                                                       | 204 us: 1.53x faster                                             |
| async_tree_io            | 1.60 sec                                                     | 1.05 sec: 1.53x faster                                           |
| async_tree_none          | 692 ms                                                       | 453 ms: 1.53x faster                                             |
| async_tree_memoization   | 819 ms                                                       | 544 ms: 1.51x faster                                             |
| sqlglot_transpile        | 2.68 ms                                                      | 1.79 ms: 1.50x faster                                            |
| mako                     | 14.7 ms                                                      | 9.94 ms: 1.48x faster                                            |
| spectral_norm            | 139 ms                                                       | 94.5 ms: 1.47x faster                                            |
| crypto_pyaes             | 119 ms                                                       | 82.5 ms: 1.44x faster                                            |
| json_dumps               | 14.5 ms                                                      | 10.2 ms: 1.43x faster                                            |
| float                    | 111 ms                                                       | 78.6 ms: 1.41x faster                                            |
| pickle_pure_python       | 455 us                                                       | 325 us: 1.40x faster                                             |
| tomli_loads              | 2.92 sec                                                     | 2.12 sec: 1.37x faster                                           |
| deepcopy_memo            | 49.8 us                                                      | 36.5 us: 1.36x faster                                            |
| tornado_http             | 157 ms                                                       | 115 ms: 1.36x faster                                             |
| fannkuch                 | 483 ms                                                       | 355 ms: 1.36x faster                                             |
| coroutines               | 30.3 ms                                                      | 22.3 ms: 1.36x faster                                            |
| logging_format           | 9.64 us                                                      | 7.14 us: 1.35x faster                                            |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 696 ms: 1.35x faster                                             |
| logging_simple           | 8.88 us                                                      | 6.60 us: 1.35x faster                                            |
| regex_compile            | 190 ms                                                       | 143 ms: 1.33x faster                                             |
| pycparser                | 1.67 sec                                                     | 1.27 sec: 1.32x faster                                           |
| pprint_pformat           | 2.15 sec                                                     | 1.65 sec: 1.30x faster                                           |
| pprint_safe_repr         | 1.05 sec                                                     | 809 ms: 1.30x faster                                             |
| xml_etree_process        | 75.9 ms                                                      | 59.0 ms: 1.29x faster                                            |
| nqueens                  | 115 ms                                                       | 90.2 ms: 1.27x faster                                            |
| deepcopy                 | 468 us                                                       | 370 us: 1.26x faster                                             |
| sqlglot_normalize        | 144 ms                                                       | 115 ms: 1.25x faster                                             |
| json_loads               | 30.3 us                                                      | 24.2 us: 1.25x faster                                            |
| unpack_sequence          | 59.9 ns                                                      | 48.1 ns: 1.25x faster                                            |
| comprehensions           | 26.7 us                                                      | 21.6 us: 1.24x faster                                            |
| 2to3                     | 350 ms                                                       | 284 ms: 1.23x faster                                             |
| sqlglot_optimize         | 70.1 ms                                                      | 57.2 ms: 1.23x faster                                            |
| dulwich_log              | 81.1 ms                                                      | 66.1 ms: 1.23x faster                                            |
| bench_thread_pool        | 1.14 ms                                                      | 943 us: 1.21x faster                                             |
| mdp                      | 3.01 sec                                                     | 2.53 sec: 1.19x faster                                           |
| deepcopy_reduce          | 4.01 us                                                      | 3.37 us: 1.19x faster                                            |
| regex_v8                 | 27.2 ms                                                      | 22.8 ms: 1.19x faster                                            |
| docutils                 | 3.41 sec                                                     | 2.87 sec: 1.19x faster                                           |
| scimark_fft              | 361 ms                                                       | 305 ms: 1.19x faster                                             |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.38 ms: 1.16x faster                                            |
| json                     | 5.86 ms                                                      | 5.16 ms: 1.14x faster                                            |
| sqlite_synth             | 2.99 us                                                      | 2.68 us: 1.12x faster                                            |
| async_generators         | 421 ms                                                       | 379 ms: 1.11x faster                                             |
| pathlib                  | 21.4 ms                                                      | 19.3 ms: 1.11x faster                                            |
| regex_dna                | 261 ms                                                       | 237 ms: 1.10x faster                                             |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                             |
| meteor_contest           | 138 ms                                                       | 127 ms: 1.09x faster                                             |
| xml_etree_generate       | 92.3 ms                                                      | 86.8 ms: 1.06x faster                                            |
| create_gc_cycles         | 1.76 ms                                                      | 1.68 ms: 1.05x faster                                            |
| xml_etree_iterparse      | 110 ms                                                       | 106 ms: 1.04x faster                                             |
| pidigits                 | 271 ms                                                       | 261 ms: 1.04x faster                                             |
| telco                    | 7.23 ms                                                      | 7.11 ms: 1.02x faster                                            |
| unpickle_list            | 4.65 us                                                      | 4.72 us: 1.02x slower                                            |
| pickle                   | 9.89 us                                                      | 10.1 us: 1.02x slower                                            |
| pickle_list              | 4.12 us                                                      | 4.37 us: 1.06x slower                                            |
| unpickle                 | 13.5 us                                                      | 14.4 us: 1.07x slower                                            |
| gc_traversal             | 3.42 ms                                                      | 3.79 ms: 1.11x slower                                            |
| pickle_dict              | 29.5 us                                                      | 33.2 us: 1.13x slower                                            |
| regex_effbot             | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                            |
| python_startup_no_site   | 7.33 ms                                                      | 8.50 ms: 1.16x slower                                            |
| dask                     | 472 ms                                                       | 551 ms: 1.17x slower                                             |
| bench_mp_pool            | 6.37 ms                                                      | 8.65 ms: 1.36x slower                                            |
| coverage                 | 63.3 ms                                                      | 88.0 ms: 1.39x slower                                            |
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