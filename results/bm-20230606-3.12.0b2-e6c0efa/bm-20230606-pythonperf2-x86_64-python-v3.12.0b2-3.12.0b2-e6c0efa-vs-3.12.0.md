
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b2
- machine: linux-x86_64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.01x slower \*
- HPT reliability: 60.48%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 285 ms: 1.00x faster                                             |
| docutils       | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                           |
| Geometric mean | (ref)                                                        | 1.00x faster                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io  | 1.04 sec                                                     | 1.04 sec: 1.00x slower                                           |
| Geometric mean | (ref)                                                        | 1.00x slower                                                     |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 83.7 ms: 1.05x faster                                            |
| pidigits       | 265 ms                                                       | 259 ms: 1.02x faster                                             |
| float          | 76.6 ms                                                      | 77.3 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                        | 1.02x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.55 ms: 1.01x faster                                            |
| regex_v8       | 23.6 ms                                                      | 23.6 ms: 1.00x faster                                            |
| regex_compile  | 144 ms                                                       | 144 ms: 1.00x slower                                             |
| regex_dna      | 239 ms                                                       | 245 ms: 1.03x slower                                             |
| Geometric mean | (ref)                                                        | 1.01x slower                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 10.0 us: 1.05x faster                                            |
| pickle_dict          | 32.5 us                                                      | 31.2 us: 1.04x faster                                            |
| pickle_list          | 4.43 us                                                      | 4.27 us: 1.04x faster                                            |
| unpickle_pure_python | 210 us                                                       | 205 us: 1.02x faster                                             |
| unpickle             | 14.8 us                                                      | 14.6 us: 1.01x faster                                            |
| xml_etree_generate   | 86.1 ms                                                      | 85.6 ms: 1.01x faster                                            |
| json_loads           | 24.4 us                                                      | 24.5 us: 1.00x slower                                            |
| xml_etree_process    | 58.4 ms                                                      | 58.8 ms: 1.01x slower                                            |
| unpickle_list        | 4.66 us                                                      | 4.71 us: 1.01x slower                                            |
| tomli_loads          | 2.16 sec                                                     | 2.19 sec: 1.01x slower                                           |
| pickle_pure_python   | 318 us                                                       | 324 us: 1.02x slower                                             |
| xml_etree_parse      | 144 ms                                                       | 148 ms: 1.03x slower                                             |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                     |

Benchmark hidden because not significant (2): json_dumps, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.45 ms: 1.02x faster                                            |
| python_startup         | 11.6 ms                                                      | 11.4 ms: 1.02x faster                                            |
| Geometric mean         | (ref)                                                        | 1.02x faster                                                     |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpack_sequence          | 53.2 ns                                                      | 49.8 ns: 1.07x faster                                            |
| generators               | 37.4 ms                                                      | 35.5 ms: 1.06x faster                                            |
| nbody                    | 88.0 ms                                                      | 83.7 ms: 1.05x faster                                            |
| pickle                   | 10.5 us                                                      | 10.0 us: 1.05x faster                                            |
| pickle_dict              | 32.5 us                                                      | 31.2 us: 1.04x faster                                            |
| pickle_list              | 4.43 us                                                      | 4.27 us: 1.04x faster                                            |
| coroutines               | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                            |
| scimark_lu               | 98.8 ms                                                      | 96.3 ms: 1.03x faster                                            |
| mdp                      | 2.57 sec                                                     | 2.51 sec: 1.02x faster                                           |
| unpickle_pure_python     | 210 us                                                       | 205 us: 1.02x faster                                             |
| sqlite_synth             | 2.77 us                                                      | 2.71 us: 1.02x faster                                            |
| deepcopy_memo            | 36.8 us                                                      | 36.0 us: 1.02x faster                                            |
| python_startup_no_site   | 8.64 ms                                                      | 8.45 ms: 1.02x faster                                            |
| pidigits                 | 265 ms                                                       | 259 ms: 1.02x faster                                             |
| go                       | 150 ms                                                       | 147 ms: 1.02x faster                                             |
| fannkuch                 | 350 ms                                                       | 343 ms: 1.02x faster                                             |
| pprint_pformat           | 1.65 sec                                                     | 1.62 sec: 1.02x faster                                           |
| scimark_sor              | 109 ms                                                       | 107 ms: 1.02x faster                                             |
| pprint_safe_repr         | 807 ms                                                       | 792 ms: 1.02x faster                                             |
| logging_format           | 7.48 us                                                      | 7.35 us: 1.02x faster                                            |
| python_startup           | 11.6 ms                                                      | 11.4 ms: 1.02x faster                                            |
| comprehensions           | 21.9 us                                                      | 21.6 us: 1.02x faster                                            |
| scimark_fft              | 301 ms                                                       | 296 ms: 1.02x faster                                             |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                           |
| unpickle                 | 14.8 us                                                      | 14.6 us: 1.01x faster                                            |
| typing_runtime_protocols | 152 us                                                       | 150 us: 1.01x faster                                             |
| logging_silent           | 94.4 ns                                                      | 93.8 ns: 1.01x faster                                            |
| richards_super           | 51.3 ms                                                      | 51.0 ms: 1.01x faster                                            |
| xml_etree_generate       | 86.1 ms                                                      | 85.6 ms: 1.01x faster                                            |
| regex_effbot             | 3.57 ms                                                      | 3.55 ms: 1.01x faster                                            |
| meteor_contest           | 128 ms                                                       | 127 ms: 1.01x faster                                             |
| nqueens                  | 89.9 ms                                                      | 89.5 ms: 1.00x faster                                            |
| 2to3                     | 285 ms                                                       | 285 ms: 1.00x faster                                             |
| regex_v8                 | 23.6 ms                                                      | 23.6 ms: 1.00x faster                                            |
| docutils                 | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                           |
| async_tree_io            | 1.04 sec                                                     | 1.04 sec: 1.00x slower                                           |
| regex_compile            | 144 ms                                                       | 144 ms: 1.00x slower                                             |
| scimark_monte_carlo      | 69.0 ms                                                      | 69.2 ms: 1.00x slower                                            |
| json_loads               | 24.4 us                                                      | 24.5 us: 1.00x slower                                            |
| pyflate                  | 439 ms                                                       | 441 ms: 1.01x slower                                             |
| xml_etree_process        | 58.4 ms                                                      | 58.8 ms: 1.01x slower                                            |
| dulwich_log              | 65.4 ms                                                      | 65.9 ms: 1.01x slower                                            |
| float                    | 76.6 ms                                                      | 77.3 ms: 1.01x slower                                            |
| deepcopy_reduce          | 3.37 us                                                      | 3.40 us: 1.01x slower                                            |
| unpickle_list            | 4.66 us                                                      | 4.71 us: 1.01x slower                                            |
| crypto_pyaes             | 80.3 ms                                                      | 81.2 ms: 1.01x slower                                            |
| sqlglot_transpile        | 1.78 ms                                                      | 1.80 ms: 1.01x slower                                            |
| tomli_loads              | 2.16 sec                                                     | 2.19 sec: 1.01x slower                                           |
| sqlglot_parse            | 1.38 ms                                                      | 1.40 ms: 1.01x slower                                            |
| json                     | 5.12 ms                                                      | 5.19 ms: 1.01x slower                                            |
| telco                    | 6.96 ms                                                      | 7.08 ms: 1.02x slower                                            |
| pickle_pure_python       | 318 us                                                       | 324 us: 1.02x slower                                             |
| create_gc_cycles         | 1.59 ms                                                      | 1.62 ms: 1.02x slower                                            |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.29 ms: 1.02x slower                                            |
| pathlib                  | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                            |
| regex_dna                | 239 ms                                                       | 245 ms: 1.03x slower                                             |
| xml_etree_parse          | 144 ms                                                       | 148 ms: 1.03x slower                                             |
| raytrace                 | 298 ms                                                       | 307 ms: 1.03x slower                                             |
| gc_traversal             | 3.48 ms                                                      | 3.79 ms: 1.09x slower                                            |
| bench_mp_pool            | 4.76 ms                                                      | 5.41 ms: 1.14x slower                                            |
| coverage                 | 66.7 ms                                                      | 88.5 ms: 1.33x slower                                            |
| dask                     | 392 ms                                                       | 563 ms: 1.44x slower                                             |
| Geometric mean           | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (20): mako, chaos, richards, tornado_http, async_generators, hexiom, json_dumps, spectral_norm, async_tree_cpu_io_mixed, async_tree_none, sqlglot_optimize, deepcopy, asyncio_tcp, logging_simple, sqlglot_normalize, deltablue, async_tree_memoization, pycparser, xml_etree_iterparse, bench_thread_pool
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 60.48% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x