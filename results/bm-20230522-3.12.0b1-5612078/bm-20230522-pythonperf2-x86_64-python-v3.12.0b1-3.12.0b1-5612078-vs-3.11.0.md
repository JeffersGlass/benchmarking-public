
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b1
- machine: linux-x86_64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.96%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.16x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 284 ms: 1.01x faster                                             |
| docutils       | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                           |
| tornado_http   | 124 ms                                                       | 115 ms: 1.08x faster                                             |
| Geometric mean | (ref)                                                        | 1.03x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 544 ms: 1.16x faster                                             |
| async_tree_none         | 518 ms                                                       | 453 ms: 1.14x faster                                             |
| async_tree_io           | 1.17 sec                                                     | 1.05 sec: 1.12x faster                                           |
| async_tree_cpu_io_mixed | 753 ms                                                       | 696 ms: 1.08x faster                                             |
| Geometric mean          | (ref)                                                        | 1.13x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 84.7 ms: 1.10x faster                                            |
| pidigits       | 251 ms                                                       | 261 ms: 1.04x slower                                             |
| float          | 74.9 ms                                                      | 78.6 ms: 1.05x slower                                            |
| Geometric mean | (ref)                                                        | 1.00x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 143 ms: 1.09x faster                                             |
| regex_v8       | 24.4 ms                                                      | 22.8 ms: 1.07x faster                                            |
| regex_dna      | 227 ms                                                       | 237 ms: 1.04x slower                                             |
| regex_effbot   | 3.34 ms                                                      | 3.49 ms: 1.05x slower                                            |
| Geometric mean | (ref)                                                        | 1.02x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                            |
| json_loads           | 28.9 us                                                      | 24.2 us: 1.19x faster                                            |
| unpickle_pure_python | 238 us                                                       | 204 us: 1.17x faster                                             |
| tomli_loads          | 2.25 sec                                                     | 2.12 sec: 1.06x faster                                           |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.05x faster                                             |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                            |
| unpickle_list        | 4.60 us                                                      | 4.72 us: 1.03x slower                                            |
| pickle_dict          | 32.3 us                                                      | 33.2 us: 1.03x slower                                            |
| pickle_pure_python   | 316 us                                                       | 325 us: 1.03x slower                                             |
| xml_etree_process    | 55.9 ms                                                      | 59.0 ms: 1.06x slower                                            |
| xml_etree_generate   | 79.7 ms                                                      | 86.8 ms: 1.09x slower                                            |
| unpickle             | 13.3 us                                                      | 14.4 us: 1.09x slower                                            |
| pickle_list          | 3.94 us                                                      | 4.37 us: 1.11x slower                                            |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                     |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                            |
| python_startup_no_site | 7.73 ms                                                      | 8.50 ms: 1.10x slower                                            |
| Geometric mean         | (ref)                                                        | 1.09x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 9.94 ms: 1.11x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 532 us                                                       | 149 us: 3.57x faster                                             |
| asyncio_tcp              | 747 ms                                                       | 380 ms: 1.97x faster                                             |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                           |
| generators               | 54.6 ms                                                      | 35.1 ms: 1.56x faster                                            |
| json_dumps               | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                            |
| richards_super           | 63.6 ms                                                      | 51.1 ms: 1.25x faster                                            |
| coroutines               | 27.8 ms                                                      | 22.3 ms: 1.24x faster                                            |
| deltablue                | 3.97 ms                                                      | 3.22 ms: 1.23x faster                                            |
| json_loads               | 28.9 us                                                      | 24.2 us: 1.19x faster                                            |
| hexiom                   | 6.98 ms                                                      | 5.88 ms: 1.19x faster                                            |
| fannkuch                 | 416 ms                                                       | 355 ms: 1.17x faster                                             |
| unpickle_pure_python     | 238 us                                                       | 204 us: 1.17x faster                                             |
| chaos                    | 74.9 ms                                                      | 64.0 ms: 1.17x faster                                            |
| scimark_lu               | 114 ms                                                       | 98.0 ms: 1.16x faster                                            |
| comprehensions           | 25.1 us                                                      | 21.6 us: 1.16x faster                                            |
| async_tree_memoization   | 629 ms                                                       | 544 ms: 1.16x faster                                             |
| async_tree_none          | 518 ms                                                       | 453 ms: 1.14x faster                                             |
| nqueens                  | 103 ms                                                       | 90.2 ms: 1.14x faster                                            |
| async_tree_io            | 1.17 sec                                                     | 1.05 sec: 1.12x faster                                           |
| mako                     | 11.0 ms                                                      | 9.94 ms: 1.11x faster                                            |
| richards                 | 49.7 ms                                                      | 45.0 ms: 1.10x faster                                            |
| logging_simple           | 7.24 us                                                      | 6.60 us: 1.10x faster                                            |
| nbody                    | 92.9 ms                                                      | 84.7 ms: 1.10x faster                                            |
| mdp                      | 2.77 sec                                                     | 2.53 sec: 1.10x faster                                           |
| sqlglot_parse            | 1.51 ms                                                      | 1.38 ms: 1.10x faster                                            |
| gc_traversal             | 4.15 ms                                                      | 3.79 ms: 1.10x faster                                            |
| regex_compile            | 156 ms                                                       | 143 ms: 1.09x faster                                             |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 696 ms: 1.08x faster                                             |
| json                     | 5.58 ms                                                      | 5.16 ms: 1.08x faster                                            |
| logging_format           | 7.71 us                                                      | 7.14 us: 1.08x faster                                            |
| tornado_http             | 124 ms                                                       | 115 ms: 1.08x faster                                             |
| logging_silent           | 100 ns                                                       | 93.0 ns: 1.08x faster                                            |
| regex_v8                 | 24.4 ms                                                      | 22.8 ms: 1.07x faster                                            |
| sqlglot_transpile        | 1.91 ms                                                      | 1.79 ms: 1.07x faster                                            |
| go                       | 158 ms                                                       | 148 ms: 1.07x faster                                             |
| sqlglot_normalize        | 122 ms                                                       | 115 ms: 1.06x faster                                             |
| bench_thread_pool        | 1.00 ms                                                      | 943 us: 1.06x faster                                             |
| tomli_loads              | 2.25 sec                                                     | 2.12 sec: 1.06x faster                                           |
| deepcopy                 | 391 us                                                       | 370 us: 1.06x faster                                             |
| xml_etree_parse          | 155 ms                                                       | 147 ms: 1.05x faster                                             |
| raytrace                 | 309 ms                                                       | 297 ms: 1.04x faster                                             |
| pycparser                | 1.31 sec                                                     | 1.27 sec: 1.03x faster                                           |
| sqlglot_optimize         | 59.0 ms                                                      | 57.2 ms: 1.03x faster                                            |
| deepcopy_memo            | 37.5 us                                                      | 36.5 us: 1.03x faster                                            |
| meteor_contest           | 131 ms                                                       | 127 ms: 1.03x faster                                             |
| scimark_monte_carlo      | 69.8 ms                                                      | 68.2 ms: 1.02x faster                                            |
| dulwich_log              | 67.4 ms                                                      | 66.1 ms: 1.02x faster                                            |
| pyflate                  | 449 ms                                                       | 443 ms: 1.01x faster                                             |
| 2to3                     | 287 ms                                                       | 284 ms: 1.01x faster                                             |
| pprint_pformat           | 1.67 sec                                                     | 1.65 sec: 1.01x faster                                           |
| crypto_pyaes             | 83.3 ms                                                      | 82.5 ms: 1.01x faster                                            |
| deepcopy_reduce          | 3.40 us                                                      | 3.37 us: 1.01x faster                                            |
| spectral_norm            | 95.1 ms                                                      | 94.5 ms: 1.01x faster                                            |
| pprint_safe_repr         | 805 ms                                                       | 809 ms: 1.01x slower                                             |
| docutils                 | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                           |
| pickle                   | 9.89 us                                                      | 10.1 us: 1.02x slower                                            |
| pathlib                  | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                            |
| unpickle_list            | 4.60 us                                                      | 4.72 us: 1.03x slower                                            |
| pickle_dict              | 32.3 us                                                      | 33.2 us: 1.03x slower                                            |
| pickle_pure_python       | 316 us                                                       | 325 us: 1.03x slower                                             |
| pidigits                 | 251 ms                                                       | 261 ms: 1.04x slower                                             |
| telco                    | 6.81 ms                                                      | 7.11 ms: 1.04x slower                                            |
| regex_dna                | 227 ms                                                       | 237 ms: 1.04x slower                                             |
| regex_effbot             | 3.34 ms                                                      | 3.49 ms: 1.05x slower                                            |
| float                    | 74.9 ms                                                      | 78.6 ms: 1.05x slower                                            |
| unpack_sequence          | 45.7 ns                                                      | 48.1 ns: 1.05x slower                                            |
| xml_etree_process        | 55.9 ms                                                      | 59.0 ms: 1.06x slower                                            |
| sqlite_synth             | 2.52 us                                                      | 2.68 us: 1.06x slower                                            |
| create_gc_cycles         | 1.58 ms                                                      | 1.68 ms: 1.06x slower                                            |
| python_startup           | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                            |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.38 ms: 1.08x slower                                            |
| scimark_fft              | 281 ms                                                       | 305 ms: 1.09x slower                                             |
| xml_etree_generate       | 79.7 ms                                                      | 86.8 ms: 1.09x slower                                            |
| unpickle                 | 13.3 us                                                      | 14.4 us: 1.09x slower                                            |
| python_startup_no_site   | 7.73 ms                                                      | 8.50 ms: 1.10x slower                                            |
| pickle_list              | 3.94 us                                                      | 4.37 us: 1.11x slower                                            |
| async_generators         | 322 ms                                                       | 379 ms: 1.18x slower                                             |
| coverage                 | 66.1 ms                                                      | 88.0 ms: 1.33x slower                                            |
| dask                     | 410 ms                                                       | 551 ms: 1.34x slower                                             |
| bench_mp_pool            | 4.70 ms                                                      | 8.65 ms: 1.84x slower                                            |
| Geometric mean           | (ref)                                                        | 1.06x faster                                                     |

Benchmark hidden because not significant (2): xml_etree_iterparse, scimark_sor
Ignored benchmarks (22) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.16x