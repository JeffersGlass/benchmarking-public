# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: 8915762
- commit date: 2024-01-20
- overall geometric mean: 1.00x faster
- HPT reliability: 50.72%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 241 ms                                                                          | 252 ms: 1.04x slower                                                                      |
| chameleon      | 5.80 ms                                                                         | 5.67 ms: 1.02x faster                                                                     |
| docutils       | 1.79 sec                                                                        | 1.83 sec: 1.02x slower                                                                    |
| Geometric mean | (ref)                                                                           | 1.01x slower                                                                              |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 502 ms                                                                          | 493 ms: 1.02x faster                                                                      |
| async_tree_cpu_io_mixed    | 511 ms                                                                          | 505 ms: 1.01x faster                                                                      |
| async_tree_none_tg         | 237 ms                                                                          | 235 ms: 1.01x faster                                                                      |
| Geometric mean             | (ref)                                                                           | 1.01x faster                                                                              |

Benchmark hidden because not significant (5): async_tree_io, async_tree_io_tg, async_tree_memoization_tg, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| float          | 59.3 ms                                                                         | 56.2 ms: 1.05x faster                                                                     |
| nbody          | 86.8 ms                                                                         | 85.9 ms: 1.01x faster                                                                     |
| pidigits       | 199 ms                                                                          | 198 ms: 1.00x faster                                                                      |
| Geometric mean | (ref)                                                                           | 1.02x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_dna      | 121 ms                                                                          | 117 ms: 1.04x faster                                                                      |
| regex_compile  | 104 ms                                                                          | 107 ms: 1.03x slower                                                                      |
| Geometric mean | (ref)                                                                           | 1.00x faster                                                                              |

Benchmark hidden because not significant (2): regex_effbot, regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_list        | 2.99 us                                                                         | 2.83 us: 1.05x faster                                                                     |
| unpickle             | 10.1 us                                                                         | 9.55 us: 1.05x faster                                                                     |
| unpickle_pure_python | 156 us                                                                          | 149 us: 1.04x faster                                                                      |
| pickle_list          | 3.31 us                                                                         | 3.25 us: 1.02x faster                                                                     |
| tomli_loads          | 1.65 sec                                                                        | 1.62 sec: 1.02x faster                                                                    |
| xml_etree_parse      | 111 ms                                                                          | 109 ms: 1.02x faster                                                                      |
| json_dumps           | 6.72 ms                                                                         | 6.64 ms: 1.01x faster                                                                     |
| pickle_pure_python   | 210 us                                                                          | 209 us: 1.01x faster                                                                      |
| json_loads           | 19.8 us                                                                         | 19.9 us: 1.00x slower                                                                     |
| pickle_dict          | 20.0 us                                                                         | 20.2 us: 1.01x slower                                                                     |
| xml_etree_process    | 41.2 ms                                                                         | 41.9 ms: 1.02x slower                                                                     |
| Geometric mean       | (ref)                                                                           | 1.01x faster                                                                              |

Benchmark hidden because not significant (3): pickle, xml_etree_generate, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 23.3 ms                                                                         | 22.7 ms: 1.03x faster                                                                     |
| python_startup_no_site | 21.0 ms                                                                         | 20.6 ms: 1.02x faster                                                                     |
| Geometric mean         | (ref)                                                                           | 1.02x faster                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-----------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 7.77 ms                                                                         | 7.74 ms: 1.00x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| scimark_fft                | 231 ms                                                                          | 207 ms: 1.12x faster                                                                      |
| spectral_norm              | 89.4 ms                                                                         | 79.8 ms: 1.12x faster                                                                     |
| scimark_monte_carlo        | 52.5 ms                                                                         | 49.6 ms: 1.06x faster                                                                     |
| mdp                        | 1.80 sec                                                                        | 1.71 sec: 1.06x faster                                                                    |
| unpickle_list              | 2.99 us                                                                         | 2.83 us: 1.05x faster                                                                     |
| float                      | 59.3 ms                                                                         | 56.2 ms: 1.05x faster                                                                     |
| unpickle                   | 10.1 us                                                                         | 9.55 us: 1.05x faster                                                                     |
| deltablue                  | 2.81 ms                                                                         | 2.67 ms: 1.05x faster                                                                     |
| unpickle_pure_python       | 156 us                                                                          | 149 us: 1.04x faster                                                                      |
| regex_dna                  | 121 ms                                                                          | 117 ms: 1.04x faster                                                                      |
| python_startup             | 23.3 ms                                                                         | 22.7 ms: 1.03x faster                                                                     |
| sqlite_synth               | 1.91 us                                                                         | 1.86 us: 1.03x faster                                                                     |
| scimark_sparse_mat_mult    | 3.37 ms                                                                         | 3.28 ms: 1.03x faster                                                                     |
| fannkuch                   | 294 ms                                                                          | 288 ms: 1.02x faster                                                                      |
| chameleon                  | 5.80 ms                                                                         | 5.67 ms: 1.02x faster                                                                     |
| python_startup_no_site     | 21.0 ms                                                                         | 20.6 ms: 1.02x faster                                                                     |
| chaos                      | 53.6 ms                                                                         | 52.5 ms: 1.02x faster                                                                     |
| pickle_list                | 3.31 us                                                                         | 3.25 us: 1.02x faster                                                                     |
| async_tree_cpu_io_mixed_tg | 502 ms                                                                          | 493 ms: 1.02x faster                                                                      |
| tomli_loads                | 1.65 sec                                                                        | 1.62 sec: 1.02x faster                                                                    |
| xml_etree_parse            | 111 ms                                                                          | 109 ms: 1.02x faster                                                                      |
| hexiom                     | 5.29 ms                                                                         | 5.21 ms: 1.02x faster                                                                     |
| create_gc_cycles           | 651 us                                                                          | 642 us: 1.01x faster                                                                      |
| async_tree_cpu_io_mixed    | 511 ms                                                                          | 505 ms: 1.01x faster                                                                      |
| pyflate                    | 337 ms                                                                          | 333 ms: 1.01x faster                                                                      |
| bench_mp_pool              | 75.8 ms                                                                         | 74.9 ms: 1.01x faster                                                                     |
| scimark_lu                 | 62.7 ms                                                                         | 62.0 ms: 1.01x faster                                                                     |
| json_dumps                 | 6.72 ms                                                                         | 6.64 ms: 1.01x faster                                                                     |
| nbody                      | 86.8 ms                                                                         | 85.9 ms: 1.01x faster                                                                     |
| meteor_contest             | 78.8 ms                                                                         | 78.1 ms: 1.01x faster                                                                     |
| async_generators           | 272 ms                                                                          | 270 ms: 1.01x faster                                                                      |
| async_tree_none_tg         | 237 ms                                                                          | 235 ms: 1.01x faster                                                                      |
| pickle_pure_python         | 210 us                                                                          | 209 us: 1.01x faster                                                                      |
| mako                       | 7.77 ms                                                                         | 7.74 ms: 1.00x faster                                                                     |
| comprehensions             | 13.6 us                                                                         | 13.5 us: 1.00x faster                                                                     |
| pidigits                   | 199 ms                                                                          | 198 ms: 1.00x faster                                                                      |
| pathlib                    | 87.7 ms                                                                         | 88.1 ms: 1.00x slower                                                                     |
| logging_silent             | 60.1 ns                                                                         | 60.4 ns: 1.00x slower                                                                     |
| json_loads                 | 19.8 us                                                                         | 19.9 us: 1.00x slower                                                                     |
| crypto_pyaes               | 55.4 ms                                                                         | 55.7 ms: 1.01x slower                                                                     |
| sympy_str                  | 212 ms                                                                          | 213 ms: 1.01x slower                                                                      |
| json                       | 4.07 ms                                                                         | 4.10 ms: 1.01x slower                                                                     |
| gc_traversal               | 1.39 ms                                                                         | 1.41 ms: 1.01x slower                                                                     |
| pickle_dict                | 20.0 us                                                                         | 20.2 us: 1.01x slower                                                                     |
| nqueens                    | 77.1 ms                                                                         | 77.8 ms: 1.01x slower                                                                     |
| sympy_integrate            | 15.2 ms                                                                         | 15.4 ms: 1.01x slower                                                                     |
| dask                       | 303 ms                                                                          | 307 ms: 1.01x slower                                                                      |
| scimark_sor                | 81.2 ms                                                                         | 82.1 ms: 1.01x slower                                                                     |
| logging_format             | 8.60 us                                                                         | 8.71 us: 1.01x slower                                                                     |
| sqlglot_parse              | 900 us                                                                          | 913 us: 1.01x slower                                                                      |
| logging_simple             | 7.94 us                                                                         | 8.06 us: 1.02x slower                                                                     |
| raytrace                   | 207 ms                                                                          | 211 ms: 1.02x slower                                                                      |
| xml_etree_process          | 41.2 ms                                                                         | 41.9 ms: 1.02x slower                                                                     |
| sympy_sum                  | 107 ms                                                                          | 109 ms: 1.02x slower                                                                      |
| typing_runtime_protocols   | 90.3 us                                                                         | 92.3 us: 1.02x slower                                                                     |
| pprint_safe_repr           | 585 ms                                                                          | 599 ms: 1.02x slower                                                                      |
| richards_super             | 32.5 ms                                                                         | 33.3 ms: 1.02x slower                                                                     |
| docutils                   | 1.79 sec                                                                        | 1.83 sec: 1.02x slower                                                                    |
| regex_compile              | 104 ms                                                                          | 107 ms: 1.03x slower                                                                      |
| richards                   | 28.8 ms                                                                         | 29.6 ms: 1.03x slower                                                                     |
| sqlglot_transpile          | 1.14 ms                                                                         | 1.17 ms: 1.03x slower                                                                     |
| coroutines                 | 14.3 ms                                                                         | 14.7 ms: 1.03x slower                                                                     |
| sympy_expand               | 365 ms                                                                          | 376 ms: 1.03x slower                                                                      |
| coverage                   | 474 ms                                                                          | 487 ms: 1.03x slower                                                                      |
| generators                 | 23.3 ms                                                                         | 24.0 ms: 1.03x slower                                                                     |
| pycparser                  | 812 ms                                                                          | 837 ms: 1.03x slower                                                                      |
| unpack_sequence            | 40.3 ns                                                                         | 41.6 ns: 1.03x slower                                                                     |
| deepcopy_reduce            | 2.41 us                                                                         | 2.49 us: 1.03x slower                                                                     |
| sqlglot_optimize           | 40.4 ms                                                                         | 41.8 ms: 1.04x slower                                                                     |
| pprint_pformat             | 1.19 sec                                                                        | 1.24 sec: 1.04x slower                                                                    |
| deepcopy_memo              | 24.1 us                                                                         | 25.1 us: 1.04x slower                                                                     |
| 2to3                       | 241 ms                                                                          | 252 ms: 1.04x slower                                                                      |
| sqlglot_normalize          | 207 ms                                                                          | 216 ms: 1.05x slower                                                                      |
| deepcopy                   | 266 us                                                                          | 279 us: 1.05x slower                                                                      |
| telco                      | 5.65 ms                                                                         | 6.14 ms: 1.09x slower                                                                     |
| Geometric mean             | (ref)                                                                           | 1.00x faster                                                                              |

Benchmark hidden because not significant (15): bench_thread_pool, asyncio_tcp, tornado_http, regex_effbot, pickle, async_tree_io, async_tree_io_tg, async_tree_memoization_tg, xml_etree_generate, regex_v8, async_tree_memoization, xml_etree_iterparse, go, asyncio_tcp_ssl, async_tree_none


# HPT report

- Reliability score: 50.72% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown