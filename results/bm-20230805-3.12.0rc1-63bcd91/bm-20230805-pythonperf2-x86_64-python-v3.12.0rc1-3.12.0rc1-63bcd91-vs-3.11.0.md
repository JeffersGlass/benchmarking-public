
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0rc1
- machine: linux-x86_64
- commit hash: 63bcd91
- commit date: 2023-08-05
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.89%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.16x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 287 ms: 1.00x slower                                               |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                             |
| tornado_http   | 124 ms                                                       | 122 ms: 1.02x faster                                               |
| Geometric mean | (ref)                                                        | 1.00x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 554 ms: 1.13x faster                                               |
| async_tree_none         | 518 ms                                                       | 459 ms: 1.13x faster                                               |
| async_tree_io           | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                             |
| async_tree_cpu_io_mixed | 753 ms                                                       | 703 ms: 1.07x faster                                               |
| Geometric mean          | (ref)                                                        | 1.11x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 86.7 ms: 1.07x faster                                              |
| pidigits       | 251 ms                                                       | 260 ms: 1.03x slower                                               |
| float          | 74.9 ms                                                      | 77.8 ms: 1.04x slower                                              |
| Geometric mean | (ref)                                                        | 1.00x slower                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 145 ms: 1.08x faster                                               |
| regex_v8       | 24.4 ms                                                      | 24.0 ms: 1.02x faster                                              |
| regex_effbot   | 3.34 ms                                                      | 3.38 ms: 1.01x slower                                              |
| regex_dna      | 227 ms                                                       | 236 ms: 1.04x slower                                               |
| Geometric mean | (ref)                                                        | 1.01x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.4 ms: 1.27x faster                                              |
| json_loads           | 28.9 us                                                      | 24.5 us: 1.18x faster                                              |
| unpickle_pure_python | 238 us                                                       | 209 us: 1.14x faster                                               |
| xml_etree_parse      | 155 ms                                                       | 149 ms: 1.04x faster                                               |
| tomli_loads          | 2.25 sec                                                     | 2.18 sec: 1.03x faster                                             |
| pickle_dict          | 32.3 us                                                      | 31.6 us: 1.02x faster                                              |
| xml_etree_iterparse  | 107 ms                                                       | 104 ms: 1.02x faster                                               |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                              |
| unpickle_list        | 4.60 us                                                      | 4.67 us: 1.01x slower                                              |
| pickle_pure_python   | 316 us                                                       | 325 us: 1.03x slower                                               |
| xml_etree_process    | 55.9 ms                                                      | 58.6 ms: 1.05x slower                                              |
| xml_etree_generate   | 79.7 ms                                                      | 84.2 ms: 1.06x slower                                              |
| unpickle             | 13.3 us                                                      | 14.3 us: 1.08x slower                                              |
| pickle_list          | 3.94 us                                                      | 4.35 us: 1.10x slower                                              |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                       |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                              |
| python_startup_no_site | 7.73 ms                                                      | 8.50 ms: 1.10x slower                                              |
| Geometric mean         | (ref)                                                        | 1.08x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|-----------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 9.91 ms: 1.11x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230805-pythonperf2-x86_64-python-v3.12.0rc1-3.12.0rc1-63bcd91 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols | 532 us                                                       | 151 us: 3.53x faster                                               |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                             |
| asyncio_tcp              | 747 ms                                                       | 384 ms: 1.94x faster                                               |
| generators               | 54.6 ms                                                      | 36.4 ms: 1.50x faster                                              |
| json_dumps               | 13.3 ms                                                      | 10.4 ms: 1.27x faster                                              |
| deltablue                | 3.97 ms                                                      | 3.21 ms: 1.23x faster                                              |
| coroutines               | 27.8 ms                                                      | 22.6 ms: 1.23x faster                                              |
| richards_super           | 63.6 ms                                                      | 52.1 ms: 1.22x faster                                              |
| hexiom                   | 6.98 ms                                                      | 5.81 ms: 1.20x faster                                              |
| json_loads               | 28.9 us                                                      | 24.5 us: 1.18x faster                                              |
| chaos                    | 74.9 ms                                                      | 63.5 ms: 1.18x faster                                              |
| scimark_lu               | 114 ms                                                       | 98.0 ms: 1.16x faster                                              |
| comprehensions           | 25.1 us                                                      | 21.7 us: 1.15x faster                                              |
| fannkuch                 | 416 ms                                                       | 361 ms: 1.15x faster                                               |
| nqueens                  | 103 ms                                                       | 89.9 ms: 1.14x faster                                              |
| unpickle_pure_python     | 238 us                                                       | 209 us: 1.14x faster                                               |
| async_tree_memoization   | 629 ms                                                       | 554 ms: 1.13x faster                                               |
| async_tree_none          | 518 ms                                                       | 459 ms: 1.13x faster                                               |
| mako                     | 11.0 ms                                                      | 9.91 ms: 1.11x faster                                              |
| async_tree_io            | 1.17 sec                                                     | 1.06 sec: 1.11x faster                                             |
| richards                 | 49.7 ms                                                      | 45.1 ms: 1.10x faster                                              |
| gc_traversal             | 4.15 ms                                                      | 3.77 ms: 1.10x faster                                              |
| logging_silent           | 100 ns                                                       | 92.1 ns: 1.09x faster                                              |
| sqlglot_parse            | 1.51 ms                                                      | 1.39 ms: 1.09x faster                                              |
| json                     | 5.58 ms                                                      | 5.13 ms: 1.09x faster                                              |
| go                       | 158 ms                                                       | 146 ms: 1.08x faster                                               |
| mdp                      | 2.77 sec                                                     | 2.56 sec: 1.08x faster                                             |
| regex_compile            | 156 ms                                                       | 145 ms: 1.08x faster                                               |
| nbody                    | 92.9 ms                                                      | 86.7 ms: 1.07x faster                                              |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 703 ms: 1.07x faster                                               |
| logging_simple           | 7.24 us                                                      | 6.82 us: 1.06x faster                                              |
| sqlglot_transpile        | 1.91 ms                                                      | 1.80 ms: 1.06x faster                                              |
| spectral_norm            | 95.1 ms                                                      | 90.9 ms: 1.05x faster                                              |
| xml_etree_parse          | 155 ms                                                       | 149 ms: 1.04x faster                                               |
| bench_thread_pool        | 1.00 ms                                                      | 966 us: 1.04x faster                                               |
| sqlglot_normalize        | 122 ms                                                       | 118 ms: 1.04x faster                                               |
| tomli_loads              | 2.25 sec                                                     | 2.18 sec: 1.03x faster                                             |
| raytrace                 | 309 ms                                                       | 300 ms: 1.03x faster                                               |
| pyflate                  | 449 ms                                                       | 437 ms: 1.03x faster                                               |
| logging_format           | 7.71 us                                                      | 7.52 us: 1.02x faster                                              |
| pickle_dict              | 32.3 us                                                      | 31.6 us: 1.02x faster                                              |
| xml_etree_iterparse      | 107 ms                                                       | 104 ms: 1.02x faster                                               |
| meteor_contest           | 131 ms                                                       | 128 ms: 1.02x faster                                               |
| tornado_http             | 124 ms                                                       | 122 ms: 1.02x faster                                               |
| dulwich_log              | 67.4 ms                                                      | 66.1 ms: 1.02x faster                                              |
| deepcopy_memo            | 37.5 us                                                      | 36.8 us: 1.02x faster                                              |
| crypto_pyaes             | 83.3 ms                                                      | 81.8 ms: 1.02x faster                                              |
| regex_v8                 | 24.4 ms                                                      | 24.0 ms: 1.02x faster                                              |
| pycparser                | 1.31 sec                                                     | 1.29 sec: 1.01x faster                                             |
| sqlglot_optimize         | 59.0 ms                                                      | 58.1 ms: 1.01x faster                                              |
| scimark_sor              | 110 ms                                                       | 109 ms: 1.01x faster                                               |
| pprint_pformat           | 1.67 sec                                                     | 1.66 sec: 1.01x faster                                             |
| 2to3                     | 287 ms                                                       | 287 ms: 1.00x slower                                               |
| pprint_safe_repr         | 805 ms                                                       | 811 ms: 1.01x slower                                               |
| docutils                 | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                             |
| regex_effbot             | 3.34 ms                                                      | 3.38 ms: 1.01x slower                                              |
| pickle                   | 9.89 us                                                      | 10.0 us: 1.01x slower                                              |
| unpickle_list            | 4.60 us                                                      | 4.67 us: 1.01x slower                                              |
| scimark_monte_carlo      | 69.8 ms                                                      | 71.2 ms: 1.02x slower                                              |
| pickle_pure_python       | 316 us                                                       | 325 us: 1.03x slower                                               |
| create_gc_cycles         | 1.58 ms                                                      | 1.62 ms: 1.03x slower                                              |
| telco                    | 6.81 ms                                                      | 7.01 ms: 1.03x slower                                              |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.19 ms: 1.03x slower                                              |
| pidigits                 | 251 ms                                                       | 260 ms: 1.03x slower                                               |
| float                    | 74.9 ms                                                      | 77.8 ms: 1.04x slower                                              |
| regex_dna                | 227 ms                                                       | 236 ms: 1.04x slower                                               |
| deepcopy_reduce          | 3.40 us                                                      | 3.55 us: 1.05x slower                                              |
| xml_etree_process        | 55.9 ms                                                      | 58.6 ms: 1.05x slower                                              |
| xml_etree_generate       | 79.7 ms                                                      | 84.2 ms: 1.06x slower                                              |
| scimark_fft              | 281 ms                                                       | 297 ms: 1.06x slower                                               |
| python_startup           | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                              |
| sqlite_synth             | 2.52 us                                                      | 2.70 us: 1.07x slower                                              |
| unpickle                 | 13.3 us                                                      | 14.3 us: 1.08x slower                                              |
| python_startup_no_site   | 7.73 ms                                                      | 8.50 ms: 1.10x slower                                              |
| pickle_list              | 3.94 us                                                      | 4.35 us: 1.10x slower                                              |
| async_generators         | 322 ms                                                       | 380 ms: 1.18x slower                                               |
| unpack_sequence          | 45.7 ns                                                      | 56.2 ns: 1.23x slower                                              |
| coverage                 | 66.1 ms                                                      | 87.0 ms: 1.32x slower                                              |
| dask                     | 410 ms                                                       | 566 ms: 1.38x slower                                               |
| Geometric mean           | (ref)                                                        | 1.06x faster                                                       |

Benchmark hidden because not significant (3): deepcopy, pathlib, bench_mp_pool
Ignored benchmarks (22) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 99.89% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.16x