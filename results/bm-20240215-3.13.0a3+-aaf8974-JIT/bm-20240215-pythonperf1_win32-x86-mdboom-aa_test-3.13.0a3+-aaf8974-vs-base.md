# Results vs. base

- fork: mdboom
- ref: aa_test
- machine: windows-x86
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.00x faster
- HPT reliability: 61.78%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| chameleon      | 5.96 ms                                                                         | 5.83 ms: 1.02x faster                                              |
| docutils       | 1.81 sec                                                                        | 1.81 sec: 1.00x slower                                             |
| tornado_http   | 97.8 ms                                                                         | 98.6 ms: 1.01x slower                                              |
| Geometric mean | (ref)                                                                           | 1.00x faster                                                       |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_memoization_tg  | 305 ms                                                                          | 301 ms: 1.01x faster                                               |
| async_tree_none_tg         | 243 ms                                                                          | 241 ms: 1.01x faster                                               |
| async_tree_memoization     | 320 ms                                                                          | 317 ms: 1.01x faster                                               |
| async_tree_io_tg           | 601 ms                                                                          | 597 ms: 1.01x faster                                               |
| async_tree_io              | 611 ms                                                                          | 615 ms: 1.01x slower                                               |
| async_tree_cpu_io_mixed_tg | 498 ms                                                                          | 503 ms: 1.01x slower                                               |
| async_tree_cpu_io_mixed    | 511 ms                                                                          | 517 ms: 1.01x slower                                               |
| Geometric mean             | (ref)                                                                           | 1.00x faster                                                       |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 92.6 ms                                                                         | 88.6 ms: 1.05x faster                                              |
| float          | 54.5 ms                                                                         | 54.0 ms: 1.01x faster                                              |
| pidigits       | 200 ms                                                                          | 199 ms: 1.00x faster                                               |
| Geometric mean | (ref)                                                                           | 1.02x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_v8       | 16.0 ms                                                                         | 15.8 ms: 1.01x faster                                              |
| regex_compile  | 108 ms                                                                          | 108 ms: 1.00x slower                                               |
| Geometric mean | (ref)                                                                           | 1.00x faster                                                       |

Benchmark hidden because not significant (2): regex_effbot, regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| xml_etree_parse      | 113 ms                                                                          | 109 ms: 1.04x faster                                               |
| pickle_list          | 3.26 us                                                                         | 3.18 us: 1.02x faster                                              |
| unpickle             | 10.3 us                                                                         | 10.1 us: 1.02x faster                                              |
| xml_etree_iterparse  | 68.0 ms                                                                         | 66.6 ms: 1.02x faster                                              |
| unpickle_pure_python | 161 us                                                                          | 158 us: 1.02x faster                                               |
| xml_etree_process    | 43.3 ms                                                                         | 42.6 ms: 1.02x faster                                              |
| pickle_pure_python   | 224 us                                                                          | 222 us: 1.01x faster                                               |
| xml_etree_generate   | 61.7 ms                                                                         | 61.1 ms: 1.01x faster                                              |
| json_loads           | 20.0 us                                                                         | 20.0 us: 1.00x slower                                              |
| unpickle_list        | 3.08 us                                                                         | 3.13 us: 1.02x slower                                              |
| tomli_loads          | 1.61 sec                                                                        | 1.67 sec: 1.04x slower                                             |
| Geometric mean       | (ref)                                                                           | 1.01x faster                                                       |

Benchmark hidden because not significant (3): pickle_dict, pickle, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup_no_site | 20.4 ms                                                                         | 20.8 ms: 1.02x slower                                              |
| python_startup         | 22.4 ms                                                                         | 22.9 ms: 1.02x slower                                              |
| Geometric mean         | (ref)                                                                           | 1.02x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 7.31 ms                                                                         | 7.44 ms: 1.02x slower                                              |

All benchmarks:
===============

| Benchmark                  | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------:|
| scimark_sor                | 94.1 ms                                                                         | 88.3 ms: 1.07x faster                                              |
| nbody                      | 92.6 ms                                                                         | 88.6 ms: 1.05x faster                                              |
| xml_etree_parse            | 113 ms                                                                          | 109 ms: 1.04x faster                                               |
| scimark_sparse_mat_mult    | 3.20 ms                                                                         | 3.11 ms: 1.03x faster                                              |
| coroutines                 | 15.2 ms                                                                         | 14.8 ms: 1.03x faster                                              |
| deepcopy_memo              | 26.4 us                                                                         | 25.7 us: 1.03x faster                                              |
| pickle_list                | 3.26 us                                                                         | 3.18 us: 1.02x faster                                              |
| chameleon                  | 5.96 ms                                                                         | 5.83 ms: 1.02x faster                                              |
| unpickle                   | 10.3 us                                                                         | 10.1 us: 1.02x faster                                              |
| xml_etree_iterparse        | 68.0 ms                                                                         | 66.6 ms: 1.02x faster                                              |
| unpickle_pure_python       | 161 us                                                                          | 158 us: 1.02x faster                                               |
| coverage                   | 483 ms                                                                          | 474 ms: 1.02x faster                                               |
| xml_etree_process          | 43.3 ms                                                                         | 42.6 ms: 1.02x faster                                              |
| async_tree_memoization_tg  | 305 ms                                                                          | 301 ms: 1.01x faster                                               |
| scimark_lu                 | 69.1 ms                                                                         | 68.2 ms: 1.01x faster                                              |
| scimark_monte_carlo        | 70.2 ms                                                                         | 69.3 ms: 1.01x faster                                              |
| pickle_pure_python         | 224 us                                                                          | 222 us: 1.01x faster                                               |
| comprehensions             | 14.3 us                                                                         | 14.1 us: 1.01x faster                                              |
| regex_v8                   | 16.0 ms                                                                         | 15.8 ms: 1.01x faster                                              |
| sqlglot_normalize          | 224 ms                                                                          | 221 ms: 1.01x faster                                               |
| richards                   | 31.2 ms                                                                         | 30.9 ms: 1.01x faster                                              |
| async_tree_none_tg         | 243 ms                                                                          | 241 ms: 1.01x faster                                               |
| sqlite_synth               | 1.89 us                                                                         | 1.87 us: 1.01x faster                                              |
| float                      | 54.5 ms                                                                         | 54.0 ms: 1.01x faster                                              |
| xml_etree_generate         | 61.7 ms                                                                         | 61.1 ms: 1.01x faster                                              |
| pprint_pformat             | 1.45 sec                                                                        | 1.43 sec: 1.01x faster                                             |
| deepcopy_reduce            | 2.45 us                                                                         | 2.43 us: 1.01x faster                                              |
| unpack_sequence            | 46.9 ns                                                                         | 46.5 ns: 1.01x faster                                              |
| async_tree_memoization     | 320 ms                                                                          | 317 ms: 1.01x faster                                               |
| pathlib                    | 84.3 ms                                                                         | 83.6 ms: 1.01x faster                                              |
| generators                 | 24.7 ms                                                                         | 24.5 ms: 1.01x faster                                              |
| async_tree_io_tg           | 601 ms                                                                          | 597 ms: 1.01x faster                                               |
| deltablue                  | 2.57 ms                                                                         | 2.55 ms: 1.01x faster                                              |
| asyncio_tcp_ssl            | 16.8 sec                                                                        | 16.7 sec: 1.01x faster                                             |
| pprint_safe_repr           | 703 ms                                                                          | 700 ms: 1.00x faster                                               |
| pidigits                   | 200 ms                                                                          | 199 ms: 1.00x faster                                               |
| json_loads                 | 20.0 us                                                                         | 20.0 us: 1.00x slower                                              |
| docutils                   | 1.81 sec                                                                        | 1.81 sec: 1.00x slower                                             |
| regex_compile              | 108 ms                                                                          | 108 ms: 1.00x slower                                               |
| meteor_contest             | 84.2 ms                                                                         | 84.6 ms: 1.00x slower                                              |
| async_tree_io              | 611 ms                                                                          | 615 ms: 1.01x slower                                               |
| hexiom                     | 6.50 ms                                                                         | 6.54 ms: 1.01x slower                                              |
| tornado_http               | 97.8 ms                                                                         | 98.6 ms: 1.01x slower                                              |
| nqueens                    | 87.0 ms                                                                         | 87.8 ms: 1.01x slower                                              |
| async_tree_cpu_io_mixed_tg | 498 ms                                                                          | 503 ms: 1.01x slower                                               |
| dask                       | 301 ms                                                                          | 305 ms: 1.01x slower                                               |
| sympy_str                  | 214 ms                                                                          | 216 ms: 1.01x slower                                               |
| pycparser                  | 861 ms                                                                          | 872 ms: 1.01x slower                                               |
| async_tree_cpu_io_mixed    | 511 ms                                                                          | 517 ms: 1.01x slower                                               |
| logging_format             | 8.95 us                                                                         | 9.07 us: 1.01x slower                                              |
| sympy_expand               | 374 ms                                                                          | 379 ms: 1.01x slower                                               |
| unpickle_list              | 3.08 us                                                                         | 3.13 us: 1.02x slower                                              |
| sympy_sum                  | 109 ms                                                                          | 110 ms: 1.02x slower                                               |
| mdp                        | 1.82 sec                                                                        | 1.84 sec: 1.02x slower                                             |
| logging_silent             | 66.7 ns                                                                         | 67.8 ns: 1.02x slower                                              |
| mako                       | 7.31 ms                                                                         | 7.44 ms: 1.02x slower                                              |
| python_startup_no_site     | 20.4 ms                                                                         | 20.8 ms: 1.02x slower                                              |
| logging_simple             | 8.25 us                                                                         | 8.42 us: 1.02x slower                                              |
| python_startup             | 22.4 ms                                                                         | 22.9 ms: 1.02x slower                                              |
| deepcopy                   | 280 us                                                                          | 286 us: 1.02x slower                                               |
| pyflate                    | 370 ms                                                                          | 379 ms: 1.02x slower                                               |
| fannkuch                   | 306 ms                                                                          | 315 ms: 1.03x slower                                               |
| telco                      | 6.11 ms                                                                         | 6.35 ms: 1.04x slower                                              |
| tomli_loads                | 1.61 sec                                                                        | 1.67 sec: 1.04x slower                                             |
| bench_mp_pool              | 71.2 ms                                                                         | 74.7 ms: 1.05x slower                                              |
| spectral_norm              | 70.6 ms                                                                         | 74.1 ms: 1.05x slower                                              |
| Geometric mean             | (ref)                                                                           | 1.00x faster                                                       |

Benchmark hidden because not significant (24): regex_effbot, scimark_fft, asyncio_tcp, go, crypto_pyaes, richards_super, pickle_dict, async_tree_none, pickle, regex_dna, json, sqlglot_optimize, bench_thread_pool, async_generators, sqlglot_parse, 2to3, sqlglot_transpile, raytrace, sympy_integrate, chaos, typing_runtime_protocols, json_dumps, gc_traversal, create_gc_cycles


# HPT report

- Reliability score: 61.78% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown