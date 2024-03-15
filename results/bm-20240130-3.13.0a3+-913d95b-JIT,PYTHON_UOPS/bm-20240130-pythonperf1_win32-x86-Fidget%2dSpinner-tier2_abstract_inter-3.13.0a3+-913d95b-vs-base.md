# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.01x slower
- HPT reliability: 96.25%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 259 ms                                                                          | 268 ms: 1.03x slower                                                                      |
| chameleon      | 6.08 ms                                                                         | 6.17 ms: 1.02x slower                                                                     |
| docutils       | 1.88 sec                                                                        | 1.86 sec: 1.01x faster                                                                    |
| tornado_http   | 100 ms                                                                          | 103 ms: 1.02x slower                                                                      |
| Geometric mean | (ref)                                                                           | 1.01x slower                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_io           | 645 ms                                                                          | 634 ms: 1.02x faster                                                                      |
| async_tree_cpu_io_mixed | 532 ms                                                                          | 527 ms: 1.01x faster                                                                      |
| async_tree_none_tg      | 251 ms                                                                          | 253 ms: 1.01x slower                                                                      |
| async_tree_io_tg        | 617 ms                                                                          | 625 ms: 1.01x slower                                                                      |
| Geometric mean          | (ref)                                                                           | 1.00x faster                                                                              |

Benchmark hidden because not significant (4): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| pidigits       | 203 ms                                                                          | 201 ms: 1.01x faster                                                                      |
| Geometric mean | (ref)                                                                           | 1.01x faster                                                                              |

Benchmark hidden because not significant (2): nbody, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_dna      | 124 ms                                                                          | 122 ms: 1.01x faster                                                                      |
| regex_effbot   | 1.92 ms                                                                         | 1.91 ms: 1.01x faster                                                                     |
| regex_compile  | 109 ms                                                                          | 113 ms: 1.03x slower                                                                      |
| Geometric mean | (ref)                                                                           | 1.00x slower                                                                              |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_list        | 3.10 us                                                                         | 2.79 us: 1.11x faster                                                                     |
| xml_etree_parse      | 111 ms                                                                          | 104 ms: 1.06x faster                                                                      |
| xml_etree_iterparse  | 69.0 ms                                                                         | 67.2 ms: 1.03x faster                                                                     |
| unpickle             | 10.3 us                                                                         | 10.1 us: 1.02x faster                                                                     |
| xml_etree_process    | 43.2 ms                                                                         | 42.8 ms: 1.01x faster                                                                     |
| unpickle_pure_python | 159 us                                                                          | 157 us: 1.01x faster                                                                      |
| tomli_loads          | 1.62 sec                                                                        | 1.64 sec: 1.01x slower                                                                    |
| xml_etree_generate   | 61.1 ms                                                                         | 62.3 ms: 1.02x slower                                                                     |
| json_loads           | 19.7 us                                                                         | 20.1 us: 1.02x slower                                                                     |
| pickle_pure_python   | 220 us                                                                          | 227 us: 1.03x slower                                                                      |
| pickle_dict          | 19.8 us                                                                         | 20.5 us: 1.03x slower                                                                     |
| pickle_list          | 3.17 us                                                                         | 3.31 us: 1.04x slower                                                                     |
| json_dumps           | 6.73 ms                                                                         | 7.14 ms: 1.06x slower                                                                     |
| Geometric mean       | (ref)                                                                           | 1.00x slower                                                                              |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup_no_site | 21.0 ms                                                                         | 21.1 ms: 1.01x slower                                                                     |
| python_startup         | 23.1 ms                                                                         | 23.6 ms: 1.02x slower                                                                     |
| Geometric mean         | (ref)                                                                           | 1.01x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 7.92 ms                                                                         | 8.01 ms: 1.01x slower                                                                     |

All benchmarks:
===============

| Benchmark                | bm-20240129-pythonperf1_win32-x86-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_list            | 3.10 us                                                                         | 2.79 us: 1.11x faster                                                                     |
| xml_etree_parse          | 111 ms                                                                          | 104 ms: 1.06x faster                                                                      |
| asyncio_tcp              | 650 ms                                                                          | 622 ms: 1.05x faster                                                                      |
| bench_thread_pool        | 1.10 ms                                                                         | 1.07 ms: 1.03x faster                                                                     |
| telco                    | 6.64 ms                                                                         | 6.44 ms: 1.03x faster                                                                     |
| chaos                    | 59.5 ms                                                                         | 58.0 ms: 1.03x faster                                                                     |
| xml_etree_iterparse      | 69.0 ms                                                                         | 67.2 ms: 1.03x faster                                                                     |
| deepcopy_reduce          | 2.51 us                                                                         | 2.45 us: 1.02x faster                                                                     |
| deepcopy_memo            | 26.6 us                                                                         | 26.1 us: 1.02x faster                                                                     |
| unpickle                 | 10.3 us                                                                         | 10.1 us: 1.02x faster                                                                     |
| logging_silent           | 67.4 ns                                                                         | 66.3 ns: 1.02x faster                                                                     |
| mdp                      | 1.90 sec                                                                        | 1.87 sec: 1.02x faster                                                                    |
| async_tree_io            | 645 ms                                                                          | 634 ms: 1.02x faster                                                                      |
| deepcopy                 | 288 us                                                                          | 284 us: 1.01x faster                                                                      |
| dask                     | 315 ms                                                                          | 311 ms: 1.01x faster                                                                      |
| docutils                 | 1.88 sec                                                                        | 1.86 sec: 1.01x faster                                                                    |
| sqlite_synth             | 1.88 us                                                                         | 1.86 us: 1.01x faster                                                                     |
| regex_dna                | 124 ms                                                                          | 122 ms: 1.01x faster                                                                      |
| scimark_sparse_mat_mult  | 3.27 ms                                                                         | 3.23 ms: 1.01x faster                                                                     |
| gc_traversal             | 1.43 ms                                                                         | 1.41 ms: 1.01x faster                                                                     |
| pidigits                 | 203 ms                                                                          | 201 ms: 1.01x faster                                                                      |
| async_tree_cpu_io_mixed  | 532 ms                                                                          | 527 ms: 1.01x faster                                                                      |
| xml_etree_process        | 43.2 ms                                                                         | 42.8 ms: 1.01x faster                                                                     |
| regex_effbot             | 1.92 ms                                                                         | 1.91 ms: 1.01x faster                                                                     |
| richards                 | 31.3 ms                                                                         | 31.1 ms: 1.01x faster                                                                     |
| unpickle_pure_python     | 159 us                                                                          | 157 us: 1.01x faster                                                                      |
| sqlglot_parse            | 971 us                                                                          | 965 us: 1.01x faster                                                                      |
| scimark_monte_carlo      | 70.6 ms                                                                         | 70.3 ms: 1.00x faster                                                                     |
| generators               | 24.8 ms                                                                         | 25.0 ms: 1.01x slower                                                                     |
| go                       | 121 ms                                                                          | 122 ms: 1.01x slower                                                                      |
| python_startup_no_site   | 21.0 ms                                                                         | 21.1 ms: 1.01x slower                                                                     |
| coroutines               | 15.0 ms                                                                         | 15.2 ms: 1.01x slower                                                                     |
| async_tree_none_tg       | 251 ms                                                                          | 253 ms: 1.01x slower                                                                      |
| mako                     | 7.92 ms                                                                         | 8.01 ms: 1.01x slower                                                                     |
| pycparser                | 859 ms                                                                          | 869 ms: 1.01x slower                                                                      |
| tomli_loads              | 1.62 sec                                                                        | 1.64 sec: 1.01x slower                                                                    |
| async_tree_io_tg         | 617 ms                                                                          | 625 ms: 1.01x slower                                                                      |
| sympy_str                | 218 ms                                                                          | 221 ms: 1.01x slower                                                                      |
| logging_format           | 8.89 us                                                                         | 9.01 us: 1.01x slower                                                                     |
| coverage                 | 476 ms                                                                          | 483 ms: 1.01x slower                                                                      |
| bench_mp_pool            | 75.3 ms                                                                         | 76.3 ms: 1.01x slower                                                                     |
| nqueens                  | 88.3 ms                                                                         | 89.6 ms: 1.01x slower                                                                     |
| sqlglot_optimize         | 43.7 ms                                                                         | 44.3 ms: 1.01x slower                                                                     |
| sympy_expand             | 372 ms                                                                          | 378 ms: 1.02x slower                                                                      |
| scimark_lu               | 67.6 ms                                                                         | 68.7 ms: 1.02x slower                                                                     |
| chameleon                | 6.08 ms                                                                         | 6.17 ms: 1.02x slower                                                                     |
| pyflate                  | 376 ms                                                                          | 383 ms: 1.02x slower                                                                      |
| python_startup           | 23.1 ms                                                                         | 23.6 ms: 1.02x slower                                                                     |
| deltablue                | 2.57 ms                                                                         | 2.62 ms: 1.02x slower                                                                     |
| xml_etree_generate       | 61.1 ms                                                                         | 62.3 ms: 1.02x slower                                                                     |
| json_loads               | 19.7 us                                                                         | 20.1 us: 1.02x slower                                                                     |
| fannkuch                 | 304 ms                                                                          | 310 ms: 1.02x slower                                                                      |
| scimark_fft              | 251 ms                                                                          | 257 ms: 1.02x slower                                                                      |
| tornado_http             | 100 ms                                                                          | 103 ms: 1.02x slower                                                                      |
| create_gc_cycles         | 652 us                                                                          | 668 us: 1.03x slower                                                                      |
| unpack_sequence          | 40.8 ns                                                                         | 41.9 ns: 1.03x slower                                                                     |
| crypto_pyaes             | 62.9 ms                                                                         | 64.7 ms: 1.03x slower                                                                     |
| regex_compile            | 109 ms                                                                          | 113 ms: 1.03x slower                                                                      |
| typing_runtime_protocols | 94.9 us                                                                         | 97.9 us: 1.03x slower                                                                     |
| pickle_pure_python       | 220 us                                                                          | 227 us: 1.03x slower                                                                      |
| pickle_dict              | 19.8 us                                                                         | 20.5 us: 1.03x slower                                                                     |
| scimark_sor              | 90.2 ms                                                                         | 93.2 ms: 1.03x slower                                                                     |
| 2to3                     | 259 ms                                                                          | 268 ms: 1.03x slower                                                                      |
| sympy_sum                | 111 ms                                                                          | 116 ms: 1.04x slower                                                                      |
| pickle_list              | 3.17 us                                                                         | 3.31 us: 1.04x slower                                                                     |
| meteor_contest           | 83.9 ms                                                                         | 88.3 ms: 1.05x slower                                                                     |
| json_dumps               | 6.73 ms                                                                         | 7.14 ms: 1.06x slower                                                                     |
| async_generators         | 283 ms                                                                          | 303 ms: 1.07x slower                                                                      |
| hexiom                   | 6.61 ms                                                                         | 7.09 ms: 1.07x slower                                                                     |
| sympy_integrate          | 16.0 ms                                                                         | 17.2 ms: 1.08x slower                                                                     |
| comprehensions           | 14.8 us                                                                         | 15.9 us: 1.08x slower                                                                     |
| json                     | 4.26 ms                                                                         | 4.71 ms: 1.11x slower                                                                     |
| Geometric mean           | (ref)                                                                           | 1.01x slower                                                                              |

Benchmark hidden because not significant (18): nbody, async_tree_memoization_tg, richards_super, async_tree_cpu_io_mixed_tg, async_tree_memoization, float, sqlglot_normalize, regex_v8, pprint_safe_repr, logging_simple, pathlib, sqlglot_transpile, pprint_pformat, spectral_norm, async_tree_none, asyncio_tcp_ssl, raytrace, pickle


# HPT report

- Reliability score: 96.25% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown