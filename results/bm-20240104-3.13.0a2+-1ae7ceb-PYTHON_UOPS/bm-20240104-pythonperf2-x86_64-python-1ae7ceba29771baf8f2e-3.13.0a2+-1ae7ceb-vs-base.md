# Results vs. base

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.00x slower
- HPT reliability: 54.96%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 311 ms                                                                       | 310 ms: 1.00x faster                                                         |
| chameleon      | 7.82 ms                                                                      | 8.01 ms: 1.02x slower                                                        |
| docutils       | 2.93 sec                                                                     | 2.95 sec: 1.00x slower                                                       |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|---------------------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none_tg        | 448 ms                                                                       | 445 ms: 1.01x faster                                                         |
| async_tree_io_tg          | 1.09 sec                                                                     | 1.09 sec: 1.01x faster                                                       |
| async_tree_io             | 1.10 sec                                                                     | 1.09 sec: 1.01x faster                                                       |
| async_tree_memoization_tg | 555 ms                                                                       | 567 ms: 1.02x slower                                                         |
| Geometric mean            | (ref)                                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                                       | 265 ms: 1.00x slower                                                         |
| nbody          | 126 ms                                                                       | 128 ms: 1.01x slower                                                         |
| float          | 102 ms                                                                       | 103 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 236 ms                                                                       | 239 ms: 1.01x slower                                                         |
| regex_effbot   | 3.44 ms                                                                      | 3.51 ms: 1.02x slower                                                        |
| regex_v8       | 24.9 ms                                                                      | 25.9 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_loads         | 25.2 us                                                                      | 24.7 us: 1.02x faster                                                        |
| tomli_loads        | 2.81 sec                                                                     | 2.77 sec: 1.01x faster                                                       |
| unpickle           | 14.7 us                                                                      | 14.6 us: 1.01x faster                                                        |
| xml_etree_generate | 92.8 ms                                                                      | 92.1 ms: 1.01x faster                                                        |
| xml_etree_process  | 63.0 ms                                                                      | 62.7 ms: 1.01x faster                                                        |
| json_dumps         | 10.9 ms                                                                      | 11.0 ms: 1.01x slower                                                        |
| pickle_pure_python | 309 us                                                                       | 314 us: 1.01x slower                                                         |
| xml_etree_parse    | 148 ms                                                                       | 150 ms: 1.02x slower                                                         |
| pickle             | 10.1 us                                                                      | 10.2 us: 1.02x slower                                                        |
| pickle_dict        | 30.5 us                                                                      | 31.2 us: 1.02x slower                                                        |
| unpickle_list      | 4.57 us                                                                      | 4.68 us: 1.02x slower                                                        |
| pickle_list        | 4.35 us                                                                      | 4.57 us: 1.05x slower                                                        |
| Geometric mean     | (ref)                                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (2): unpickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 12.5 ms                                                                      | 12.6 ms: 1.00x slower                                                        |
| python_startup_no_site | 11.0 ms                                                                      | 11.0 ms: 1.00x slower                                                        |
| Geometric mean         | (ref)                                                                        | 1.00x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.6 ms                                                                      | 15.0 ms: 1.03x slower                                                        |

All benchmarks:
===============

| Benchmark                 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|---------------------------|:----------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpack_sequence           | 46.6 ns                                                                      | 44.0 ns: 1.06x faster                                                        |
| spectral_norm             | 172 ms                                                                       | 164 ms: 1.05x faster                                                         |
| pyflate                   | 597 ms                                                                       | 574 ms: 1.04x faster                                                         |
| scimark_sparse_mat_mult   | 6.52 ms                                                                      | 6.37 ms: 1.02x faster                                                        |
| nqueens                   | 110 ms                                                                       | 107 ms: 1.02x faster                                                         |
| json_loads                | 25.2 us                                                                      | 24.7 us: 1.02x faster                                                        |
| deepcopy                  | 381 us                                                                       | 375 us: 1.02x faster                                                         |
| chaos                     | 77.2 ms                                                                      | 76.0 ms: 1.02x faster                                                        |
| pprint_safe_repr          | 929 ms                                                                       | 915 ms: 1.02x faster                                                         |
| pprint_pformat            | 1.92 sec                                                                     | 1.89 sec: 1.01x faster                                                       |
| scimark_fft               | 429 ms                                                                       | 423 ms: 1.01x faster                                                         |
| richards_super            | 59.6 ms                                                                      | 58.7 ms: 1.01x faster                                                        |
| gc_traversal              | 3.79 ms                                                                      | 3.74 ms: 1.01x faster                                                        |
| tomli_loads               | 2.81 sec                                                                     | 2.77 sec: 1.01x faster                                                       |
| create_gc_cycles          | 1.63 ms                                                                      | 1.61 ms: 1.01x faster                                                        |
| scimark_monte_carlo       | 86.7 ms                                                                      | 85.8 ms: 1.01x faster                                                        |
| unpickle                  | 14.7 us                                                                      | 14.6 us: 1.01x faster                                                        |
| telco                     | 8.49 ms                                                                      | 8.41 ms: 1.01x faster                                                        |
| xml_etree_generate        | 92.8 ms                                                                      | 92.1 ms: 1.01x faster                                                        |
| meteor_contest            | 140 ms                                                                       | 139 ms: 1.01x faster                                                         |
| async_tree_none_tg        | 448 ms                                                                       | 445 ms: 1.01x faster                                                         |
| logging_format            | 7.49 us                                                                      | 7.44 us: 1.01x faster                                                        |
| async_tree_io_tg          | 1.09 sec                                                                     | 1.09 sec: 1.01x faster                                                       |
| json                      | 5.24 ms                                                                      | 5.20 ms: 1.01x faster                                                        |
| xml_etree_process         | 63.0 ms                                                                      | 62.7 ms: 1.01x faster                                                        |
| scimark_lu                | 106 ms                                                                       | 105 ms: 1.01x faster                                                         |
| async_tree_io             | 1.10 sec                                                                     | 1.09 sec: 1.01x faster                                                       |
| sqlglot_parse             | 1.46 ms                                                                      | 1.45 ms: 1.00x faster                                                        |
| fannkuch                  | 475 ms                                                                       | 473 ms: 1.00x faster                                                         |
| 2to3                      | 311 ms                                                                       | 310 ms: 1.00x faster                                                         |
| mdp                       | 2.64 sec                                                                     | 2.63 sec: 1.00x faster                                                       |
| comprehensions            | 25.0 us                                                                      | 24.9 us: 1.00x faster                                                        |
| python_startup            | 12.5 ms                                                                      | 12.6 ms: 1.00x slower                                                        |
| python_startup_no_site    | 11.0 ms                                                                      | 11.0 ms: 1.00x slower                                                        |
| pidigits                  | 265 ms                                                                       | 265 ms: 1.00x slower                                                         |
| sqlglot_optimize          | 63.6 ms                                                                      | 63.8 ms: 1.00x slower                                                        |
| docutils                  | 2.93 sec                                                                     | 2.95 sec: 1.00x slower                                                       |
| sympy_sum                 | 169 ms                                                                       | 170 ms: 1.01x slower                                                         |
| deepcopy_reduce           | 3.36 us                                                                      | 3.39 us: 1.01x slower                                                        |
| logging_simple            | 6.80 us                                                                      | 6.85 us: 1.01x slower                                                        |
| asyncio_tcp               | 372 ms                                                                       | 375 ms: 1.01x slower                                                         |
| deepcopy_memo             | 39.8 us                                                                      | 40.1 us: 1.01x slower                                                        |
| generators                | 33.8 ms                                                                      | 34.1 ms: 1.01x slower                                                        |
| coroutines                | 22.0 ms                                                                      | 22.2 ms: 1.01x slower                                                        |
| sqlglot_normalize         | 124 ms                                                                       | 125 ms: 1.01x slower                                                         |
| sqlite_synth              | 2.79 us                                                                      | 2.82 us: 1.01x slower                                                        |
| asyncio_websockets        | 384 ms                                                                       | 387 ms: 1.01x slower                                                         |
| regex_dna                 | 236 ms                                                                       | 239 ms: 1.01x slower                                                         |
| json_dumps                | 10.9 ms                                                                      | 11.0 ms: 1.01x slower                                                        |
| dask                      | 409 ms                                                                       | 414 ms: 1.01x slower                                                         |
| async_generators          | 370 ms                                                                       | 374 ms: 1.01x slower                                                         |
| nbody                     | 126 ms                                                                       | 128 ms: 1.01x slower                                                         |
| float                     | 102 ms                                                                       | 103 ms: 1.01x slower                                                         |
| pickle_pure_python        | 309 us                                                                       | 314 us: 1.01x slower                                                         |
| xml_etree_parse           | 148 ms                                                                       | 150 ms: 1.02x slower                                                         |
| pickle                    | 10.1 us                                                                      | 10.2 us: 1.02x slower                                                        |
| logging_silent            | 99.7 ns                                                                      | 102 ns: 1.02x slower                                                         |
| regex_effbot              | 3.44 ms                                                                      | 3.51 ms: 1.02x slower                                                        |
| async_tree_memoization_tg | 555 ms                                                                       | 567 ms: 1.02x slower                                                         |
| typing_runtime_protocols  | 127 us                                                                       | 129 us: 1.02x slower                                                         |
| deltablue                 | 5.37 ms                                                                      | 5.49 ms: 1.02x slower                                                        |
| pickle_dict               | 30.5 us                                                                      | 31.2 us: 1.02x slower                                                        |
| chameleon                 | 7.82 ms                                                                      | 8.01 ms: 1.02x slower                                                        |
| unpickle_list             | 4.57 us                                                                      | 4.68 us: 1.02x slower                                                        |
| mako                      | 14.6 ms                                                                      | 15.0 ms: 1.03x slower                                                        |
| regex_v8                  | 24.9 ms                                                                      | 25.9 ms: 1.04x slower                                                        |
| go                        | 180 ms                                                                       | 187 ms: 1.04x slower                                                         |
| pickle_list               | 4.35 us                                                                      | 4.57 us: 1.05x slower                                                        |
| coverage                  | 79.9 ms                                                                      | 85.7 ms: 1.07x slower                                                        |
| Geometric mean            | (ref)                                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (24): bench_mp_pool, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, sqlglot_transpile, unpickle_pure_python, sympy_str, async_tree_memoization, regex_compile, dulwich_log, xml_etree_iterparse, hexiom, sympy_expand, sympy_integrate, crypto_pyaes, async_tree_none, asyncio_tcp_ssl, pathlib, scimark_sor, mypy2, richards, raytrace, bench_thread_pool, pycparser, tornado_http


# HPT report

- Reliability score: 54.96% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x