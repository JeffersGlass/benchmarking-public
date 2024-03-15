
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0rc1
- machine: linux-x86_64
- commit hash: 63bcd91
- commit date: 2023-08-05
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.26x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 287 ms: 1.22x faster                                               |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                             |
| tornado_http   | 157 ms                                                       | 122 ms: 1.29x faster                                               |
| Geometric mean | (ref)                                                        | 1.23x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                             |
| async_tree_none         | 692 ms                                                       | 459 ms: 1.51x faster                                               |
| async_tree_memoization  | 819 ms                                                       | 554 ms: 1.48x faster                                               |
| async_tree_cpu_io_mixed | 936 ms                                                       | 703 ms: 1.33x faster                                               |
| Geometric mean          | (ref)                                                        | 1.45x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 86.7 ms: 1.55x faster                                              |
| float          | 111 ms                                                       | 77.8 ms: 1.43x faster                                              |
| pidigits       | 271 ms                                                       | 260 ms: 1.04x faster                                               |
| Geometric mean | (ref)                                                        | 1.32x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 145 ms: 1.31x faster                                               |
| regex_v8       | 27.2 ms                                                      | 24.0 ms: 1.13x faster                                              |
| regex_dna      | 261 ms                                                       | 236 ms: 1.11x faster                                               |
| regex_effbot   | 3.09 ms                                                      | 3.38 ms: 1.10x slower                                              |
| Geometric mean | (ref)                                                        | 1.11x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 209 us: 1.49x faster                                               |
| pickle_pure_python   | 455 us                                                       | 325 us: 1.40x faster                                               |
| json_dumps           | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                              |
| tomli_loads          | 2.92 sec                                                     | 2.18 sec: 1.34x faster                                             |
| xml_etree_process    | 75.9 ms                                                      | 58.6 ms: 1.29x faster                                              |
| json_loads           | 30.3 us                                                      | 24.5 us: 1.24x faster                                              |
| xml_etree_generate   | 92.3 ms                                                      | 84.2 ms: 1.10x faster                                              |
| xml_etree_parse      | 160 ms                                                       | 149 ms: 1.08x faster                                               |
| xml_etree_iterparse  | 110 ms                                                       | 104 ms: 1.06x faster                                               |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                              |
| pickle_list          | 4.12 us                                                      | 4.35 us: 1.06x slower                                              |
| unpickle             | 13.5 us                                                      | 14.3 us: 1.06x slower                                              |
| pickle_dict          | 29.5 us                                                      | 31.6 us: 1.07x slower                                              |
| Geometric mean       | (ref)                                                        | 1.14x faster                                                       |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.5 ms: 1.00x faster                                              |
| python_startup_no_site | 7.33 ms                                                      | 8.50 ms: 1.16x slower                                              |
| Geometric mean         | (ref)                                                        | 1.07x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-----------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 9.91 ms: 1.48x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 151 us: 3.56x faster                                               |
| deltablue                | 7.50 ms                                                      | 3.21 ms: 2.33x faster                                              |
| asyncio_tcp              | 779 ms                                                       | 384 ms: 2.03x faster                                               |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                             |
| logging_silent           | 167 ns                                                       | 92.1 ns: 1.82x faster                                              |
| go                       | 262 ms                                                       | 146 ms: 1.80x faster                                               |
| richards_super           | 90.6 ms                                                      | 52.1 ms: 1.74x faster                                              |
| chaos                    | 109 ms                                                       | 63.5 ms: 1.71x faster                                              |
| scimark_lu               | 167 ms                                                       | 98.0 ms: 1.70x faster                                              |
| pyflate                  | 733 ms                                                       | 437 ms: 1.68x faster                                               |
| richards                 | 75.1 ms                                                      | 45.1 ms: 1.67x faster                                              |
| scimark_sor              | 180 ms                                                       | 109 ms: 1.65x faster                                               |
| raytrace                 | 489 ms                                                       | 300 ms: 1.63x faster                                               |
| hexiom                   | 9.42 ms                                                      | 5.81 ms: 1.62x faster                                              |
| sqlglot_parse            | 2.24 ms                                                      | 1.39 ms: 1.61x faster                                              |
| generators               | 57.3 ms                                                      | 36.4 ms: 1.58x faster                                              |
| nbody                    | 134 ms                                                       | 86.7 ms: 1.55x faster                                              |
| spectral_norm            | 139 ms                                                       | 90.9 ms: 1.53x faster                                              |
| scimark_monte_carlo      | 107 ms                                                       | 71.2 ms: 1.51x faster                                              |
| async_tree_io            | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                             |
| async_tree_none          | 692 ms                                                       | 459 ms: 1.51x faster                                               |
| unpickle_pure_python     | 312 us                                                       | 209 us: 1.49x faster                                               |
| sqlglot_transpile        | 2.68 ms                                                      | 1.80 ms: 1.49x faster                                              |
| mako                     | 14.7 ms                                                      | 9.91 ms: 1.48x faster                                              |
| async_tree_memoization   | 819 ms                                                       | 554 ms: 1.48x faster                                               |
| crypto_pyaes             | 119 ms                                                       | 81.8 ms: 1.46x faster                                              |
| float                    | 111 ms                                                       | 77.8 ms: 1.43x faster                                              |
| pickle_pure_python       | 455 us                                                       | 325 us: 1.40x faster                                               |
| json_dumps               | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                              |
| deepcopy_memo            | 49.8 us                                                      | 36.8 us: 1.35x faster                                              |
| tomli_loads              | 2.92 sec                                                     | 2.18 sec: 1.34x faster                                             |
| coroutines               | 30.3 ms                                                      | 22.6 ms: 1.34x faster                                              |
| fannkuch                 | 483 ms                                                       | 361 ms: 1.34x faster                                               |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 703 ms: 1.33x faster                                               |
| regex_compile            | 190 ms                                                       | 145 ms: 1.31x faster                                               |
| logging_simple           | 8.88 us                                                      | 6.82 us: 1.30x faster                                              |
| pprint_pformat           | 2.15 sec                                                     | 1.66 sec: 1.30x faster                                             |
| pycparser                | 1.67 sec                                                     | 1.29 sec: 1.30x faster                                             |
| bench_mp_pool            | 6.37 ms                                                      | 4.91 ms: 1.30x faster                                              |
| xml_etree_process        | 75.9 ms                                                      | 58.6 ms: 1.29x faster                                              |
| pprint_safe_repr         | 1.05 sec                                                     | 811 ms: 1.29x faster                                               |
| tornado_http             | 157 ms                                                       | 122 ms: 1.29x faster                                               |
| logging_format           | 9.64 us                                                      | 7.52 us: 1.28x faster                                              |
| nqueens                  | 115 ms                                                       | 89.9 ms: 1.28x faster                                              |
| json_loads               | 30.3 us                                                      | 24.5 us: 1.24x faster                                              |
| comprehensions           | 26.7 us                                                      | 21.7 us: 1.23x faster                                              |
| dulwich_log              | 81.1 ms                                                      | 66.1 ms: 1.23x faster                                              |
| sqlglot_normalize        | 144 ms                                                       | 118 ms: 1.22x faster                                               |
| scimark_fft              | 361 ms                                                       | 297 ms: 1.22x faster                                               |
| 2to3                     | 350 ms                                                       | 287 ms: 1.22x faster                                               |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.19 ms: 1.21x faster                                              |
| sqlglot_optimize         | 70.1 ms                                                      | 58.1 ms: 1.21x faster                                              |
| deepcopy                 | 468 us                                                       | 391 us: 1.20x faster                                               |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                             |
| bench_thread_pool        | 1.14 ms                                                      | 966 us: 1.18x faster                                               |
| mdp                      | 3.01 sec                                                     | 2.56 sec: 1.17x faster                                             |
| json                     | 5.86 ms                                                      | 5.13 ms: 1.14x faster                                              |
| regex_v8                 | 27.2 ms                                                      | 24.0 ms: 1.13x faster                                              |
| deepcopy_reduce          | 4.01 us                                                      | 3.55 us: 1.13x faster                                              |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.13x faster                                              |
| async_generators         | 421 ms                                                       | 380 ms: 1.11x faster                                               |
| regex_dna                | 261 ms                                                       | 236 ms: 1.11x faster                                               |
| sqlite_synth             | 2.99 us                                                      | 2.70 us: 1.11x faster                                              |
| xml_etree_generate       | 92.3 ms                                                      | 84.2 ms: 1.10x faster                                              |
| create_gc_cycles         | 1.76 ms                                                      | 1.62 ms: 1.09x faster                                              |
| meteor_contest           | 138 ms                                                       | 128 ms: 1.08x faster                                               |
| xml_etree_parse          | 160 ms                                                       | 149 ms: 1.08x faster                                               |
| unpack_sequence          | 59.9 ns                                                      | 56.2 ns: 1.07x faster                                              |
| xml_etree_iterparse      | 110 ms                                                       | 104 ms: 1.06x faster                                               |
| pidigits                 | 271 ms                                                       | 260 ms: 1.04x faster                                               |
| telco                    | 7.23 ms                                                      | 7.01 ms: 1.03x faster                                              |
| python_startup           | 11.5 ms                                                      | 11.5 ms: 1.00x faster                                              |
| pickle                   | 9.89 us                                                      | 10.0 us: 1.01x slower                                              |
| pickle_list              | 4.12 us                                                      | 4.35 us: 1.06x slower                                              |
| unpickle                 | 13.5 us                                                      | 14.3 us: 1.06x slower                                              |
| pickle_dict              | 29.5 us                                                      | 31.6 us: 1.07x slower                                              |
| regex_effbot             | 3.09 ms                                                      | 3.38 ms: 1.10x slower                                              |
| gc_traversal             | 3.42 ms                                                      | 3.77 ms: 1.10x slower                                              |
| python_startup_no_site   | 7.33 ms                                                      | 8.50 ms: 1.16x slower                                              |
| dask                     | 472 ms                                                       | 566 ms: 1.20x slower                                               |
| coverage                 | 63.3 ms                                                      | 87.0 ms: 1.38x slower                                              |
| Geometric mean           | (ref)                                                        | 1.30x faster                                                       |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (18) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.28x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.26x