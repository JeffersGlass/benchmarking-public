# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.01x faster
- HPT reliability: 97.58%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                                          | 252 ms: 1.02x slower                                                                      |
| chameleon      | 5.79 ms                                                                         | 5.72 ms: 1.01x faster                                                                     |
| docutils       | 1.84 sec                                                                        | 1.81 sec: 1.02x faster                                                                    |
| tornado_http   | 99.1 ms                                                                         | 99.9 ms: 1.01x slower                                                                     |
| Geometric mean | (ref)                                                                           | 1.00x slower                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 310 ms                                                                          | 301 ms: 1.03x faster                                                                      |
| async_tree_memoization     | 328 ms                                                                          | 320 ms: 1.02x faster                                                                      |
| async_tree_io              | 628 ms                                                                          | 614 ms: 1.02x faster                                                                      |
| async_tree_none            | 261 ms                                                                          | 256 ms: 1.02x faster                                                                      |
| async_tree_cpu_io_mixed    | 511 ms                                                                          | 501 ms: 1.02x faster                                                                      |
| async_tree_none_tg         | 241 ms                                                                          | 237 ms: 1.02x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 504 ms                                                                          | 499 ms: 1.01x faster                                                                      |
| async_tree_io_tg           | 603 ms                                                                          | 599 ms: 1.01x faster                                                                      |
| Geometric mean             | (ref)                                                                           | 1.02x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 88.5 ms                                                                         | 82.3 ms: 1.08x faster                                                                     |
| float          | 59.3 ms                                                                         | 56.6 ms: 1.05x faster                                                                     |
| Geometric mean | (ref)                                                                           | 1.04x faster                                                                              |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_dna      | 119 ms                                                                          | 120 ms: 1.01x slower                                                                      |
| regex_v8       | 16.0 ms                                                                         | 16.3 ms: 1.02x slower                                                                     |
| Geometric mean | (ref)                                                                           | 1.01x slower                                                                              |

Benchmark hidden because not significant (2): regex_compile, regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| pickle_list          | 3.74 us                                                                         | 3.52 us: 1.06x faster                                                                     |
| xml_etree_process    | 42.2 ms                                                                         | 41.1 ms: 1.03x faster                                                                     |
| xml_etree_generate   | 61.7 ms                                                                         | 60.3 ms: 1.02x faster                                                                     |
| xml_etree_iterparse  | 71.1 ms                                                                         | 69.9 ms: 1.02x faster                                                                     |
| unpickle_list        | 3.07 us                                                                         | 3.01 us: 1.02x faster                                                                     |
| xml_etree_parse      | 113 ms                                                                          | 112 ms: 1.01x faster                                                                      |
| unpickle_pure_python | 150 us                                                                          | 150 us: 1.00x slower                                                                      |
| unpickle             | 9.57 us                                                                         | 9.62 us: 1.01x slower                                                                     |
| pickle_pure_python   | 208 us                                                                          | 211 us: 1.01x slower                                                                      |
| pickle_dict          | 19.8 us                                                                         | 20.1 us: 1.02x slower                                                                     |
| pickle               | 7.74 us                                                                         | 7.88 us: 1.02x slower                                                                     |
| json_loads           | 19.7 us                                                                         | 20.2 us: 1.03x slower                                                                     |
| json_dumps           | 6.51 ms                                                                         | 6.84 ms: 1.05x slower                                                                     |
| Geometric mean       | (ref)                                                                           | 1.00x faster                                                                              |

