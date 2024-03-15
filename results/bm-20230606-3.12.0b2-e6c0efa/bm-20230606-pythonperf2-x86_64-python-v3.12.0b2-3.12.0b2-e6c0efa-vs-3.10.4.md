
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b2
- machine: linux-x86_64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 285 ms: 1.23x faster                                             |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                           |
| tornado_http   | 157 ms                                                       | 121 ms: 1.30x faster                                             |
| Geometric mean | (ref)                                                        | 1.24x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 452 ms: 1.53x faster                                             |
| async_tree_io           | 1.60 sec                                                     | 1.04 sec: 1.53x faster                                           |
| async_tree_memoization  | 819 ms                                                       | 546 ms: 1.50x faster                                             |
| async_tree_cpu_io_mixed | 936 ms                                                       | 697 ms: 1.34x faster                                             |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 83.7 ms: 1.60x faster                                            |
| float          | 111 ms                                                       | 77.3 ms: 1.44x faster                                            |
| pidigits       | 271 ms                                                       | 259 ms: 1.04x faster                                             |
| Geometric mean | (ref)                                                        | 1.34x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 144 ms: 1.32x faster                                             |
| regex_v8       | 27.2 ms                                                      | 23.6 ms: 1.15x faster                                            |
| regex_dna      | 261 ms                                                       | 245 ms: 1.06x faster                                             |
| regex_effbot   | 3.09 ms                                                      | 3.55 ms: 1.15x slower                                            |
| Geometric mean | (ref)                                                        | 1.09x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 205 us: 1.52x faster                                             |
| json_dumps           | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                            |
| pickle_pure_python   | 455 us                                                       | 324 us: 1.41x faster                                             |
| tomli_loads          | 2.92 sec                                                     | 2.19 sec: 1.33x faster                                           |
| xml_etree_process    | 75.9 ms                                                      | 58.8 ms: 1.29x faster                                            |
| json_loads           | 30.3 us                                                      | 24.5 us: 1.24x faster                                            |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                             |
| xml_etree_generate   | 92.3 ms                                                      | 85.6 ms: 1.08x faster                                            |
| xml_etree_iterparse  | 110 ms                                                       | 104 ms: 1.07x faster                                             |
| unpickle_list        | 4.65 us                                                      | 4.71 us: 1.01x slower                                            |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                            |
| pickle_list          | 4.12 us                                                      | 4.27 us: 1.04x slower                                            |
| pickle_dict          | 29.5 us                                                      | 31.2 us: 1.06x slower                                            |
| unpickle             | 13.5 us                                                      | 14.6 us: 1.08x slower                                            |
| Geometric mean       | (ref)                                                        | 1.14x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.4 ms: 1.01x faster                                            |
| python_startup_no_site | 7.33 ms                                                      | 8.45 ms: 1.15x slower                                            |
| Geometric mean         | (ref)                                                        | 1.07x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 9.93 ms: 1.48x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 150 us: 3.58x faster                                             |
| deltablue                | 7.50 ms                                                      | 3.25 ms: 2.31x faster                                            |
| asyncio_tcp              | 779 ms                                                       | 379 ms: 2.06x faster                                             |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.98x faster                                           |
| go                       | 262 ms                                                       | 147 ms: 1.79x faster                                             |
| logging_silent           | 167 ns                                                       | 93.8 ns: 1.78x faster                                            |
| richards_super           | 90.6 ms                                                      | 51.0 ms: 1.78x faster                                            |
| scimark_lu               | 167 ms                                                       | 96.3 ms: 1.73x faster                                            |
| chaos                    | 109 ms                                                       | 63.6 ms: 1.71x faster                                            |
| scimark_sor              | 180 ms                                                       | 107 ms: 1.69x faster                                             |
| pyflate                  | 733 ms                                                       | 441 ms: 1.66x faster                                             |
| richards                 | 75.1 ms                                                      | 45.5 ms: 1.65x faster                                            |
| generators               | 57.3 ms                                                      | 35.5 ms: 1.62x faster                                            |
| sqlglot_parse            | 2.24 ms                                                      | 1.40 ms: 1.60x faster                                            |
| nbody                    | 134 ms                                                       | 83.7 ms: 1.60x faster                                            |
| raytrace                 | 489 ms                                                       | 307 ms: 1.59x faster                                             |
| hexiom                   | 9.42 ms                                                      | 5.95 ms: 1.58x faster                                            |
| scimark_monte_carlo      | 107 ms                                                       | 69.2 ms: 1.55x faster                                            |
| async_tree_none          | 692 ms                                                       | 452 ms: 1.53x faster                                             |
| async_tree_io            | 1.60 sec                                                     | 1.04 sec: 1.53x faster                                           |
| unpickle_pure_python     | 312 us                                                       | 205 us: 1.52x faster                                             |
| spectral_norm            | 139 ms                                                       | 91.6 ms: 1.52x faster                                            |
| async_tree_memoization   | 819 ms                                                       | 546 ms: 1.50x faster                                             |
| sqlglot_transpile        | 2.68 ms                                                      | 1.80 ms: 1.49x faster                                            |
| mako                     | 14.7 ms                                                      | 9.93 ms: 1.48x faster                                            |
| crypto_pyaes             | 119 ms                                                       | 81.2 ms: 1.47x faster                                            |
| float                    | 111 ms                                                       | 77.3 ms: 1.44x faster                                            |
| json_dumps               | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                            |
| fannkuch                 | 483 ms                                                       | 343 ms: 1.41x faster                                             |
| pickle_pure_python       | 455 us                                                       | 324 us: 1.41x faster                                             |
| deepcopy_memo            | 49.8 us                                                      | 36.0 us: 1.38x faster                                            |
| coroutines               | 30.3 ms                                                      | 22.3 ms: 1.36x faster                                            |
| pycparser                | 1.67 sec                                                     | 1.24 sec: 1.35x faster                                           |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 697 ms: 1.34x faster                                             |
| tomli_loads              | 2.92 sec                                                     | 2.19 sec: 1.33x faster                                           |
| pprint_pformat           | 2.15 sec                                                     | 1.62 sec: 1.33x faster                                           |
| pprint_safe_repr         | 1.05 sec                                                     | 792 ms: 1.33x faster                                             |
| logging_simple           | 8.88 us                                                      | 6.73 us: 1.32x faster                                            |
| regex_compile            | 190 ms                                                       | 144 ms: 1.32x faster                                             |
| logging_format           | 9.64 us                                                      | 7.35 us: 1.31x faster                                            |
| tornado_http             | 157 ms                                                       | 121 ms: 1.30x faster                                             |
| xml_etree_process        | 75.9 ms                                                      | 58.8 ms: 1.29x faster                                            |
| nqueens                  | 115 ms                                                       | 89.5 ms: 1.28x faster                                            |
| deepcopy                 | 468 us                                                       | 369 us: 1.27x faster                                             |
| json_loads               | 30.3 us                                                      | 24.5 us: 1.24x faster                                            |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                             |
| comprehensions           | 26.7 us                                                      | 21.6 us: 1.24x faster                                            |
| 2to3                     | 350 ms                                                       | 285 ms: 1.23x faster                                             |
| dulwich_log              | 81.1 ms                                                      | 65.9 ms: 1.23x faster                                            |
| scimark_fft              | 361 ms                                                       | 296 ms: 1.22x faster                                             |
| sqlglot_optimize         | 70.1 ms                                                      | 57.5 ms: 1.22x faster                                            |
| unpack_sequence          | 59.9 ns                                                      | 49.8 ns: 1.20x faster                                            |
| mdp                      | 3.01 sec                                                     | 2.51 sec: 1.20x faster                                           |
| bench_thread_pool        | 1.14 ms                                                      | 960 us: 1.19x faster                                             |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                           |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.29 ms: 1.18x faster                                            |
| bench_mp_pool            | 6.37 ms                                                      | 5.41 ms: 1.18x faster                                            |
| deepcopy_reduce          | 4.01 us                                                      | 3.40 us: 1.18x faster                                            |
| regex_v8                 | 27.2 ms                                                      | 23.6 ms: 1.15x faster                                            |
| json                     | 5.86 ms                                                      | 5.19 ms: 1.13x faster                                            |
| pathlib                  | 21.4 ms                                                      | 19.3 ms: 1.11x faster                                            |
| sqlite_synth             | 2.99 us                                                      | 2.71 us: 1.10x faster                                            |
| create_gc_cycles         | 1.76 ms                                                      | 1.62 ms: 1.09x faster                                            |
| meteor_contest           | 138 ms                                                       | 127 ms: 1.09x faster                                             |
| async_generators         | 421 ms                                                       | 389 ms: 1.08x faster                                             |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                             |
| xml_etree_generate       | 92.3 ms                                                      | 85.6 ms: 1.08x faster                                            |
| xml_etree_iterparse      | 110 ms                                                       | 104 ms: 1.07x faster                                             |
| regex_dna                | 261 ms                                                       | 245 ms: 1.06x faster                                             |
| pidigits                 | 271 ms                                                       | 259 ms: 1.04x faster                                             |
| telco                    | 7.23 ms                                                      | 7.08 ms: 1.02x faster                                            |
| python_startup           | 11.5 ms                                                      | 11.4 ms: 1.01x faster                                            |
| unpickle_list            | 4.65 us                                                      | 4.71 us: 1.01x slower                                            |
| pickle                   | 9.89 us                                                      | 10.0 us: 1.01x slower                                            |
| pickle_list              | 4.12 us                                                      | 4.27 us: 1.04x slower                                            |
| pickle_dict              | 29.5 us                                                      | 31.2 us: 1.06x slower                                            |
| unpickle                 | 13.5 us                                                      | 14.6 us: 1.08x slower                                            |
| gc_traversal             | 3.42 ms                                                      | 3.79 ms: 1.11x slower                                            |
| regex_effbot             | 3.09 ms                                                      | 3.55 ms: 1.15x slower                                            |
| python_startup_no_site   | 7.33 ms                                                      | 8.45 ms: 1.15x slower                                            |
| dask                     | 472 ms                                                       | 563 ms: 1.19x slower                                             |
| coverage                 | 63.3 ms                                                      | 88.5 ms: 1.40x slower                                            |
| Geometric mean           | (ref)                                                        | 1.31x faster                                                     |
Ignored benchmarks (18) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.28x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.26x