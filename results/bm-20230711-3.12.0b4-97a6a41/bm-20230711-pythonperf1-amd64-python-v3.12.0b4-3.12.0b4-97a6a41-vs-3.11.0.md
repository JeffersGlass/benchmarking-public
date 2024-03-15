
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b4
- machine: windows-amd64
- commit hash: 97a6a41
- commit date: 2023-07-11
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 207 ms: 1.03x faster                                            |
| docutils       | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                          |
| tornado_http   | 92.8 ms                                                     | 86.3 ms: 1.07x faster                                           |
| Geometric mean | (ref)                                                       | 1.04x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 333 ms: 1.20x faster                                            |
| async_tree_none         | 332 ms                                                      | 287 ms: 1.16x faster                                            |
| async_tree_io           | 808 ms                                                      | 709 ms: 1.14x faster                                            |
| async_tree_cpu_io_mixed | 530 ms                                                      | 475 ms: 1.12x faster                                            |
| Geometric mean          | (ref)                                                       | 1.15x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 53.6 ms: 1.01x faster                                           |
| pidigits       | 150 ms                                                      | 150 ms: 1.00x slower                                            |
| nbody          | 70.3 ms                                                     | 74.4 ms: 1.06x slower                                           |
| Geometric mean | (ref)                                                       | 1.02x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.0 ms: 1.09x faster                                           |
| regex_compile  | 91.0 ms                                                     | 87.2 ms: 1.04x faster                                           |
| regex_dna      | 116 ms                                                      | 115 ms: 1.01x faster                                            |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                           |
| Geometric mean | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.50 ms: 1.47x faster                                           |
| unpickle_pure_python | 157 us                                                      | 135 us: 1.16x faster                                            |
| pickle_pure_python   | 208 us                                                      | 195 us: 1.07x faster                                            |
| xml_etree_parse      | 97.6 ms                                                     | 91.5 ms: 1.07x faster                                           |
| tomli_loads          | 1.46 sec                                                    | 1.41 sec: 1.03x faster                                          |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.6 ms: 1.02x faster                                           |
| pickle_dict          | 18.5 us                                                     | 18.4 us: 1.00x faster                                           |
| xml_etree_process    | 37.2 ms                                                     | 37.4 ms: 1.01x slower                                           |
| json_loads           | 13.0 us                                                     | 13.4 us: 1.03x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 55.0 ms: 1.05x slower                                           |
| pickle               | 6.64 us                                                     | 7.05 us: 1.06x slower                                           |
| pickle_list          | 2.70 us                                                     | 2.89 us: 1.07x slower                                           |
| unpickle             | 7.57 us                                                     | 8.23 us: 1.09x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.90 us: 1.12x slower                                           |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 19.1 ms: 1.03x faster                                           |
| python_startup_no_site | 16.8 ms                                                     | 16.4 ms: 1.03x faster                                           |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.86 ms: 1.11x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230711-pythonperf1-amd64-python-v3.12.0b4-3.12.0b4-97a6a41 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 326 us                                                      | 93.3 us: 3.49x faster                                           |
| generators               | 34.0 ms                                                     | 22.2 ms: 1.53x faster                                           |
| asyncio_tcp              | 726 ms                                                      | 474 ms: 1.53x faster                                            |
| json_dumps               | 8.09 ms                                                     | 5.50 ms: 1.47x faster                                           |
| deltablue                | 2.70 ms                                                     | 2.10 ms: 1.28x faster                                           |
| richards_super           | 38.7 ms                                                     | 30.2 ms: 1.28x faster                                           |
| logging_silent           | 71.8 ns                                                     | 59.4 ns: 1.21x faster                                           |
| async_tree_memoization   | 399 ms                                                      | 333 ms: 1.20x faster                                            |
| sqlglot_parse            | 953 us                                                      | 802 us: 1.19x faster                                            |
| richards                 | 31.4 ms                                                     | 26.8 ms: 1.17x faster                                           |
| unpickle_pure_python     | 157 us                                                      | 135 us: 1.16x faster                                            |
| async_tree_none          | 332 ms                                                      | 287 ms: 1.16x faster                                            |
| raytrace                 | 213 ms                                                      | 186 ms: 1.15x faster                                            |
| sqlglot_transpile        | 1.16 ms                                                     | 1.01 ms: 1.15x faster                                           |
| go                       | 101 ms                                                      | 88.2 ms: 1.15x faster                                           |
| async_tree_io            | 808 ms                                                      | 709 ms: 1.14x faster                                            |
| chaos                    | 48.4 ms                                                     | 43.3 ms: 1.12x faster                                           |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 475 ms: 1.12x faster                                            |
| comprehensions           | 15.6 us                                                     | 14.0 us: 1.12x faster                                           |
| nqueens                  | 68.3 ms                                                     | 61.6 ms: 1.11x faster                                           |
| mako                     | 7.58 ms                                                     | 6.86 ms: 1.11x faster                                           |
| dulwich_log              | 46.4 ms                                                     | 42.1 ms: 1.10x faster                                           |
| hexiom                   | 4.55 ms                                                     | 4.14 ms: 1.10x faster                                           |
| scimark_lu               | 62.8 ms                                                     | 57.6 ms: 1.09x faster                                           |
| regex_v8                 | 14.2 ms                                                     | 13.0 ms: 1.09x faster                                           |
| pycparser                | 720 ms                                                      | 667 ms: 1.08x faster                                            |
| tornado_http             | 92.8 ms                                                     | 86.3 ms: 1.07x faster                                           |
| pickle_pure_python       | 208 us                                                      | 195 us: 1.07x faster                                            |
| mdp                      | 1.59 sec                                                    | 1.49 sec: 1.07x faster                                          |
| xml_etree_parse          | 97.6 ms                                                     | 91.5 ms: 1.07x faster                                           |
| coroutines               | 15.0 ms                                                     | 14.0 ms: 1.07x faster                                           |
| deepcopy                 | 246 us                                                      | 231 us: 1.06x faster                                            |
| logging_simple           | 6.86 us                                                     | 6.46 us: 1.06x faster                                           |
| scimark_monte_carlo      | 45.3 ms                                                     | 43.0 ms: 1.05x faster                                           |
| spectral_norm            | 68.3 ms                                                     | 65.1 ms: 1.05x faster                                           |
| pyflate                  | 312 ms                                                      | 298 ms: 1.05x faster                                            |
| unpack_sequence          | 46.9 ns                                                     | 44.7 ns: 1.05x faster                                           |
| sqlglot_normalize        | 190 ms                                                      | 181 ms: 1.05x faster                                            |
| crypto_pyaes             | 48.9 ms                                                     | 46.8 ms: 1.04x faster                                           |
| regex_compile            | 91.0 ms                                                     | 87.2 ms: 1.04x faster                                           |
| deepcopy_memo            | 26.0 us                                                     | 24.9 us: 1.04x faster                                           |
| bench_thread_pool        | 872 us                                                      | 836 us: 1.04x faster                                            |
| aiohttp                  | 883 us                                                      | 849 us: 1.04x faster                                            |
| logging_format           | 7.16 us                                                     | 6.88 us: 1.04x faster                                           |
| pprint_pformat           | 1.09 sec                                                    | 1.05 sec: 1.04x faster                                          |
| python_startup           | 19.8 ms                                                     | 19.1 ms: 1.03x faster                                           |
| tomli_loads              | 1.46 sec                                                    | 1.41 sec: 1.03x faster                                          |
| pprint_safe_repr         | 529 ms                                                      | 514 ms: 1.03x faster                                            |
| 2to3                     | 214 ms                                                      | 207 ms: 1.03x faster                                            |
| python_startup_no_site   | 16.8 ms                                                     | 16.4 ms: 1.03x faster                                           |
| sqlglot_optimize         | 34.5 ms                                                     | 33.7 ms: 1.02x faster                                           |
| fannkuch                 | 253 ms                                                      | 248 ms: 1.02x faster                                            |
| docutils                 | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                          |
| meteor_contest           | 75.2 ms                                                     | 73.8 ms: 1.02x faster                                           |
| scimark_sparse_mat_mult  | 2.58 ms                                                     | 2.53 ms: 1.02x faster                                           |
| xml_etree_iterparse      | 65.6 ms                                                     | 64.6 ms: 1.02x faster                                           |
| float                    | 54.4 ms                                                     | 53.6 ms: 1.01x faster                                           |
| deepcopy_reduce          | 2.06 us                                                     | 2.03 us: 1.01x faster                                           |
| sqlite_synth             | 1.77 us                                                     | 1.75 us: 1.01x faster                                           |
| scimark_fft              | 179 ms                                                      | 177 ms: 1.01x faster                                            |
| regex_dna                | 116 ms                                                      | 115 ms: 1.01x faster                                            |
| pickle_dict              | 18.5 us                                                     | 18.4 us: 1.00x faster                                           |
| pidigits                 | 150 ms                                                      | 150 ms: 1.00x slower                                            |
| xml_etree_process        | 37.2 ms                                                     | 37.4 ms: 1.01x slower                                           |
| telco                    | 4.06 ms                                                     | 4.11 ms: 1.01x slower                                           |
| create_gc_cycles         | 713 us                                                      | 724 us: 1.01x slower                                            |
| json_loads               | 13.0 us                                                     | 13.4 us: 1.03x slower                                           |
| bench_mp_pool            | 63.2 ms                                                     | 65.4 ms: 1.03x slower                                           |
| xml_etree_generate       | 52.5 ms                                                     | 55.0 ms: 1.05x slower                                           |
| regex_effbot             | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                           |
| scimark_sor              | 78.1 ms                                                     | 82.6 ms: 1.06x slower                                           |
| nbody                    | 70.3 ms                                                     | 74.4 ms: 1.06x slower                                           |
| pickle                   | 6.64 us                                                     | 7.05 us: 1.06x slower                                           |
| pickle_list              | 2.70 us                                                     | 2.89 us: 1.07x slower                                           |
| unpickle                 | 7.57 us                                                     | 8.23 us: 1.09x slower                                           |
| pathlib                  | 70.9 ms                                                     | 78.0 ms: 1.10x slower                                           |
| unpickle_list            | 2.59 us                                                     | 2.90 us: 1.12x slower                                           |
| coverage                 | 43.4 ms                                                     | 52.7 ms: 1.21x slower                                           |
| async_generators         | 177 ms                                                      | 230 ms: 1.30x slower                                            |
| dask                     | 273 ms                                                      | 359 ms: 1.32x slower                                            |
| Geometric mean           | (ref)                                                       | 1.07x faster                                                    |

Benchmark hidden because not significant (3): json, gc_traversal, asyncio_tcp_ssl
Ignored benchmarks (19) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown