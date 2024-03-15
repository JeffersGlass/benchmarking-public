
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0rc1
- machine: linux-x86_64
- commit hash: 63bcd91
- commit date: 2023-08-05
- overall geometric mean: 1.01x slower \*
- HPT reliability: 97.05%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 287 ms: 1.01x slower                                               |
| docutils       | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                             |
| Geometric mean | (ref)                                                        | 1.01x slower                                                       |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_io          | 1.04 sec                                                     | 1.06 sec: 1.02x slower                                             |
| async_tree_none        | 452 ms                                                       | 459 ms: 1.02x slower                                               |
| async_tree_memoization | 544 ms                                                       | 554 ms: 1.02x slower                                               |
| Geometric mean         | (ref)                                                        | 1.02x slower                                                       |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 260 ms: 1.02x faster                                               |
| float          | 76.6 ms                                                      | 77.8 ms: 1.02x slower                                              |
| Geometric mean | (ref)                                                        | 1.01x faster                                                       |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.38 ms: 1.06x faster                                              |
| regex_dna      | 239 ms                                                       | 236 ms: 1.01x faster                                               |
| regex_compile  | 144 ms                                                       | 145 ms: 1.01x slower                                               |
| regex_v8       | 23.6 ms                                                      | 24.0 ms: 1.02x slower                                              |
| Geometric mean | (ref)                                                        | 1.01x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|---------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| pickle              | 10.5 us                                                      | 10.0 us: 1.05x faster                                              |
| unpickle            | 14.8 us                                                      | 14.3 us: 1.04x faster                                              |
| pickle_dict         | 32.5 us                                                      | 31.6 us: 1.03x faster                                              |
| xml_etree_generate  | 86.1 ms                                                      | 84.2 ms: 1.02x faster                                              |
| pickle_list         | 4.43 us                                                      | 4.35 us: 1.02x faster                                              |
| json_loads          | 24.4 us                                                      | 24.5 us: 1.00x slower                                              |
| tomli_loads         | 2.16 sec                                                     | 2.18 sec: 1.01x slower                                             |
| xml_etree_iterparse | 103 ms                                                       | 104 ms: 1.02x slower                                               |
| json_dumps          | 10.2 ms                                                      | 10.4 ms: 1.02x slower                                              |
| pickle_pure_python  | 318 us                                                       | 325 us: 1.02x slower                                               |
| xml_etree_parse     | 144 ms                                                       | 149 ms: 1.03x slower                                               |
| Geometric mean      | (ref)                                                        | 1.00x faster                                                       |

Benchmark hidden because not significant (3): unpickle_pure_python, unpickle_list, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.50 ms: 1.02x faster                                              |
| python_startup         | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                              |
| Geometric mean         | (ref)                                                        | 1.02x faster                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-----------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 9.91 ms: 1.01x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_effbot             | 3.57 ms                                                      | 3.38 ms: 1.06x faster                                              |
| pickle                   | 10.5 us                                                      | 10.0 us: 1.05x faster                                              |
| unpickle                 | 14.8 us                                                      | 14.3 us: 1.04x faster                                              |
| pickle_dict              | 32.5 us                                                      | 31.6 us: 1.03x faster                                              |
| generators               | 37.4 ms                                                      | 36.4 ms: 1.03x faster                                              |
| go                       | 150 ms                                                       | 146 ms: 1.03x faster                                               |
| async_generators         | 390 ms                                                       | 380 ms: 1.03x faster                                               |
| sqlite_synth             | 2.77 us                                                      | 2.70 us: 1.03x faster                                              |
| hexiom                   | 5.96 ms                                                      | 5.81 ms: 1.03x faster                                              |
| logging_silent           | 94.4 ns                                                      | 92.1 ns: 1.02x faster                                              |
| xml_etree_generate       | 86.1 ms                                                      | 84.2 ms: 1.02x faster                                              |
| pidigits                 | 265 ms                                                       | 260 ms: 1.02x faster                                               |
| pickle_list              | 4.43 us                                                      | 4.35 us: 1.02x faster                                              |
| python_startup_no_site   | 8.64 ms                                                      | 8.50 ms: 1.02x faster                                              |
| coroutines               | 23.0 ms                                                      | 22.6 ms: 1.02x faster                                              |
| scimark_fft              | 301 ms                                                       | 297 ms: 1.02x faster                                               |
| richards                 | 45.7 ms                                                      | 45.1 ms: 1.01x faster                                              |
| python_startup           | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                              |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                             |
| regex_dna                | 239 ms                                                       | 236 ms: 1.01x faster                                               |
| comprehensions           | 21.9 us                                                      | 21.7 us: 1.01x faster                                              |
| mako                     | 10.0 ms                                                      | 9.91 ms: 1.01x faster                                              |
| scimark_lu               | 98.8 ms                                                      | 98.0 ms: 1.01x faster                                              |
| spectral_norm            | 91.6 ms                                                      | 90.9 ms: 1.01x faster                                              |
| chaos                    | 64.0 ms                                                      | 63.5 ms: 1.01x faster                                              |
| deltablue                | 3.24 ms                                                      | 3.21 ms: 1.01x faster                                              |
| typing_runtime_protocols | 152 us                                                       | 151 us: 1.01x faster                                               |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.19 ms: 1.00x faster                                              |
| mdp                      | 2.57 sec                                                     | 2.56 sec: 1.00x faster                                             |
| pyflate                  | 439 ms                                                       | 437 ms: 1.00x faster                                               |
| meteor_contest           | 128 ms                                                       | 128 ms: 1.00x faster                                               |
| pprint_pformat           | 1.65 sec                                                     | 1.66 sec: 1.00x slower                                             |
| pathlib                  | 18.9 ms                                                      | 19.0 ms: 1.00x slower                                              |
| docutils                 | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                             |
| pprint_safe_repr         | 807 ms                                                       | 811 ms: 1.00x slower                                               |
| json_loads               | 24.4 us                                                      | 24.5 us: 1.00x slower                                              |
| telco                    | 6.96 ms                                                      | 7.01 ms: 1.01x slower                                              |
| regex_compile            | 144 ms                                                       | 145 ms: 1.01x slower                                               |
| raytrace                 | 298 ms                                                       | 300 ms: 1.01x slower                                               |
| 2to3                     | 285 ms                                                       | 287 ms: 1.01x slower                                               |
| tomli_loads              | 2.16 sec                                                     | 2.18 sec: 1.01x slower                                             |
| sqlglot_parse            | 1.38 ms                                                      | 1.39 ms: 1.01x slower                                              |
| dulwich_log              | 65.4 ms                                                      | 66.1 ms: 1.01x slower                                              |
| sqlglot_optimize         | 57.5 ms                                                      | 58.1 ms: 1.01x slower                                              |
| sqlglot_transpile        | 1.78 ms                                                      | 1.80 ms: 1.01x slower                                              |
| richards_super           | 51.3 ms                                                      | 52.1 ms: 1.01x slower                                              |
| regex_v8                 | 23.6 ms                                                      | 24.0 ms: 1.02x slower                                              |
| xml_etree_iterparse      | 103 ms                                                       | 104 ms: 1.02x slower                                               |
| float                    | 76.6 ms                                                      | 77.8 ms: 1.02x slower                                              |
| sqlglot_normalize        | 116 ms                                                       | 118 ms: 1.02x slower                                               |
| logging_simple           | 6.71 us                                                      | 6.82 us: 1.02x slower                                              |
| asyncio_tcp              | 378 ms                                                       | 384 ms: 1.02x slower                                               |
| async_tree_io            | 1.04 sec                                                     | 1.06 sec: 1.02x slower                                             |
| async_tree_none          | 452 ms                                                       | 459 ms: 1.02x slower                                               |
| crypto_pyaes             | 80.3 ms                                                      | 81.8 ms: 1.02x slower                                              |
| json_dumps               | 10.2 ms                                                      | 10.4 ms: 1.02x slower                                              |
| async_tree_memoization   | 544 ms                                                       | 554 ms: 1.02x slower                                               |
| create_gc_cycles         | 1.59 ms                                                      | 1.62 ms: 1.02x slower                                              |
| pickle_pure_python       | 318 us                                                       | 325 us: 1.02x slower                                               |
| fannkuch                 | 350 ms                                                       | 361 ms: 1.03x slower                                               |
| scimark_monte_carlo      | 69.0 ms                                                      | 71.2 ms: 1.03x slower                                              |
| xml_etree_parse          | 144 ms                                                       | 149 ms: 1.03x slower                                               |
| pycparser                | 1.23 sec                                                     | 1.29 sec: 1.04x slower                                             |
| deepcopy_reduce          | 3.37 us                                                      | 3.55 us: 1.05x slower                                              |
| unpack_sequence          | 53.2 ns                                                      | 56.2 ns: 1.06x slower                                              |
| deepcopy                 | 368 us                                                       | 391 us: 1.06x slower                                               |
| gc_traversal             | 3.48 ms                                                      | 3.77 ms: 1.08x slower                                              |
| coverage                 | 66.7 ms                                                      | 87.0 ms: 1.31x slower                                              |
| dask                     | 392 ms                                                       | 566 ms: 1.44x slower                                               |
| Geometric mean           | (ref)                                                        | 1.01x slower                                                       |

Benchmark hidden because not significant (13): nbody, unpickle_pure_python, scimark_sor, nqueens, deepcopy_memo, unpickle_list, json, xml_etree_process, tornado_http, logging_format, async_tree_cpu_io_mixed, bench_thread_pool, bench_mp_pool
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 97.05% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x