
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b4
- machine: linux-x86_64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.07x faster \*
- HPT reliability: 99.96%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 285 ms: 1.01x faster                                             |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                           |
| tornado_http   | 124 ms                                                       | 120 ms: 1.04x faster                                             |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 551 ms: 1.14x faster                                             |
| async_tree_none         | 518 ms                                                       | 458 ms: 1.13x faster                                             |
| async_tree_io           | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                           |
| async_tree_cpu_io_mixed | 753 ms                                                       | 700 ms: 1.08x faster                                             |
| Geometric mean          | (ref)                                                        | 1.11x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 85.5 ms: 1.09x faster                                            |
| pidigits       | 251 ms                                                       | 260 ms: 1.03x slower                                             |
| float          | 74.9 ms                                                      | 77.8 ms: 1.04x slower                                            |
| Geometric mean | (ref)                                                        | 1.00x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 144 ms: 1.09x faster                                             |
| regex_v8       | 24.4 ms                                                      | 23.7 ms: 1.03x faster                                            |
| regex_dna      | 227 ms                                                       | 236 ms: 1.04x slower                                             |
| regex_effbot   | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                            |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                            |
| json_loads           | 28.9 us                                                      | 25.1 us: 1.15x faster                                            |
| unpickle_pure_python | 238 us                                                       | 207 us: 1.15x faster                                             |
| tomli_loads          | 2.25 sec                                                     | 2.18 sec: 1.03x faster                                           |
| xml_etree_parse      | 155 ms                                                       | 151 ms: 1.02x faster                                             |
| pickle_pure_python   | 316 us                                                       | 319 us: 1.01x slower                                             |
| pickle_dict          | 32.3 us                                                      | 33.2 us: 1.03x slower                                            |
| unpickle_list        | 4.60 us                                                      | 4.74 us: 1.03x slower                                            |
| xml_etree_process    | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                            |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                            |
| xml_etree_generate   | 79.7 ms                                                      | 85.2 ms: 1.07x slower                                            |
| unpickle             | 13.3 us                                                      | 14.6 us: 1.10x slower                                            |
| pickle_list          | 3.94 us                                                      | 4.44 us: 1.13x slower                                            |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                     |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                            |
| python_startup_no_site | 7.73 ms                                                      | 8.52 ms: 1.10x slower                                            |
| Geometric mean         | (ref)                                                        | 1.09x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 9.88 ms: 1.11x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf2-x86_64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 532 us                                                       | 151 us: 3.51x faster                                             |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                           |
| asyncio_tcp              | 747 ms                                                       | 383 ms: 1.95x faster                                             |
| generators               | 54.6 ms                                                      | 36.2 ms: 1.51x faster                                            |
| json_dumps               | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                            |
| richards_super           | 63.6 ms                                                      | 51.0 ms: 1.25x faster                                            |
| deltablue                | 3.97 ms                                                      | 3.19 ms: 1.25x faster                                            |
| fannkuch                 | 416 ms                                                       | 342 ms: 1.22x faster                                             |
| chaos                    | 74.9 ms                                                      | 62.5 ms: 1.20x faster                                            |
| hexiom                   | 6.98 ms                                                      | 5.84 ms: 1.19x faster                                            |
| scimark_lu               | 114 ms                                                       | 96.5 ms: 1.18x faster                                            |
| gc_traversal             | 4.15 ms                                                      | 3.52 ms: 1.18x faster                                            |
| coroutines               | 27.8 ms                                                      | 23.7 ms: 1.17x faster                                            |
| json_loads               | 28.9 us                                                      | 25.1 us: 1.15x faster                                            |
| unpickle_pure_python     | 238 us                                                       | 207 us: 1.15x faster                                             |
| nqueens                  | 103 ms                                                       | 89.7 ms: 1.14x faster                                            |
| comprehensions           | 25.1 us                                                      | 21.9 us: 1.14x faster                                            |
| async_tree_memoization   | 629 ms                                                       | 551 ms: 1.14x faster                                             |
| async_tree_none          | 518 ms                                                       | 458 ms: 1.13x faster                                             |
| richards                 | 49.7 ms                                                      | 44.4 ms: 1.12x faster                                            |
| mako                     | 11.0 ms                                                      | 9.88 ms: 1.11x faster                                            |
| async_tree_io            | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                           |
| mdp                      | 2.77 sec                                                     | 2.51 sec: 1.10x faster                                           |
| logging_simple           | 7.24 us                                                      | 6.64 us: 1.09x faster                                            |
| nbody                    | 92.9 ms                                                      | 85.5 ms: 1.09x faster                                            |
| regex_compile            | 156 ms                                                       | 144 ms: 1.09x faster                                             |
| go                       | 158 ms                                                       | 145 ms: 1.09x faster                                             |
| sqlglot_parse            | 1.51 ms                                                      | 1.40 ms: 1.08x faster                                            |
| json                     | 5.58 ms                                                      | 5.19 ms: 1.08x faster                                            |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 700 ms: 1.08x faster                                             |
| logging_silent           | 100 ns                                                       | 93.5 ns: 1.07x faster                                            |
| sqlglot_transpile        | 1.91 ms                                                      | 1.79 ms: 1.07x faster                                            |
| bench_thread_pool        | 1.00 ms                                                      | 942 us: 1.06x faster                                             |
| pycparser                | 1.31 sec                                                     | 1.23 sec: 1.06x faster                                           |
| logging_format           | 7.71 us                                                      | 7.31 us: 1.06x faster                                            |
| sqlglot_normalize        | 122 ms                                                       | 115 ms: 1.05x faster                                             |
| deepcopy                 | 391 us                                                       | 372 us: 1.05x faster                                             |
| spectral_norm            | 95.1 ms                                                      | 91.5 ms: 1.04x faster                                            |
| tornado_http             | 124 ms                                                       | 120 ms: 1.04x faster                                             |
| deepcopy_memo            | 37.5 us                                                      | 36.2 us: 1.04x faster                                            |
| tomli_loads              | 2.25 sec                                                     | 2.18 sec: 1.03x faster                                           |
| pprint_pformat           | 1.67 sec                                                     | 1.62 sec: 1.03x faster                                           |
| raytrace                 | 309 ms                                                       | 300 ms: 1.03x faster                                             |
| regex_v8                 | 24.4 ms                                                      | 23.7 ms: 1.03x faster                                            |
| crypto_pyaes             | 83.3 ms                                                      | 81.1 ms: 1.03x faster                                            |
| sqlglot_optimize         | 59.0 ms                                                      | 57.4 ms: 1.03x faster                                            |
| meteor_contest           | 131 ms                                                       | 127 ms: 1.03x faster                                             |
| xml_etree_parse          | 155 ms                                                       | 151 ms: 1.02x faster                                             |
| scimark_sor              | 110 ms                                                       | 107 ms: 1.02x faster                                             |
| pprint_safe_repr         | 805 ms                                                       | 789 ms: 1.02x faster                                             |
| dulwich_log              | 67.4 ms                                                      | 66.3 ms: 1.02x faster                                            |
| 2to3                     | 287 ms                                                       | 285 ms: 1.01x faster                                             |
| scimark_monte_carlo      | 69.8 ms                                                      | 69.3 ms: 1.01x faster                                            |
| pickle_pure_python       | 316 us                                                       | 319 us: 1.01x slower                                             |
| docutils                 | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                           |
| pyflate                  | 449 ms                                                       | 457 ms: 1.02x slower                                             |
| pickle_dict              | 32.3 us                                                      | 33.2 us: 1.03x slower                                            |
| unpickle_list            | 4.60 us                                                      | 4.74 us: 1.03x slower                                            |
| pidigits                 | 251 ms                                                       | 260 ms: 1.03x slower                                             |
| regex_dna                | 227 ms                                                       | 236 ms: 1.04x slower                                             |
| float                    | 74.9 ms                                                      | 77.8 ms: 1.04x slower                                            |
| xml_etree_process        | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                            |
| create_gc_cycles         | 1.58 ms                                                      | 1.65 ms: 1.05x slower                                            |
| telco                    | 6.81 ms                                                      | 7.13 ms: 1.05x slower                                            |
| regex_effbot             | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                            |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                            |
| xml_etree_generate       | 79.7 ms                                                      | 85.2 ms: 1.07x slower                                            |
| python_startup           | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                            |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.36 ms: 1.07x slower                                            |
| scimark_fft              | 281 ms                                                       | 302 ms: 1.08x slower                                             |
| sqlite_synth             | 2.52 us                                                      | 2.75 us: 1.09x slower                                            |
| unpack_sequence          | 45.7 ns                                                      | 50.2 ns: 1.10x slower                                            |
| python_startup_no_site   | 7.73 ms                                                      | 8.52 ms: 1.10x slower                                            |
| unpickle                 | 13.3 us                                                      | 14.6 us: 1.10x slower                                            |
| pickle_list              | 3.94 us                                                      | 4.44 us: 1.13x slower                                            |
| bench_mp_pool            | 4.70 ms                                                      | 5.44 ms: 1.16x slower                                            |
| async_generators         | 322 ms                                                       | 390 ms: 1.21x slower                                             |
| dask                     | 410 ms                                                       | 558 ms: 1.36x slower                                             |
| coverage                 | 66.1 ms                                                      | 91.3 ms: 1.38x slower                                            |
| Geometric mean           | (ref)                                                        | 1.07x faster                                                     |

Benchmark hidden because not significant (3): deepcopy_reduce, xml_etree_iterparse, pathlib
Ignored benchmarks (22) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.17x