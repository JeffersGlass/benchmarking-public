
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b1
- machine: windows-amd64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.04x faster \*
- HPT reliability: 97.83%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 218 ms: 1.02x slower                                            |
| docutils       | 1.64 sec                                                    | 1.67 sec: 1.02x slower                                          |
| tornado_http   | 92.8 ms                                                     | 98.2 ms: 1.06x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x slower                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 351 ms: 1.14x faster                                            |
| async_tree_none         | 332 ms                                                      | 309 ms: 1.07x faster                                            |
| async_tree_cpu_io_mixed | 530 ms                                                      | 494 ms: 1.07x faster                                            |
| async_tree_io           | 808 ms                                                      | 765 ms: 1.06x faster                                            |
| Geometric mean          | (ref)                                                       | 1.08x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 69.0 ms: 1.02x faster                                           |
| pidigits       | 150 ms                                                      | 153 ms: 1.02x slower                                            |
| float          | 54.4 ms                                                     | 56.5 ms: 1.04x slower                                           |
| Geometric mean | (ref)                                                       | 1.01x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 89.3 ms: 1.02x faster                                           |
| regex_v8       | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                           |
| regex_dna      | 116 ms                                                      | 126 ms: 1.08x slower                                            |
| regex_effbot   | 1.50 ms                                                     | 1.62 ms: 1.08x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.68 ms: 1.42x faster                                           |
| unpickle_pure_python | 157 us                                                      | 137 us: 1.14x faster                                            |
| pickle_pure_python   | 208 us                                                      | 196 us: 1.06x faster                                            |
| tomli_loads          | 1.46 sec                                                    | 1.39 sec: 1.05x faster                                          |
| xml_etree_parse      | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 66.2 ms: 1.01x slower                                           |
| xml_etree_process    | 37.2 ms                                                     | 38.6 ms: 1.04x slower                                           |
| pickle_dict          | 18.5 us                                                     | 19.2 us: 1.04x slower                                           |
| pickle               | 6.64 us                                                     | 7.00 us: 1.05x slower                                           |
| pickle_list          | 2.70 us                                                     | 2.86 us: 1.06x slower                                           |
| json_loads           | 13.0 us                                                     | 13.8 us: 1.06x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 56.6 ms: 1.08x slower                                           |
| unpickle             | 7.57 us                                                     | 8.47 us: 1.12x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.92 us: 1.13x slower                                           |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.8 ms: 1.05x slower                                           |
| python_startup_no_site | 16.8 ms                                                     | 17.8 ms: 1.06x slower                                           |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.24 ms: 1.05x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230522-pythonperf1-amd64-python-v3.12.0b1-3.12.0b1-5612078 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 326 us                                                      | 94.7 us: 3.44x faster                                           |
| generators               | 34.0 ms                                                     | 23.0 ms: 1.48x faster                                           |
| json_dumps               | 8.09 ms                                                     | 5.68 ms: 1.42x faster                                           |
| richards_super           | 38.7 ms                                                     | 29.1 ms: 1.33x faster                                           |
| richards                 | 31.4 ms                                                     | 25.5 ms: 1.23x faster                                           |
| deltablue                | 2.70 ms                                                     | 2.20 ms: 1.23x faster                                           |
| unpack_sequence          | 46.9 ns                                                     | 38.7 ns: 1.21x faster                                           |
| logging_silent           | 71.8 ns                                                     | 60.1 ns: 1.19x faster                                           |
| sqlglot_parse            | 953 us                                                      | 800 us: 1.19x faster                                            |
| go                       | 101 ms                                                      | 88.2 ms: 1.15x faster                                           |
| sqlglot_transpile        | 1.16 ms                                                     | 1.02 ms: 1.14x faster                                           |
| unpickle_pure_python     | 157 us                                                      | 137 us: 1.14x faster                                            |
| mdp                      | 1.59 sec                                                    | 1.40 sec: 1.14x faster                                          |
| async_tree_memoization   | 399 ms                                                      | 351 ms: 1.14x faster                                            |
| hexiom                   | 4.55 ms                                                     | 4.09 ms: 1.11x faster                                           |
| raytrace                 | 213 ms                                                      | 192 ms: 1.11x faster                                            |
| nqueens                  | 68.3 ms                                                     | 61.6 ms: 1.11x faster                                           |
| deepcopy_memo            | 26.0 us                                                     | 23.7 us: 1.09x faster                                           |
| chaos                    | 48.4 ms                                                     | 44.3 ms: 1.09x faster                                           |
| comprehensions           | 15.6 us                                                     | 14.4 us: 1.08x faster                                           |
| async_tree_none          | 332 ms                                                      | 309 ms: 1.07x faster                                            |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 494 ms: 1.07x faster                                            |
| pickle_pure_python       | 208 us                                                      | 196 us: 1.06x faster                                            |
| asyncio_tcp              | 726 ms                                                      | 686 ms: 1.06x faster                                            |
| scimark_monte_carlo      | 45.3 ms                                                     | 42.9 ms: 1.06x faster                                           |
| async_tree_io            | 808 ms                                                      | 765 ms: 1.06x faster                                            |
| tomli_loads              | 1.46 sec                                                    | 1.39 sec: 1.05x faster                                          |
| mako                     | 7.58 ms                                                     | 7.24 ms: 1.05x faster                                           |
| scimark_lu               | 62.8 ms                                                     | 60.0 ms: 1.05x faster                                           |
| pyflate                  | 312 ms                                                      | 298 ms: 1.05x faster                                            |
| deepcopy                 | 246 us                                                      | 236 us: 1.05x faster                                            |
| xml_etree_parse          | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                           |
| coroutines               | 15.0 ms                                                     | 14.4 ms: 1.04x faster                                           |
| spectral_norm            | 68.3 ms                                                     | 66.3 ms: 1.03x faster                                           |
| fannkuch                 | 253 ms                                                      | 246 ms: 1.03x faster                                            |
| crypto_pyaes             | 48.9 ms                                                     | 47.4 ms: 1.03x faster                                           |
| pprint_pformat           | 1.09 sec                                                    | 1.06 sec: 1.03x faster                                          |
| pycparser                | 720 ms                                                      | 700 ms: 1.03x faster                                            |
| pprint_safe_repr         | 529 ms                                                      | 517 ms: 1.02x faster                                            |
| dulwich_log              | 46.4 ms                                                     | 45.3 ms: 1.02x faster                                           |
| scimark_sparse_mat_mult  | 2.58 ms                                                     | 2.52 ms: 1.02x faster                                           |
| regex_compile            | 91.0 ms                                                     | 89.3 ms: 1.02x faster                                           |
| nbody                    | 70.3 ms                                                     | 69.0 ms: 1.02x faster                                           |
| regex_v8                 | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                           |
| sqlglot_normalize        | 190 ms                                                      | 187 ms: 1.02x faster                                            |
| logging_simple           | 6.86 us                                                     | 6.77 us: 1.01x faster                                           |
| xml_etree_iterparse      | 65.6 ms                                                     | 66.2 ms: 1.01x slower                                           |
| sqlite_synth             | 1.77 us                                                     | 1.78 us: 1.01x slower                                           |
| sqlglot_optimize         | 34.5 ms                                                     | 35.0 ms: 1.01x slower                                           |
| logging_format           | 7.16 us                                                     | 7.28 us: 1.02x slower                                           |
| docutils                 | 1.64 sec                                                    | 1.67 sec: 1.02x slower                                          |
| deepcopy_reduce          | 2.06 us                                                     | 2.10 us: 1.02x slower                                           |
| 2to3                     | 214 ms                                                      | 218 ms: 1.02x slower                                            |
| pidigits                 | 150 ms                                                      | 153 ms: 1.02x slower                                            |
| bench_thread_pool        | 872 us                                                      | 895 us: 1.03x slower                                            |
| gc_traversal             | 1.49 ms                                                     | 1.53 ms: 1.03x slower                                           |
| scimark_sor              | 78.1 ms                                                     | 80.6 ms: 1.03x slower                                           |
| xml_etree_process        | 37.2 ms                                                     | 38.6 ms: 1.04x slower                                           |
| float                    | 54.4 ms                                                     | 56.5 ms: 1.04x slower                                           |
| pickle_dict              | 18.5 us                                                     | 19.2 us: 1.04x slower                                           |
| telco                    | 4.06 ms                                                     | 4.23 ms: 1.04x slower                                           |
| aiohttp                  | 883 us                                                      | 928 us: 1.05x slower                                            |
| python_startup           | 19.8 ms                                                     | 20.8 ms: 1.05x slower                                           |
| pickle                   | 6.64 us                                                     | 7.00 us: 1.05x slower                                           |
| python_startup_no_site   | 16.8 ms                                                     | 17.8 ms: 1.06x slower                                           |
| tornado_http             | 92.8 ms                                                     | 98.2 ms: 1.06x slower                                           |
| pickle_list              | 2.70 us                                                     | 2.86 us: 1.06x slower                                           |
| json_loads               | 13.0 us                                                     | 13.8 us: 1.06x slower                                           |
| create_gc_cycles         | 713 us                                                      | 766 us: 1.07x slower                                            |
| xml_etree_generate       | 52.5 ms                                                     | 56.6 ms: 1.08x slower                                           |
| regex_dna                | 116 ms                                                      | 126 ms: 1.08x slower                                            |
| regex_effbot             | 1.50 ms                                                     | 1.62 ms: 1.08x slower                                           |
| bench_mp_pool            | 63.2 ms                                                     | 70.0 ms: 1.11x slower                                           |
| unpickle                 | 7.57 us                                                     | 8.47 us: 1.12x slower                                           |
| unpickle_list            | 2.59 us                                                     | 2.92 us: 1.13x slower                                           |
| coverage                 | 43.4 ms                                                     | 50.9 ms: 1.17x slower                                           |
| asyncio_tcp_ssl          | 2.03 sec                                                    | 2.39 sec: 1.18x slower                                          |
| pathlib                  | 70.9 ms                                                     | 85.4 ms: 1.21x slower                                           |
| async_generators         | 177 ms                                                      | 237 ms: 1.34x slower                                            |
| dask                     | 273 ms                                                      | 382 ms: 1.40x slower                                            |
| Geometric mean           | (ref)                                                       | 1.04x faster                                                    |

Benchmark hidden because not significant (3): scimark_fft, meteor_contest, json
Ignored benchmarks (19) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 97.83% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown