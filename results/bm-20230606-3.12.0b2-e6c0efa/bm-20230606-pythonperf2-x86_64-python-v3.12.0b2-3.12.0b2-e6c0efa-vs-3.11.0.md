
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b2
- machine: linux-x86_64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.07x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 285 ms: 1.01x faster                                             |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                           |
| tornado_http   | 124 ms                                                       | 121 ms: 1.03x faster                                             |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 546 ms: 1.15x faster                                             |
| async_tree_none         | 518 ms                                                       | 452 ms: 1.15x faster                                             |
| async_tree_io           | 1.17 sec                                                     | 1.04 sec: 1.12x faster                                           |
| async_tree_cpu_io_mixed | 753 ms                                                       | 697 ms: 1.08x faster                                             |
| Geometric mean          | (ref)                                                        | 1.12x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 83.7 ms: 1.11x faster                                            |
| float          | 74.9 ms                                                      | 77.3 ms: 1.03x slower                                            |
| pidigits       | 251 ms                                                       | 259 ms: 1.03x slower                                             |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 144 ms: 1.08x faster                                             |
| regex_v8       | 24.4 ms                                                      | 23.6 ms: 1.03x faster                                            |
| regex_effbot   | 3.34 ms                                                      | 3.55 ms: 1.06x slower                                            |
| regex_dna      | 227 ms                                                       | 245 ms: 1.08x slower                                             |
| Geometric mean | (ref)                                                        | 1.01x slower                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                            |
| json_loads           | 28.9 us                                                      | 24.5 us: 1.18x faster                                            |
| unpickle_pure_python | 238 us                                                       | 205 us: 1.16x faster                                             |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.04x faster                                             |
| pickle_dict          | 32.3 us                                                      | 31.2 us: 1.04x faster                                            |
| xml_etree_iterparse  | 107 ms                                                       | 104 ms: 1.03x faster                                             |
| tomli_loads          | 2.25 sec                                                     | 2.19 sec: 1.03x faster                                           |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                            |
| unpickle_list        | 4.60 us                                                      | 4.71 us: 1.02x slower                                            |
| pickle_pure_python   | 316 us                                                       | 324 us: 1.02x slower                                             |
| xml_etree_process    | 55.9 ms                                                      | 58.8 ms: 1.05x slower                                            |
| xml_etree_generate   | 79.7 ms                                                      | 85.6 ms: 1.07x slower                                            |
| pickle_list          | 3.94 us                                                      | 4.27 us: 1.08x slower                                            |
| unpickle             | 13.3 us                                                      | 14.6 us: 1.10x slower                                            |
| Geometric mean       | (ref)                                                        | 1.03x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.4 ms: 1.06x slower                                            |
| python_startup_no_site | 7.73 ms                                                      | 8.45 ms: 1.09x slower                                            |
| Geometric mean         | (ref)                                                        | 1.08x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 9.93 ms: 1.11x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 532 us                                                       | 150 us: 3.54x faster                                             |
| asyncio_tcp              | 747 ms                                                       | 379 ms: 1.97x faster                                             |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 1.57 sec: 1.96x faster                                           |
| generators               | 54.6 ms                                                      | 35.5 ms: 1.54x faster                                            |
| json_dumps               | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                            |
| richards_super           | 63.6 ms                                                      | 51.0 ms: 1.25x faster                                            |
| coroutines               | 27.8 ms                                                      | 22.3 ms: 1.24x faster                                            |
| deltablue                | 3.97 ms                                                      | 3.25 ms: 1.22x faster                                            |
| fannkuch                 | 416 ms                                                       | 343 ms: 1.21x faster                                             |
| scimark_lu               | 114 ms                                                       | 96.3 ms: 1.18x faster                                            |
| json_loads               | 28.9 us                                                      | 24.5 us: 1.18x faster                                            |
| chaos                    | 74.9 ms                                                      | 63.6 ms: 1.18x faster                                            |
| hexiom                   | 6.98 ms                                                      | 5.95 ms: 1.17x faster                                            |
| unpickle_pure_python     | 238 us                                                       | 205 us: 1.16x faster                                             |
| comprehensions           | 25.1 us                                                      | 21.6 us: 1.16x faster                                            |
| async_tree_memoization   | 629 ms                                                       | 546 ms: 1.15x faster                                             |
| nqueens                  | 103 ms                                                       | 89.5 ms: 1.15x faster                                            |
| async_tree_none          | 518 ms                                                       | 452 ms: 1.15x faster                                             |
| async_tree_io            | 1.17 sec                                                     | 1.04 sec: 1.12x faster                                           |
| nbody                    | 92.9 ms                                                      | 83.7 ms: 1.11x faster                                            |
| mako                     | 11.0 ms                                                      | 9.93 ms: 1.11x faster                                            |
| mdp                      | 2.77 sec                                                     | 2.51 sec: 1.11x faster                                           |
| gc_traversal             | 4.15 ms                                                      | 3.79 ms: 1.09x faster                                            |
| richards                 | 49.7 ms                                                      | 45.5 ms: 1.09x faster                                            |
| sqlglot_parse            | 1.51 ms                                                      | 1.40 ms: 1.09x faster                                            |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 697 ms: 1.08x faster                                             |
| regex_compile            | 156 ms                                                       | 144 ms: 1.08x faster                                             |
| logging_simple           | 7.24 us                                                      | 6.73 us: 1.08x faster                                            |
| go                       | 158 ms                                                       | 147 ms: 1.08x faster                                             |
| json                     | 5.58 ms                                                      | 5.19 ms: 1.08x faster                                            |
| logging_silent           | 100 ns                                                       | 93.8 ns: 1.07x faster                                            |
| sqlglot_transpile        | 1.91 ms                                                      | 1.80 ms: 1.06x faster                                            |
| deepcopy                 | 391 us                                                       | 369 us: 1.06x faster                                             |
| pycparser                | 1.31 sec                                                     | 1.24 sec: 1.05x faster                                           |
| logging_format           | 7.71 us                                                      | 7.35 us: 1.05x faster                                            |
| sqlglot_normalize        | 122 ms                                                       | 116 ms: 1.05x faster                                             |
| deepcopy_memo            | 37.5 us                                                      | 36.0 us: 1.04x faster                                            |
| xml_etree_parse          | 155 ms                                                       | 148 ms: 1.04x faster                                             |
| bench_thread_pool        | 1.00 ms                                                      | 960 us: 1.04x faster                                             |
| spectral_norm            | 95.1 ms                                                      | 91.6 ms: 1.04x faster                                            |
| pickle_dict              | 32.3 us                                                      | 31.2 us: 1.04x faster                                            |
| regex_v8                 | 24.4 ms                                                      | 23.6 ms: 1.03x faster                                            |
| tornado_http             | 124 ms                                                       | 121 ms: 1.03x faster                                             |
| xml_etree_iterparse      | 107 ms                                                       | 104 ms: 1.03x faster                                             |
| tomli_loads              | 2.25 sec                                                     | 2.19 sec: 1.03x faster                                           |
| pprint_pformat           | 1.67 sec                                                     | 1.62 sec: 1.03x faster                                           |
| scimark_sor              | 110 ms                                                       | 107 ms: 1.03x faster                                             |
| crypto_pyaes             | 83.3 ms                                                      | 81.2 ms: 1.03x faster                                            |
| sqlglot_optimize         | 59.0 ms                                                      | 57.5 ms: 1.02x faster                                            |
| meteor_contest           | 131 ms                                                       | 127 ms: 1.02x faster                                             |
| dulwich_log              | 67.4 ms                                                      | 65.9 ms: 1.02x faster                                            |
| pyflate                  | 449 ms                                                       | 441 ms: 1.02x faster                                             |
| pprint_safe_repr         | 805 ms                                                       | 792 ms: 1.02x faster                                             |
| scimark_monte_carlo      | 69.8 ms                                                      | 69.2 ms: 1.01x faster                                            |
| 2to3                     | 287 ms                                                       | 285 ms: 1.01x faster                                             |
| raytrace                 | 309 ms                                                       | 307 ms: 1.01x faster                                             |
| docutils                 | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                           |
| pickle                   | 9.89 us                                                      | 10.0 us: 1.01x slower                                            |
| pathlib                  | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                            |
| unpickle_list            | 4.60 us                                                      | 4.71 us: 1.02x slower                                            |
| pickle_pure_python       | 316 us                                                       | 324 us: 1.02x slower                                             |
| create_gc_cycles         | 1.58 ms                                                      | 1.62 ms: 1.03x slower                                            |
| float                    | 74.9 ms                                                      | 77.3 ms: 1.03x slower                                            |
| pidigits                 | 251 ms                                                       | 259 ms: 1.03x slower                                             |
| telco                    | 6.81 ms                                                      | 7.08 ms: 1.04x slower                                            |
| xml_etree_process        | 55.9 ms                                                      | 58.8 ms: 1.05x slower                                            |
| scimark_fft              | 281 ms                                                       | 296 ms: 1.06x slower                                             |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.29 ms: 1.06x slower                                            |
| regex_effbot             | 3.34 ms                                                      | 3.55 ms: 1.06x slower                                            |
| python_startup           | 10.7 ms                                                      | 11.4 ms: 1.06x slower                                            |
| xml_etree_generate       | 79.7 ms                                                      | 85.6 ms: 1.07x slower                                            |
| sqlite_synth             | 2.52 us                                                      | 2.71 us: 1.08x slower                                            |
| regex_dna                | 227 ms                                                       | 245 ms: 1.08x slower                                             |
| pickle_list              | 3.94 us                                                      | 4.27 us: 1.08x slower                                            |
| unpack_sequence          | 45.7 ns                                                      | 49.8 ns: 1.09x slower                                            |
| python_startup_no_site   | 7.73 ms                                                      | 8.45 ms: 1.09x slower                                            |
| unpickle                 | 13.3 us                                                      | 14.6 us: 1.10x slower                                            |
| bench_mp_pool            | 4.70 ms                                                      | 5.41 ms: 1.15x slower                                            |
| async_generators         | 322 ms                                                       | 389 ms: 1.21x slower                                             |
| coverage                 | 66.1 ms                                                      | 88.5 ms: 1.34x slower                                            |
| dask                     | 410 ms                                                       | 563 ms: 1.37x slower                                             |
| Geometric mean           | (ref)                                                        | 1.07x faster                                                     |

Benchmark hidden because not significant (1): deepcopy_reduce
Ignored benchmarks (22) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.17x