Benchmark hidden because not significant (1): tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup | 23.2 ms                                                                         | 22.9 ms: 1.01x faster                                                                     |
| Geometric mean | (ref)                                                                           | 1.00x faster                                                                              |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 8.03 ms                                                                         | 7.73 ms: 1.04x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| asyncio_tcp                | 680 ms                                                                          | 622 ms: 1.09x faster                                                                      |
| fannkuch                   | 314 ms                                                                          | 289 ms: 1.09x faster                                                                      |
| spectral_norm              | 84.6 ms                                                                         | 78.2 ms: 1.08x faster                                                                     |
| nbody                      | 88.5 ms                                                                         | 82.3 ms: 1.08x faster                                                                     |
| hexiom                     | 5.41 ms                                                                         | 5.08 ms: 1.06x faster                                                                     |
| pickle_list                | 3.74 us                                                                         | 3.52 us: 1.06x faster                                                                     |
| scimark_fft                | 225 ms                                                                          | 212 ms: 1.06x faster                                                                      |
| comprehensions             | 14.0 us                                                                         | 13.3 us: 1.05x faster                                                                     |
| telco                      | 6.23 ms                                                                         | 5.92 ms: 1.05x faster                                                                     |
| deltablue                  | 2.80 ms                                                                         | 2.68 ms: 1.05x faster                                                                     |
| float                      | 59.3 ms                                                                         | 56.6 ms: 1.05x faster                                                                     |
| mako                       | 8.03 ms                                                                         | 7.73 ms: 1.04x faster                                                                     |
| nqueens                    | 79.8 ms                                                                         | 77.0 ms: 1.04x faster                                                                     |
| raytrace                   | 210 ms                                                                          | 203 ms: 1.04x faster                                                                      |
| scimark_monte_carlo        | 52.7 ms                                                                         | 50.9 ms: 1.03x faster                                                                     |
| coverage                   | 477 ms                                                                          | 461 ms: 1.03x faster                                                                      |
| async_tree_memoization_tg  | 310 ms                                                                          | 301 ms: 1.03x faster                                                                      |
| scimark_sparse_mat_mult    | 3.35 ms                                                                         | 3.26 ms: 1.03x faster                                                                     |
| xml_etree_process          | 42.2 ms                                                                         | 41.1 ms: 1.03x faster                                                                     |
| async_tree_memoization     | 328 ms                                                                          | 320 ms: 1.02x faster                                                                      |
| xml_etree_generate         | 61.7 ms                                                                         | 60.3 ms: 1.02x faster                                                                     |
| async_tree_io              | 628 ms                                                                          | 614 ms: 1.02x faster                                                                      |
| pyflate                    | 342 ms                                                                          | 335 ms: 1.02x faster                                                                      |
| async_tree_none            | 261 ms                                                                          | 256 ms: 1.02x faster                                                                      |
| logging_silent             | 61.8 ns                                                                         | 60.6 ns: 1.02x faster                                                                     |
| async_tree_cpu_io_mixed    | 511 ms                                                                          | 501 ms: 1.02x faster                                                                      |
| async_tree_none_tg         | 241 ms                                                                          | 237 ms: 1.02x faster                                                                      |
| xml_etree_iterparse        | 71.1 ms                                                                         | 69.9 ms: 1.02x faster                                                                     |
| unpickle_list              | 3.07 us                                                                         | 3.01 us: 1.02x faster                                                                     |
| docutils                   | 1.84 sec                                                                        | 1.81 sec: 1.02x faster                                                                    |
| generators                 | 23.6 ms                                                                         | 23.3 ms: 1.01x faster                                                                     |
| xml_etree_parse            | 113 ms                                                                          | 112 ms: 1.01x faster                                                                      |
| logging_format             | 8.77 us                                                                         | 8.66 us: 1.01x faster                                                                     |
| chameleon                  | 5.79 ms                                                                         | 5.72 ms: 1.01x faster                                                                     |
| python_startup             | 23.2 ms                                                                         | 22.9 ms: 1.01x faster                                                                     |
| coroutines                 | 14.5 ms                                                                         | 14.4 ms: 1.01x faster                                                                     |
| async_tree_cpu_io_mixed_tg | 504 ms                                                                          | 499 ms: 1.01x faster                                                                      |
| meteor_contest             | 80.1 ms                                                                         | 79.3 ms: 1.01x faster                                                                     |
| sympy_str                  | 211 ms                                                                          | 209 ms: 1.01x faster                                                                      |
| async_tree_io_tg           | 603 ms                                                                          | 599 ms: 1.01x faster                                                                      |
| deepcopy                   | 268 us                                                                          | 266 us: 1.01x faster                                                                      |
| sympy_expand               | 367 ms                                                                          | 366 ms: 1.00x faster                                                                      |
| sqlite_synth               | 1.85 us                                                                         | 1.85 us: 1.00x slower                                                                     |
| unpickle_pure_python       | 150 us                                                                          | 150 us: 1.00x slower                                                                      |
| unpickle                   | 9.57 us                                                                         | 9.62 us: 1.01x slower                                                                     |
| logging_simple             | 8.08 us                                                                         | 8.12 us: 1.01x slower                                                                     |
| sympy_integrate            | 15.4 ms                                                                         | 15.5 ms: 1.01x slower                                                                     |
| scimark_lu                 | 62.3 ms                                                                         | 62.7 ms: 1.01x slower                                                                     |
| scimark_sor                | 81.0 ms                                                                         | 81.5 ms: 1.01x slower                                                                     |
| tornado_http               | 99.1 ms                                                                         | 99.9 ms: 1.01x slower                                                                     |
| go                         | 106 ms                                                                          | 107 ms: 1.01x slower                                                                      |
| deepcopy_memo              | 24.0 us                                                                         | 24.3 us: 1.01x slower                                                                     |
| regex_dna                  | 119 ms                                                                          | 120 ms: 1.01x slower                                                                      |
| sqlglot_normalize          | 211 ms                                                                          | 214 ms: 1.01x slower                                                                      |
| chaos                      | 53.0 ms                                                                         | 53.6 ms: 1.01x slower                                                                     |
| pickle_pure_python         | 208 us                                                                          | 211 us: 1.01x slower                                                                      |
| pickle_dict                | 19.8 us                                                                         | 20.1 us: 1.02x slower                                                                     |
| regex_v8                   | 16.0 ms                                                                         | 16.3 ms: 1.02x slower                                                                     |
| sqlglot_optimize           | 41.1 ms                                                                         | 41.8 ms: 1.02x slower                                                                     |
| sqlglot_transpile          | 1.15 ms                                                                         | 1.17 ms: 1.02x slower                                                                     |
| pickle                     | 7.74 us                                                                         | 7.88 us: 1.02x slower                                                                     |
| json                       | 3.98 ms                                                                         | 4.06 ms: 1.02x slower                                                                     |
| bench_thread_pool          | 1.06 ms                                                                         | 1.09 ms: 1.02x slower                                                                     |
| pycparser                  | 839 ms                                                                          | 857 ms: 1.02x slower                                                                      |
| 2to3                       | 246 ms                                                                          | 252 ms: 1.02x slower                                                                      |
| json_loads                 | 19.7 us                                                                         | 20.2 us: 1.03x slower                                                                     |
| sqlglot_parse              | 910 us                                                                          | 935 us: 1.03x slower                                                                      |
| bench_mp_pool              | 73.0 ms                                                                         | 75.3 ms: 1.03x slower                                                                     |
| crypto_pyaes               | 57.7 ms                                                                         | 59.7 ms: 1.04x slower                                                                     |
| async_generators           | 273 ms                                                                          | 283 ms: 1.04x slower                                                                      |
| richards                   | 28.9 ms                                                                         | 30.3 ms: 1.05x slower                                                                     |
| json_dumps                 | 6.51 ms                                                                         | 6.84 ms: 1.05x slower                                                                     |
| richards_super             | 33.0 ms                                                                         | 34.7 ms: 1.05x slower                                                                     |
| unpack_sequence            | 42.6 ns                                                                         | 46.1 ns: 1.08x slower                                                                     |
| Geometric mean             | (ref)                                                                           | 1.01x faster                                                                              |

Benchmark hidden because not significant (16): deepcopy_reduce, pidigits, tomli_loads, create_gc_cycles, typing_runtime_protocols, gc_traversal, regex_compile, pprint_pformat, pathlib, python_startup_no_site, dask, pprint_safe_repr, mdp, asyncio_tcp_ssl, sympy_sum, regex_effbot


# HPT report

- Reliability score: 97.58% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown