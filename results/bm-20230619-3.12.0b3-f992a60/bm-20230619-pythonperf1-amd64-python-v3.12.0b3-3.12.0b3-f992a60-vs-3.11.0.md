
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b3
- machine: windows-amd64
- commit hash: f992a60
- commit date: 2023-06-19
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 217 ms: 1.01x slower                                            |
| docutils       | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                          |
| tornado_http   | 92.8 ms                                                     | 90.2 ms: 1.03x faster                                           |
| Geometric mean | (ref)                                                       | 1.00x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none         | 332 ms                                                      | 292 ms: 1.14x faster                                            |
| async_tree_memoization  | 399 ms                                                      | 352 ms: 1.13x faster                                            |
| async_tree_io           | 808 ms                                                      | 744 ms: 1.09x faster                                            |
| async_tree_cpu_io_mixed | 530 ms                                                      | 493 ms: 1.07x faster                                            |
| Geometric mean          | (ref)                                                       | 1.11x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 67.6 ms: 1.04x faster                                           |
| pidigits       | 150 ms                                                      | 154 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                       | 1.01x faster                                                    |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 87.5 ms: 1.04x faster                                           |
| regex_v8       | 14.2 ms                                                     | 14.0 ms: 1.01x faster                                           |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                            |
| regex_effbot   | 1.50 ms                                                     | 1.61 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                       | 1.02x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.79 ms: 1.40x faster                                           |
| unpickle_pure_python | 157 us                                                      | 132 us: 1.19x faster                                            |
| pickle_pure_python   | 208 us                                                      | 194 us: 1.07x faster                                            |
| xml_etree_parse      | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                           |
| tomli_loads          | 1.46 sec                                                    | 1.38 sec: 1.05x faster                                          |
| pickle_dict          | 18.5 us                                                     | 18.1 us: 1.02x faster                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.6 ms: 1.02x faster                                           |
| xml_etree_process    | 37.2 ms                                                     | 38.1 ms: 1.03x slower                                           |
| pickle               | 6.64 us                                                     | 6.86 us: 1.03x slower                                           |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                           |
| pickle_list          | 2.70 us                                                     | 2.84 us: 1.05x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 56.2 ms: 1.07x slower                                           |
| unpickle             | 7.57 us                                                     | 8.28 us: 1.09x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.83 us: 1.10x slower                                           |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 17.1 ms: 1.02x slower                                           |
| python_startup         | 19.8 ms                                                     | 20.4 ms: 1.03x slower                                           |
| Geometric mean         | (ref)                                                       | 1.02x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.88 ms: 1.10x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230619-pythonperf1-amd64-python-v3.12.0b3-3.12.0b3-f992a60 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 326 us                                                      | 94.6 us: 3.45x faster                                           |
| generators               | 34.0 ms                                                     | 22.0 ms: 1.54x faster                                           |
| asyncio_tcp              | 726 ms                                                      | 498 ms: 1.46x faster                                            |
| json_dumps               | 8.09 ms                                                     | 5.79 ms: 1.40x faster                                           |
| deltablue                | 2.70 ms                                                     | 2.07 ms: 1.30x faster                                           |
| richards_super           | 38.7 ms                                                     | 29.7 ms: 1.30x faster                                           |
| logging_silent           | 71.8 ns                                                     | 59.3 ns: 1.21x faster                                           |
| unpack_sequence          | 46.9 ns                                                     | 38.8 ns: 1.21x faster                                           |
| richards                 | 31.4 ms                                                     | 26.1 ms: 1.21x faster                                           |
| sqlglot_parse            | 953 us                                                      | 802 us: 1.19x faster                                            |
| unpickle_pure_python     | 157 us                                                      | 132 us: 1.19x faster                                            |
| raytrace                 | 213 ms                                                      | 184 ms: 1.16x faster                                            |
| sqlglot_transpile        | 1.16 ms                                                     | 1.01 ms: 1.15x faster                                           |
| go                       | 101 ms                                                      | 88.3 ms: 1.15x faster                                           |
| hexiom                   | 4.55 ms                                                     | 3.99 ms: 1.14x faster                                           |
| async_tree_none          | 332 ms                                                      | 292 ms: 1.14x faster                                            |
| async_tree_memoization   | 399 ms                                                      | 352 ms: 1.13x faster                                            |
| chaos                    | 48.4 ms                                                     | 42.8 ms: 1.13x faster                                           |
| comprehensions           | 15.6 us                                                     | 14.0 us: 1.12x faster                                           |
| nqueens                  | 68.3 ms                                                     | 61.1 ms: 1.12x faster                                           |
| deepcopy_memo            | 26.0 us                                                     | 23.3 us: 1.11x faster                                           |
| mdp                      | 1.59 sec                                                    | 1.43 sec: 1.11x faster                                          |
| scimark_lu               | 62.8 ms                                                     | 56.6 ms: 1.11x faster                                           |
| mako                     | 7.58 ms                                                     | 6.88 ms: 1.10x faster                                           |
| async_tree_io            | 808 ms                                                      | 744 ms: 1.09x faster                                            |
| pickle_pure_python       | 208 us                                                      | 194 us: 1.07x faster                                            |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 493 ms: 1.07x faster                                            |
| coroutines               | 15.0 ms                                                     | 14.0 ms: 1.07x faster                                           |
| logging_simple           | 6.86 us                                                     | 6.44 us: 1.07x faster                                           |
| scimark_monte_carlo      | 45.3 ms                                                     | 42.6 ms: 1.06x faster                                           |
| spectral_norm            | 68.3 ms                                                     | 64.6 ms: 1.06x faster                                           |
| deepcopy                 | 246 us                                                      | 234 us: 1.05x faster                                            |
| xml_etree_parse          | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                           |
| tomli_loads              | 1.46 sec                                                    | 1.38 sec: 1.05x faster                                          |
| pyflate                  | 312 ms                                                      | 297 ms: 1.05x faster                                            |
| dulwich_log              | 46.4 ms                                                     | 44.1 ms: 1.05x faster                                           |
| pprint_pformat           | 1.09 sec                                                    | 1.04 sec: 1.05x faster                                          |
| scimark_sparse_mat_mult  | 2.58 ms                                                     | 2.47 ms: 1.04x faster                                           |
| fannkuch                 | 253 ms                                                      | 243 ms: 1.04x faster                                            |
| regex_compile            | 91.0 ms                                                     | 87.5 ms: 1.04x faster                                           |
| nbody                    | 70.3 ms                                                     | 67.6 ms: 1.04x faster                                           |
| logging_format           | 7.16 us                                                     | 6.91 us: 1.04x faster                                           |
| pprint_safe_repr         | 529 ms                                                      | 511 ms: 1.03x faster                                            |
| sqlglot_normalize        | 190 ms                                                      | 184 ms: 1.03x faster                                            |
| pycparser                | 720 ms                                                      | 699 ms: 1.03x faster                                            |
| tornado_http             | 92.8 ms                                                     | 90.2 ms: 1.03x faster                                           |
| scimark_fft              | 179 ms                                                      | 175 ms: 1.03x faster                                            |
| crypto_pyaes             | 48.9 ms                                                     | 47.6 ms: 1.03x faster                                           |
| pickle_dict              | 18.5 us                                                     | 18.1 us: 1.02x faster                                           |
| sqlglot_optimize         | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                           |
| meteor_contest           | 75.2 ms                                                     | 73.9 ms: 1.02x faster                                           |
| xml_etree_iterparse      | 65.6 ms                                                     | 64.6 ms: 1.02x faster                                           |
| regex_v8                 | 14.2 ms                                                     | 14.0 ms: 1.01x faster                                           |
| docutils                 | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                          |
| telco                    | 4.06 ms                                                     | 4.11 ms: 1.01x slower                                           |
| 2to3                     | 214 ms                                                      | 217 ms: 1.01x slower                                            |
| python_startup_no_site   | 16.8 ms                                                     | 17.1 ms: 1.02x slower                                           |
| xml_etree_process        | 37.2 ms                                                     | 38.1 ms: 1.03x slower                                           |
| pidigits                 | 150 ms                                                      | 154 ms: 1.03x slower                                            |
| gc_traversal             | 1.49 ms                                                     | 1.53 ms: 1.03x slower                                           |
| python_startup           | 19.8 ms                                                     | 20.4 ms: 1.03x slower                                           |
| pickle                   | 6.64 us                                                     | 6.86 us: 1.03x slower                                           |
| json_loads               | 13.0 us                                                     | 13.5 us: 1.04x slower                                           |
| create_gc_cycles         | 713 us                                                      | 744 us: 1.04x slower                                            |
| regex_dna                | 116 ms                                                      | 122 ms: 1.05x slower                                            |
| sqlite_synth             | 1.77 us                                                     | 1.86 us: 1.05x slower                                           |
| pickle_list              | 2.70 us                                                     | 2.84 us: 1.05x slower                                           |
| xml_etree_generate       | 52.5 ms                                                     | 56.2 ms: 1.07x slower                                           |
| regex_effbot             | 1.50 ms                                                     | 1.61 ms: 1.07x slower                                           |
| bench_mp_pool            | 63.2 ms                                                     | 67.9 ms: 1.07x slower                                           |
| unpickle                 | 7.57 us                                                     | 8.28 us: 1.09x slower                                           |
| unpickle_list            | 2.59 us                                                     | 2.83 us: 1.10x slower                                           |
| pathlib                  | 70.9 ms                                                     | 82.8 ms: 1.17x slower                                           |
| coverage                 | 43.4 ms                                                     | 52.8 ms: 1.22x slower                                           |
| async_generators         | 177 ms                                                      | 234 ms: 1.32x slower                                            |
| dask                     | 273 ms                                                      | 370 ms: 1.36x slower                                            |
| Geometric mean           | (ref)                                                       | 1.06x faster                                                    |

Benchmark hidden because not significant (7): float, bench_thread_pool, scimark_sor, aiohttp, deepcopy_reduce, json, asyncio_tcp_ssl
Ignored benchmarks (19) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown