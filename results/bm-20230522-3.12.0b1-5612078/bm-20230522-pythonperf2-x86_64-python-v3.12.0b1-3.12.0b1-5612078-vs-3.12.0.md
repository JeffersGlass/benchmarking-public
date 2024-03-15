
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b1
- machine: linux-x86_64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.01x slower \*
- HPT reliability: 71.60%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 284 ms: 1.01x faster                                             |
| tornado_http   | 121 ms                                                       | 115 ms: 1.05x faster                                             |
| Geometric mean | (ref)                                                        | 1.02x faster                                                     |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io  | 1.04 sec                                                     | 1.05 sec: 1.00x slower                                           |
| Geometric mean | (ref)                                                        | 1.00x slower                                                     |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 88.0 ms                                                      | 84.7 ms: 1.04x faster                                            |
| pidigits       | 265 ms                                                       | 261 ms: 1.02x faster                                             |
| float          | 76.6 ms                                                      | 78.6 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_v8       | 23.6 ms                                                      | 22.8 ms: 1.03x faster                                            |
| regex_effbot   | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                            |
| regex_dna      | 239 ms                                                       | 237 ms: 1.00x faster                                             |
| regex_compile  | 144 ms                                                       | 143 ms: 1.00x faster                                             |
| Geometric mean | (ref)                                                        | 1.02x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 10.1 us: 1.05x faster                                            |
| unpickle_pure_python | 210 us                                                       | 204 us: 1.03x faster                                             |
| unpickle             | 14.8 us                                                      | 14.4 us: 1.02x faster                                            |
| tomli_loads          | 2.16 sec                                                     | 2.12 sec: 1.02x faster                                           |
| pickle_list          | 4.43 us                                                      | 4.37 us: 1.01x faster                                            |
| json_dumps           | 10.2 ms                                                      | 10.2 ms: 1.01x faster                                            |
| json_loads           | 24.4 us                                                      | 24.2 us: 1.01x faster                                            |
| xml_etree_generate   | 86.1 ms                                                      | 86.8 ms: 1.01x slower                                            |
| xml_etree_process    | 58.4 ms                                                      | 59.0 ms: 1.01x slower                                            |
| unpickle_list        | 4.66 us                                                      | 4.72 us: 1.01x slower                                            |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                             |
| pickle_dict          | 32.5 us                                                      | 33.2 us: 1.02x slower                                            |
| pickle_pure_python   | 318 us                                                       | 325 us: 1.02x slower                                             |
| xml_etree_iterparse  | 103 ms                                                       | 106 ms: 1.03x slower                                             |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.50 ms: 1.02x faster                                            |
| python_startup         | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                            |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230522-pythonperf2-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| unpack_sequence          | 53.2 ns                                                      | 48.1 ns: 1.11x faster                                            |
| generators               | 37.4 ms                                                      | 35.1 ms: 1.07x faster                                            |
| tornado_http             | 121 ms                                                       | 115 ms: 1.05x faster                                             |
| logging_format           | 7.48 us                                                      | 7.14 us: 1.05x faster                                            |
| pickle                   | 10.5 us                                                      | 10.1 us: 1.05x faster                                            |
| nbody                    | 88.0 ms                                                      | 84.7 ms: 1.04x faster                                            |
| sqlite_synth             | 2.77 us                                                      | 2.68 us: 1.04x faster                                            |
| regex_v8                 | 23.6 ms                                                      | 22.8 ms: 1.03x faster                                            |
| coroutines               | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                            |
| async_generators         | 390 ms                                                       | 379 ms: 1.03x faster                                             |
| unpickle_pure_python     | 210 us                                                       | 204 us: 1.03x faster                                             |
| unpickle                 | 14.8 us                                                      | 14.4 us: 1.02x faster                                            |
| regex_effbot             | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                            |
| typing_runtime_protocols | 152 us                                                       | 149 us: 1.02x faster                                             |
| tomli_loads              | 2.16 sec                                                     | 2.12 sec: 1.02x faster                                           |
| logging_simple           | 6.71 us                                                      | 6.60 us: 1.02x faster                                            |
| mdp                      | 2.57 sec                                                     | 2.53 sec: 1.02x faster                                           |
| comprehensions           | 21.9 us                                                      | 21.6 us: 1.02x faster                                            |
| python_startup_no_site   | 8.64 ms                                                      | 8.50 ms: 1.02x faster                                            |
| richards                 | 45.7 ms                                                      | 45.0 ms: 1.02x faster                                            |
| pidigits                 | 265 ms                                                       | 261 ms: 1.02x faster                                             |
| logging_silent           | 94.4 ns                                                      | 93.0 ns: 1.01x faster                                            |
| pickle_list              | 4.43 us                                                      | 4.37 us: 1.01x faster                                            |
| go                       | 150 ms                                                       | 148 ms: 1.01x faster                                             |
| hexiom                   | 5.96 ms                                                      | 5.88 ms: 1.01x faster                                            |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                           |
| scimark_monte_carlo      | 69.0 ms                                                      | 68.2 ms: 1.01x faster                                            |
| python_startup           | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                            |
| sqlglot_normalize        | 116 ms                                                       | 115 ms: 1.01x faster                                             |
| scimark_lu               | 98.8 ms                                                      | 98.0 ms: 1.01x faster                                            |
| meteor_contest           | 128 ms                                                       | 127 ms: 1.01x faster                                             |
| deepcopy_memo            | 36.8 us                                                      | 36.5 us: 1.01x faster                                            |
| json_dumps               | 10.2 ms                                                      | 10.2 ms: 1.01x faster                                            |
| json_loads               | 24.4 us                                                      | 24.2 us: 1.01x faster                                            |
| sqlglot_optimize         | 57.5 ms                                                      | 57.2 ms: 1.01x faster                                            |
| deltablue                | 3.24 ms                                                      | 3.22 ms: 1.01x faster                                            |
| 2to3                     | 285 ms                                                       | 284 ms: 1.01x faster                                             |
| regex_dna                | 239 ms                                                       | 237 ms: 1.00x faster                                             |
| raytrace                 | 298 ms                                                       | 297 ms: 1.00x faster                                             |
| regex_compile            | 144 ms                                                       | 143 ms: 1.00x faster                                             |
| async_tree_io            | 1.04 sec                                                     | 1.05 sec: 1.00x slower                                           |
| nqueens                  | 89.9 ms                                                      | 90.2 ms: 1.00x slower                                            |
| asyncio_tcp              | 378 ms                                                       | 380 ms: 1.00x slower                                             |
| deepcopy                 | 368 us                                                       | 370 us: 1.00x slower                                             |
| sqlglot_transpile        | 1.78 ms                                                      | 1.79 ms: 1.01x slower                                            |
| xml_etree_generate       | 86.1 ms                                                      | 86.8 ms: 1.01x slower                                            |
| json                     | 5.12 ms                                                      | 5.16 ms: 1.01x slower                                            |
| pyflate                  | 439 ms                                                       | 443 ms: 1.01x slower                                             |
| xml_etree_process        | 58.4 ms                                                      | 59.0 ms: 1.01x slower                                            |
| dulwich_log              | 65.4 ms                                                      | 66.1 ms: 1.01x slower                                            |
| scimark_fft              | 301 ms                                                       | 305 ms: 1.01x slower                                             |
| unpickle_list            | 4.66 us                                                      | 4.72 us: 1.01x slower                                            |
| fannkuch                 | 350 ms                                                       | 355 ms: 1.01x slower                                             |
| xml_etree_parse          | 144 ms                                                       | 147 ms: 1.02x slower                                             |
| pathlib                  | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                            |
| pickle_dict              | 32.5 us                                                      | 33.2 us: 1.02x slower                                            |
| pickle_pure_python       | 318 us                                                       | 325 us: 1.02x slower                                             |
| telco                    | 6.96 ms                                                      | 7.11 ms: 1.02x slower                                            |
| pycparser                | 1.23 sec                                                     | 1.27 sec: 1.03x slower                                           |
| float                    | 76.6 ms                                                      | 78.6 ms: 1.03x slower                                            |
| crypto_pyaes             | 80.3 ms                                                      | 82.5 ms: 1.03x slower                                            |
| xml_etree_iterparse      | 103 ms                                                       | 106 ms: 1.03x slower                                             |
| spectral_norm            | 91.6 ms                                                      | 94.5 ms: 1.03x slower                                            |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.38 ms: 1.04x slower                                            |
| create_gc_cycles         | 1.59 ms                                                      | 1.68 ms: 1.05x slower                                            |
| gc_traversal             | 3.48 ms                                                      | 3.79 ms: 1.09x slower                                            |
| coverage                 | 66.7 ms                                                      | 88.0 ms: 1.32x slower                                            |
| dask                     | 392 ms                                                       | 551 ms: 1.41x slower                                             |
| bench_mp_pool            | 4.76 ms                                                      | 8.65 ms: 1.82x slower                                            |
| Geometric mean           | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (13): bench_thread_pool, mako, richards_super, pprint_pformat, async_tree_cpu_io_mixed, async_tree_memoization, deepcopy_reduce, chaos, scimark_sor, docutils, pprint_safe_repr, async_tree_none, sqlglot_parse
Ignored benchmarks (16) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 71.60% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x