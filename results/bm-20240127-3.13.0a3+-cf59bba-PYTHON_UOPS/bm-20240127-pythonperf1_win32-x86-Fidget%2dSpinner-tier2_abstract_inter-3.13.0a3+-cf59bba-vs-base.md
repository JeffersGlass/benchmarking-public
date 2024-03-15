# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.00x faster
- HPT reliability: 82.21%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                                          | 250 ms: 1.02x slower                                                                      |
| chameleon      | 5.79 ms                                                                         | 5.86 ms: 1.01x slower                                                                     |
| docutils       | 1.84 sec                                                                        | 1.83 sec: 1.01x faster                                                                    |
| tornado_http   | 99.1 ms                                                                         | 101 ms: 1.01x slower                                                                      |
| Geometric mean | (ref)                                                                           | 1.01x slower                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 504 ms                                                                          | 514 ms: 1.02x slower                                                                      |
| async_tree_cpu_io_mixed    | 511 ms                                                                          | 522 ms: 1.02x slower                                                                      |
| Geometric mean             | (ref)                                                                           | 1.00x slower                                                                              |

Benchmark hidden because not significant (6): async_tree_memoization, async_tree_none_tg, async_tree_none, async_tree_io, async_tree_io_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 88.5 ms                                                                         | 85.2 ms: 1.04x faster                                                                     |
| float          | 59.3 ms                                                                         | 58.5 ms: 1.01x faster                                                                     |
| pidigits       | 200 ms                                                                          | 202 ms: 1.01x slower                                                                      |
| Geometric mean | (ref)                                                                           | 1.01x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_v8       | 16.0 ms                                                                         | 16.2 ms: 1.01x slower                                                                     |
| regex_compile  | 107 ms                                                                          | 108 ms: 1.01x slower                                                                      |
| regex_dna      | 119 ms                                                                          | 126 ms: 1.06x slower                                                                      |
| Geometric mean | (ref)                                                                           | 1.02x slower                                                                              |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|---------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| pickle_list         | 3.74 us                                                                         | 3.48 us: 1.08x faster                                                                     |
| unpickle_list       | 3.07 us                                                                         | 2.87 us: 1.07x faster                                                                     |
| xml_etree_iterparse | 71.1 ms                                                                         | 69.2 ms: 1.03x faster                                                                     |
| xml_etree_parse     | 113 ms                                                                          | 110 ms: 1.03x faster                                                                      |
| tomli_loads         | 1.68 sec                                                                        | 1.64 sec: 1.02x faster                                                                    |
| xml_etree_process   | 42.2 ms                                                                         | 41.3 ms: 1.02x faster                                                                     |
| xml_etree_generate  | 61.7 ms                                                                         | 60.6 ms: 1.02x faster                                                                     |
| pickle              | 7.74 us                                                                         | 7.64 us: 1.01x faster                                                                     |
| json_loads          | 19.7 us                                                                         | 19.9 us: 1.01x slower                                                                     |
| json_dumps          | 6.51 ms                                                                         | 6.62 ms: 1.02x slower                                                                     |
| pickle_dict         | 19.8 us                                                                         | 20.2 us: 1.02x slower                                                                     |
| unpickle            | 9.57 us                                                                         | 9.88 us: 1.03x slower                                                                     |
| Geometric mean      | (ref)                                                                           | 1.01x faster                                                                              |

Benchmark hidden because not significant (2): unpickle_pure_python, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 23.2 ms                                                                         | 23.5 ms: 1.01x slower                                                                     |
| python_startup_no_site | 20.7 ms                                                                         | 21.1 ms: 1.02x slower                                                                     |
| Geometric mean         | (ref)                                                                           | 1.02x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 8.03 ms                                                                         | 7.86 ms: 1.02x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpack_sequence            | 42.6 ns                                                                         | 39.5 ns: 1.08x faster                                                                     |
| pickle_list                | 3.74 us                                                                         | 3.48 us: 1.08x faster                                                                     |
| unpickle_list              | 3.07 us                                                                         | 2.87 us: 1.07x faster                                                                     |
| fannkuch                   | 314 ms                                                                          | 296 ms: 1.06x faster                                                                      |
| deltablue                  | 2.80 ms                                                                         | 2.65 ms: 1.06x faster                                                                     |
| comprehensions             | 14.0 us                                                                         | 13.2 us: 1.06x faster                                                                     |
| hexiom                     | 5.41 ms                                                                         | 5.18 ms: 1.04x faster                                                                     |
| nbody                      | 88.5 ms                                                                         | 85.2 ms: 1.04x faster                                                                     |
| logging_silent             | 61.8 ns                                                                         | 59.5 ns: 1.04x faster                                                                     |
| spectral_norm              | 84.6 ms                                                                         | 81.6 ms: 1.04x faster                                                                     |
| nqueens                    | 79.8 ms                                                                         | 77.0 ms: 1.04x faster                                                                     |
| scimark_fft                | 225 ms                                                                          | 217 ms: 1.03x faster                                                                      |
| meteor_contest             | 80.1 ms                                                                         | 77.6 ms: 1.03x faster                                                                     |
| xml_etree_iterparse        | 71.1 ms                                                                         | 69.2 ms: 1.03x faster                                                                     |
| scimark_monte_carlo        | 52.7 ms                                                                         | 51.3 ms: 1.03x faster                                                                     |
| telco                      | 6.23 ms                                                                         | 6.07 ms: 1.03x faster                                                                     |
| xml_etree_parse            | 113 ms                                                                          | 110 ms: 1.03x faster                                                                      |
| tomli_loads                | 1.68 sec                                                                        | 1.64 sec: 1.02x faster                                                                    |
| mako                       | 8.03 ms                                                                         | 7.86 ms: 1.02x faster                                                                     |
| xml_etree_process          | 42.2 ms                                                                         | 41.3 ms: 1.02x faster                                                                     |
| xml_etree_generate         | 61.7 ms                                                                         | 60.6 ms: 1.02x faster                                                                     |
| chaos                      | 53.0 ms                                                                         | 52.1 ms: 1.02x faster                                                                     |
| generators                 | 23.6 ms                                                                         | 23.2 ms: 1.02x faster                                                                     |
| scimark_sparse_mat_mult    | 3.35 ms                                                                         | 3.30 ms: 1.02x faster                                                                     |
| pyflate                    | 342 ms                                                                          | 337 ms: 1.02x faster                                                                      |
| gc_traversal               | 1.42 ms                                                                         | 1.40 ms: 1.01x faster                                                                     |
| float                      | 59.3 ms                                                                         | 58.5 ms: 1.01x faster                                                                     |
| create_gc_cycles           | 655 us                                                                          | 647 us: 1.01x faster                                                                      |
| pickle                     | 7.74 us                                                                         | 7.64 us: 1.01x faster                                                                     |
| docutils                   | 1.84 sec                                                                        | 1.83 sec: 1.01x faster                                                                    |
| async_generators           | 273 ms                                                                          | 271 ms: 1.01x faster                                                                      |
| sqlite_synth               | 1.85 us                                                                         | 1.84 us: 1.01x faster                                                                     |
| pathlib                    | 89.2 ms                                                                         | 88.7 ms: 1.01x faster                                                                     |
| scimark_lu                 | 62.3 ms                                                                         | 62.1 ms: 1.00x faster                                                                     |
| json_loads                 | 19.7 us                                                                         | 19.9 us: 1.01x slower                                                                     |
| sqlglot_normalize          | 211 ms                                                                          | 213 ms: 1.01x slower                                                                      |
| crypto_pyaes               | 57.7 ms                                                                         | 58.3 ms: 1.01x slower                                                                     |
| pidigits                   | 200 ms                                                                          | 202 ms: 1.01x slower                                                                      |
| regex_v8                   | 16.0 ms                                                                         | 16.2 ms: 1.01x slower                                                                     |
| sqlglot_parse              | 910 us                                                                          | 920 us: 1.01x slower                                                                      |
| chameleon                  | 5.79 ms                                                                         | 5.86 ms: 1.01x slower                                                                     |
| sympy_integrate            | 15.4 ms                                                                         | 15.6 ms: 1.01x slower                                                                     |
| go                         | 106 ms                                                                          | 107 ms: 1.01x slower                                                                      |
| richards                   | 28.9 ms                                                                         | 29.3 ms: 1.01x slower                                                                     |
| sympy_expand               | 367 ms                                                                          | 372 ms: 1.01x slower                                                                      |
| regex_compile              | 107 ms                                                                          | 108 ms: 1.01x slower                                                                      |
| sympy_str                  | 211 ms                                                                          | 214 ms: 1.01x slower                                                                      |
| python_startup             | 23.2 ms                                                                         | 23.5 ms: 1.01x slower                                                                     |
| typing_runtime_protocols   | 93.5 us                                                                         | 94.8 us: 1.01x slower                                                                     |
| tornado_http               | 99.1 ms                                                                         | 101 ms: 1.01x slower                                                                      |
| richards_super             | 33.0 ms                                                                         | 33.5 ms: 1.02x slower                                                                     |
| sqlglot_optimize           | 41.1 ms                                                                         | 41.8 ms: 1.02x slower                                                                     |
| 2to3                       | 246 ms                                                                          | 250 ms: 1.02x slower                                                                      |
| json_dumps                 | 6.51 ms                                                                         | 6.62 ms: 1.02x slower                                                                     |
| coverage                   | 477 ms                                                                          | 485 ms: 1.02x slower                                                                      |
| sqlglot_transpile          | 1.15 ms                                                                         | 1.17 ms: 1.02x slower                                                                     |
| pickle_dict                | 19.8 us                                                                         | 20.2 us: 1.02x slower                                                                     |
| pycparser                  | 839 ms                                                                          | 854 ms: 1.02x slower                                                                      |
| mdp                        | 1.64 sec                                                                        | 1.67 sec: 1.02x slower                                                                    |
| async_tree_cpu_io_mixed_tg | 504 ms                                                                          | 514 ms: 1.02x slower                                                                      |
| python_startup_no_site     | 20.7 ms                                                                         | 21.1 ms: 1.02x slower                                                                     |
| async_tree_cpu_io_mixed    | 511 ms                                                                          | 522 ms: 1.02x slower                                                                      |
| sympy_sum                  | 108 ms                                                                          | 111 ms: 1.02x slower                                                                      |
| logging_format             | 8.77 us                                                                         | 8.99 us: 1.03x slower                                                                     |
| raytrace                   | 210 ms                                                                          | 216 ms: 1.03x slower                                                                      |
| pprint_pformat             | 1.22 sec                                                                        | 1.26 sec: 1.03x slower                                                                    |
| unpickle                   | 9.57 us                                                                         | 9.88 us: 1.03x slower                                                                     |
| bench_mp_pool              | 73.0 ms                                                                         | 75.5 ms: 1.03x slower                                                                     |
| scimark_sor                | 81.0 ms                                                                         | 83.7 ms: 1.03x slower                                                                     |
| logging_simple             | 8.08 us                                                                         | 8.37 us: 1.04x slower                                                                     |
| pprint_safe_repr           | 598 ms                                                                          | 621 ms: 1.04x slower                                                                      |
| json                       | 3.98 ms                                                                         | 4.14 ms: 1.04x slower                                                                     |
| deepcopy                   | 268 us                                                                          | 280 us: 1.05x slower                                                                      |
| deepcopy_reduce            | 2.34 us                                                                         | 2.45 us: 1.05x slower                                                                     |
| deepcopy_memo              | 24.0 us                                                                         | 25.4 us: 1.06x slower                                                                     |
| regex_dna                  | 119 ms                                                                          | 126 ms: 1.06x slower                                                                      |
| Geometric mean             | (ref)                                                                           | 1.00x faster                                                                              |

Benchmark hidden because not significant (14): asyncio_tcp, async_tree_memoization, async_tree_none_tg, async_tree_none, unpickle_pure_python, async_tree_io, asyncio_tcp_ssl, pickle_pure_python, coroutines, async_tree_io_tg, async_tree_memoization_tg, dask, bench_thread_pool, regex_effbot


# HPT report

- Reliability score: 82.21% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown