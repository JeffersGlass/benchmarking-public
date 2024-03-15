
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b3
- machine: linux-x86_64
- commit hash: f992a60
- commit date: 2023-06-19
- overall geometric mean: 1.07x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 283 ms: 1.01x faster                                             |
| docutils       | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                           |
| tornado_http   | 124 ms                                                       | 118 ms: 1.05x faster                                             |
| Geometric mean | (ref)                                                        | 1.02x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 551 ms: 1.14x faster                                             |
| async_tree_none         | 518 ms                                                       | 457 ms: 1.13x faster                                             |
| async_tree_io           | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                           |
| async_tree_cpu_io_mixed | 753 ms                                                       | 704 ms: 1.07x faster                                             |
| Geometric mean          | (ref)                                                        | 1.11x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 84.2 ms: 1.10x faster                                            |
| pidigits       | 251 ms                                                       | 260 ms: 1.03x slower                                             |
| float          | 74.9 ms                                                      | 78.8 ms: 1.05x slower                                            |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 144 ms: 1.08x faster                                             |
| regex_v8       | 24.4 ms                                                      | 23.9 ms: 1.02x faster                                            |
| regex_effbot   | 3.34 ms                                                      | 3.48 ms: 1.04x slower                                            |
| regex_dna      | 227 ms                                                       | 238 ms: 1.05x slower                                             |
| Geometric mean | (ref)                                                        | 1.00x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.4 ms: 1.27x faster                                            |
| json_loads           | 28.9 us                                                      | 24.7 us: 1.17x faster                                            |
| unpickle_pure_python | 238 us                                                       | 209 us: 1.14x faster                                             |
| tomli_loads          | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                           |
| xml_etree_parse      | 155 ms                                                       | 150 ms: 1.03x faster                                             |
| unpickle_list        | 4.60 us                                                      | 4.65 us: 1.01x slower                                            |
| pickle_pure_python   | 316 us                                                       | 326 us: 1.03x slower                                             |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                            |
| pickle_dict          | 32.3 us                                                      | 33.6 us: 1.04x slower                                            |
| xml_etree_process    | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                            |
| xml_etree_generate   | 79.7 ms                                                      | 85.3 ms: 1.07x slower                                            |
| unpickle             | 13.3 us                                                      | 14.6 us: 1.10x slower                                            |
| pickle_list          | 3.94 us                                                      | 4.43 us: 1.12x slower                                            |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                     |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.4 ms: 1.06x slower                                            |
| python_startup_no_site | 7.73 ms                                                      | 8.43 ms: 1.09x slower                                            |
| Geometric mean         | (ref)                                                        | 1.08x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.0 ms: 1.10x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf2-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 532 us                                                       | 152 us: 3.50x faster                                             |
| asyncio_tcp              | 747 ms                                                       | 377 ms: 1.98x faster                                             |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 1.56 sec: 1.96x faster                                           |
| generators               | 54.6 ms                                                      | 36.7 ms: 1.49x faster                                            |
| json_dumps               | 13.3 ms                                                      | 10.4 ms: 1.27x faster                                            |
| richards_super           | 63.6 ms                                                      | 50.8 ms: 1.25x faster                                            |
| coroutines               | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                            |
| deltablue                | 3.97 ms                                                      | 3.21 ms: 1.24x faster                                            |
| fannkuch                 | 416 ms                                                       | 343 ms: 1.21x faster                                             |
| hexiom                   | 6.98 ms                                                      | 5.79 ms: 1.20x faster                                            |
| chaos                    | 74.9 ms                                                      | 63.4 ms: 1.18x faster                                            |
| scimark_lu               | 114 ms                                                       | 96.7 ms: 1.18x faster                                            |
| json_loads               | 28.9 us                                                      | 24.7 us: 1.17x faster                                            |
| comprehensions           | 25.1 us                                                      | 21.7 us: 1.16x faster                                            |
| async_tree_memoization   | 629 ms                                                       | 551 ms: 1.14x faster                                             |
| unpickle_pure_python     | 238 us                                                       | 209 us: 1.14x faster                                             |
| nqueens                  | 103 ms                                                       | 90.2 ms: 1.14x faster                                            |
| async_tree_none          | 518 ms                                                       | 457 ms: 1.13x faster                                             |
| logging_simple           | 7.24 us                                                      | 6.49 us: 1.12x faster                                            |
| richards                 | 49.7 ms                                                      | 44.7 ms: 1.11x faster                                            |
| mdp                      | 2.77 sec                                                     | 2.49 sec: 1.11x faster                                           |
| async_tree_io            | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                           |
| nbody                    | 92.9 ms                                                      | 84.2 ms: 1.10x faster                                            |
| mako                     | 11.0 ms                                                      | 10.0 ms: 1.10x faster                                            |
| logging_silent           | 100 ns                                                       | 91.8 ns: 1.09x faster                                            |
| sqlglot_parse            | 1.51 ms                                                      | 1.39 ms: 1.09x faster                                            |
| go                       | 158 ms                                                       | 145 ms: 1.08x faster                                             |
| regex_compile            | 156 ms                                                       | 144 ms: 1.08x faster                                             |
| logging_format           | 7.71 us                                                      | 7.13 us: 1.08x faster                                            |
| json                     | 5.58 ms                                                      | 5.18 ms: 1.08x faster                                            |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 704 ms: 1.07x faster                                             |
| sqlglot_transpile        | 1.91 ms                                                      | 1.80 ms: 1.06x faster                                            |
| tornado_http             | 124 ms                                                       | 118 ms: 1.05x faster                                             |
| bench_thread_pool        | 1.00 ms                                                      | 953 us: 1.05x faster                                             |
| sqlglot_normalize        | 122 ms                                                       | 116 ms: 1.05x faster                                             |
| meteor_contest           | 131 ms                                                       | 125 ms: 1.05x faster                                             |
| deepcopy                 | 391 us                                                       | 376 us: 1.04x faster                                             |
| tomli_loads              | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                           |
| xml_etree_parse          | 155 ms                                                       | 150 ms: 1.03x faster                                             |
| raytrace                 | 309 ms                                                       | 300 ms: 1.03x faster                                             |
| scimark_monte_carlo      | 69.8 ms                                                      | 67.8 ms: 1.03x faster                                            |
| crypto_pyaes             | 83.3 ms                                                      | 80.9 ms: 1.03x faster                                            |
| sqlglot_optimize         | 59.0 ms                                                      | 57.4 ms: 1.03x faster                                            |
| pycparser                | 1.31 sec                                                     | 1.27 sec: 1.03x faster                                           |
| scimark_sor              | 110 ms                                                       | 107 ms: 1.02x faster                                             |
| pyflate                  | 449 ms                                                       | 439 ms: 1.02x faster                                             |
| pprint_pformat           | 1.67 sec                                                     | 1.63 sec: 1.02x faster                                           |
| regex_v8                 | 24.4 ms                                                      | 23.9 ms: 1.02x faster                                            |
| gc_traversal             | 4.15 ms                                                      | 4.06 ms: 1.02x faster                                            |
| dulwich_log              | 67.4 ms                                                      | 66.1 ms: 1.02x faster                                            |
| spectral_norm            | 95.1 ms                                                      | 93.4 ms: 1.02x faster                                            |
| 2to3                     | 287 ms                                                       | 283 ms: 1.01x faster                                             |
| pprint_safe_repr         | 805 ms                                                       | 799 ms: 1.01x faster                                             |
| docutils                 | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                           |
| unpickle_list            | 4.60 us                                                      | 4.65 us: 1.01x slower                                            |
| pathlib                  | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                            |
| pickle_pure_python       | 316 us                                                       | 326 us: 1.03x slower                                             |
| pidigits                 | 251 ms                                                       | 260 ms: 1.03x slower                                             |
| create_gc_cycles         | 1.58 ms                                                      | 1.64 ms: 1.04x slower                                            |
| telco                    | 6.81 ms                                                      | 7.07 ms: 1.04x slower                                            |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.04x slower                                            |
| pickle_dict              | 32.3 us                                                      | 33.6 us: 1.04x slower                                            |
| regex_effbot             | 3.34 ms                                                      | 3.48 ms: 1.04x slower                                            |
| xml_etree_process        | 55.9 ms                                                      | 58.2 ms: 1.04x slower                                            |
| regex_dna                | 227 ms                                                       | 238 ms: 1.05x slower                                             |
| float                    | 74.9 ms                                                      | 78.8 ms: 1.05x slower                                            |
| python_startup           | 10.7 ms                                                      | 11.4 ms: 1.06x slower                                            |
| xml_etree_generate       | 79.7 ms                                                      | 85.3 ms: 1.07x slower                                            |
| bench_mp_pool            | 4.70 ms                                                      | 5.05 ms: 1.08x slower                                            |
| sqlite_synth             | 2.52 us                                                      | 2.72 us: 1.08x slower                                            |
| unpack_sequence          | 45.7 ns                                                      | 49.4 ns: 1.08x slower                                            |
| scimark_fft              | 281 ms                                                       | 304 ms: 1.08x slower                                             |
| python_startup_no_site   | 7.73 ms                                                      | 8.43 ms: 1.09x slower                                            |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.43 ms: 1.09x slower                                            |
| unpickle                 | 13.3 us                                                      | 14.6 us: 1.10x slower                                            |
| pickle_list              | 3.94 us                                                      | 4.43 us: 1.12x slower                                            |
| async_generators         | 322 ms                                                       | 382 ms: 1.19x slower                                             |
| coverage                 | 66.1 ms                                                      | 89.0 ms: 1.35x slower                                            |
| dask                     | 410 ms                                                       | 562 ms: 1.37x slower                                             |
| Geometric mean           | (ref)                                                        | 1.07x faster                                                     |

Benchmark hidden because not significant (3): xml_etree_iterparse, deepcopy_memo, deepcopy_reduce
Ignored benchmarks (22) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.17x