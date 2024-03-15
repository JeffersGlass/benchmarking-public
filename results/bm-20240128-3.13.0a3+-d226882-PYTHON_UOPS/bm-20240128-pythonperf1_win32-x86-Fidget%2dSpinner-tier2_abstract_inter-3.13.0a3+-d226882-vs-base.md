# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.00x slower
- HPT reliability: 52.81%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                                          | 250 ms: 1.01x slower                                                                      |
| docutils       | 1.84 sec                                                                        | 1.81 sec: 1.02x faster                                                                    |
| Geometric mean | (ref)                                                                           | 1.00x faster                                                                              |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|---------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_memoization    | 328 ms                                                                          | 316 ms: 1.04x faster                                                                      |
| async_tree_none           | 261 ms                                                                          | 255 ms: 1.02x faster                                                                      |
| async_tree_memoization_tg | 310 ms                                                                          | 306 ms: 1.01x faster                                                                      |
| async_tree_io_tg          | 603 ms                                                                          | 595 ms: 1.01x faster                                                                      |
| async_tree_io             | 628 ms                                                                          | 620 ms: 1.01x faster                                                                      |
| async_tree_none_tg        | 241 ms                                                                          | 244 ms: 1.01x slower                                                                      |
| async_tree_cpu_io_mixed   | 511 ms                                                                          | 521 ms: 1.02x slower                                                                      |
| Geometric mean            | (ref)                                                                           | 1.01x faster                                                                              |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 88.5 ms                                                                         | 87.0 ms: 1.02x faster                                                                     |
| pidigits       | 200 ms                                                                          | 204 ms: 1.02x slower                                                                      |
| float          | 59.3 ms                                                                         | 61.2 ms: 1.03x slower                                                                     |
| Geometric mean | (ref)                                                                           | 1.01x slower                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_v8       | 16.0 ms                                                                         | 16.2 ms: 1.01x slower                                                                     |
| regex_compile  | 107 ms                                                                          | 108 ms: 1.01x slower                                                                      |
| regex_effbot   | 1.89 ms                                                                         | 1.92 ms: 1.02x slower                                                                     |
| regex_dna      | 119 ms                                                                          | 123 ms: 1.03x slower                                                                      |
| Geometric mean | (ref)                                                                           | 1.02x slower                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|---------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| xml_etree_parse     | 113 ms                                                                          | 109 ms: 1.04x faster                                                                      |
| tomli_loads         | 1.68 sec                                                                        | 1.65 sec: 1.02x faster                                                                    |
| xml_etree_iterparse | 71.1 ms                                                                         | 70.5 ms: 1.01x faster                                                                     |
| xml_etree_generate  | 61.7 ms                                                                         | 61.2 ms: 1.01x faster                                                                     |
| pickle              | 7.74 us                                                                         | 7.78 us: 1.01x slower                                                                     |
| json_loads          | 19.7 us                                                                         | 20.0 us: 1.01x slower                                                                     |
| pickle_dict         | 19.8 us                                                                         | 20.2 us: 1.02x slower                                                                     |
| unpickle            | 9.57 us                                                                         | 9.90 us: 1.04x slower                                                                     |
| json_dumps          | 6.51 ms                                                                         | 6.87 ms: 1.06x slower                                                                     |
| Geometric mean      | (ref)                                                                           | 1.00x slower                                                                              |

Benchmark hidden because not significant (5): pickle_list, unpickle_list, xml_etree_process, pickle_pure_python, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 23.2 ms                                                                         | 23.8 ms: 1.03x slower                                                                     |
| python_startup_no_site | 20.7 ms                                                                         | 21.5 ms: 1.04x slower                                                                     |
| Geometric mean         | (ref)                                                                           | 1.03x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 8.03 ms                                                                         | 8.34 ms: 1.04x slower                                                                     |

All benchmarks:
===============

| Benchmark                 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|---------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| fannkuch                  | 314 ms                                                                          | 288 ms: 1.09x faster                                                                      |
| telco                     | 6.23 ms                                                                         | 5.75 ms: 1.08x faster                                                                     |
| xml_etree_parse           | 113 ms                                                                          | 109 ms: 1.04x faster                                                                      |
| async_tree_memoization    | 328 ms                                                                          | 316 ms: 1.04x faster                                                                      |
| scimark_fft               | 225 ms                                                                          | 217 ms: 1.04x faster                                                                      |
| sqlglot_parse             | 910 us                                                                          | 883 us: 1.03x faster                                                                      |
| nqueens                   | 79.8 ms                                                                         | 77.5 ms: 1.03x faster                                                                     |
| logging_silent            | 61.8 ns                                                                         | 60.2 ns: 1.03x faster                                                                     |
| unpack_sequence           | 42.6 ns                                                                         | 41.4 ns: 1.03x faster                                                                     |
| async_tree_none           | 261 ms                                                                          | 255 ms: 1.02x faster                                                                      |
| sqlglot_transpile         | 1.15 ms                                                                         | 1.13 ms: 1.02x faster                                                                     |
| coroutines                | 14.5 ms                                                                         | 14.2 ms: 1.02x faster                                                                     |
| docutils                  | 1.84 sec                                                                        | 1.81 sec: 1.02x faster                                                                    |
| crypto_pyaes              | 57.7 ms                                                                         | 56.7 ms: 1.02x faster                                                                     |
| generators                | 23.6 ms                                                                         | 23.2 ms: 1.02x faster                                                                     |
| chaos                     | 53.0 ms                                                                         | 52.1 ms: 1.02x faster                                                                     |
| nbody                     | 88.5 ms                                                                         | 87.0 ms: 1.02x faster                                                                     |
| gc_traversal              | 1.42 ms                                                                         | 1.40 ms: 1.02x faster                                                                     |
| tomli_loads               | 1.68 sec                                                                        | 1.65 sec: 1.02x faster                                                                    |
| async_tree_memoization_tg | 310 ms                                                                          | 306 ms: 1.01x faster                                                                      |
| async_tree_io_tg          | 603 ms                                                                          | 595 ms: 1.01x faster                                                                      |
| async_tree_io             | 628 ms                                                                          | 620 ms: 1.01x faster                                                                      |
| dask                      | 311 ms                                                                          | 308 ms: 1.01x faster                                                                      |
| scimark_monte_carlo       | 52.7 ms                                                                         | 52.2 ms: 1.01x faster                                                                     |
| xml_etree_iterparse       | 71.1 ms                                                                         | 70.5 ms: 1.01x faster                                                                     |
| xml_etree_generate        | 61.7 ms                                                                         | 61.2 ms: 1.01x faster                                                                     |
| pycparser                 | 839 ms                                                                          | 832 ms: 1.01x faster                                                                      |
| asyncio_tcp_ssl           | 17.6 sec                                                                        | 17.5 sec: 1.01x faster                                                                    |
| logging_format            | 8.77 us                                                                         | 8.72 us: 1.01x faster                                                                     |
| mdp                       | 1.64 sec                                                                        | 1.65 sec: 1.00x slower                                                                    |
| scimark_lu                | 62.3 ms                                                                         | 62.6 ms: 1.01x slower                                                                     |
| spectral_norm             | 84.6 ms                                                                         | 85.0 ms: 1.01x slower                                                                     |
| pickle                    | 7.74 us                                                                         | 7.78 us: 1.01x slower                                                                     |
| async_generators          | 273 ms                                                                          | 275 ms: 1.01x slower                                                                      |
| sqlglot_normalize         | 211 ms                                                                          | 213 ms: 1.01x slower                                                                      |
| regex_v8                  | 16.0 ms                                                                         | 16.2 ms: 1.01x slower                                                                     |
| regex_compile             | 107 ms                                                                          | 108 ms: 1.01x slower                                                                      |
| hexiom                    | 5.41 ms                                                                         | 5.47 ms: 1.01x slower                                                                     |
| sympy_str                 | 211 ms                                                                          | 214 ms: 1.01x slower                                                                      |
| async_tree_none_tg        | 241 ms                                                                          | 244 ms: 1.01x slower                                                                      |
| json_loads                | 19.7 us                                                                         | 20.0 us: 1.01x slower                                                                     |
| bench_thread_pool         | 1.06 ms                                                                         | 1.08 ms: 1.01x slower                                                                     |
| 2to3                      | 246 ms                                                                          | 250 ms: 1.01x slower                                                                      |
| sqlglot_optimize          | 41.1 ms                                                                         | 41.7 ms: 1.01x slower                                                                     |
| scimark_sor               | 81.0 ms                                                                         | 82.3 ms: 1.02x slower                                                                     |
| regex_effbot              | 1.89 ms                                                                         | 1.92 ms: 1.02x slower                                                                     |
| sympy_sum                 | 108 ms                                                                          | 110 ms: 1.02x slower                                                                      |
| pickle_dict               | 19.8 us                                                                         | 20.2 us: 1.02x slower                                                                     |
| richards                  | 28.9 ms                                                                         | 29.4 ms: 1.02x slower                                                                     |
| async_tree_cpu_io_mixed   | 511 ms                                                                          | 521 ms: 1.02x slower                                                                      |
| typing_runtime_protocols  | 93.5 us                                                                         | 95.4 us: 1.02x slower                                                                     |
| pidigits                  | 200 ms                                                                          | 204 ms: 1.02x slower                                                                      |
| bench_mp_pool             | 73.0 ms                                                                         | 74.6 ms: 1.02x slower                                                                     |
| deepcopy_memo             | 24.0 us                                                                         | 24.6 us: 1.02x slower                                                                     |
| deepcopy_reduce           | 2.34 us                                                                         | 2.39 us: 1.02x slower                                                                     |
| deepcopy                  | 268 us                                                                          | 275 us: 1.02x slower                                                                      |
| create_gc_cycles          | 655 us                                                                          | 671 us: 1.02x slower                                                                      |
| logging_simple            | 8.08 us                                                                         | 8.28 us: 1.03x slower                                                                     |
| python_startup            | 23.2 ms                                                                         | 23.8 ms: 1.03x slower                                                                     |
| deltablue                 | 2.80 ms                                                                         | 2.89 ms: 1.03x slower                                                                     |
| json                      | 3.98 ms                                                                         | 4.10 ms: 1.03x slower                                                                     |
| regex_dna                 | 119 ms                                                                          | 123 ms: 1.03x slower                                                                      |
| sqlite_synth              | 1.85 us                                                                         | 1.90 us: 1.03x slower                                                                     |
| float                     | 59.3 ms                                                                         | 61.2 ms: 1.03x slower                                                                     |
| pprint_pformat            | 1.22 sec                                                                        | 1.26 sec: 1.03x slower                                                                    |
| unpickle                  | 9.57 us                                                                         | 9.90 us: 1.04x slower                                                                     |
| mako                      | 8.03 ms                                                                         | 8.34 ms: 1.04x slower                                                                     |
| pprint_safe_repr          | 598 ms                                                                          | 622 ms: 1.04x slower                                                                      |
| python_startup_no_site    | 20.7 ms                                                                         | 21.5 ms: 1.04x slower                                                                     |
| json_dumps                | 6.51 ms                                                                         | 6.87 ms: 1.06x slower                                                                     |
| coverage                  | 477 ms                                                                          | 505 ms: 1.06x slower                                                                      |
| Geometric mean            | (ref)                                                                           | 1.00x slower                                                                              |

Benchmark hidden because not significant (19): pickle_list, unpickle_list, tornado_http, raytrace, pyflate, comprehensions, go, meteor_contest, asyncio_tcp, xml_etree_process, sympy_integrate, pickle_pure_python, async_tree_cpu_io_mixed_tg, pathlib, richards_super, sympy_expand, scimark_sparse_mat_mult, chameleon, unpickle_pure_python


# HPT report

- Reliability score: 52.81% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown