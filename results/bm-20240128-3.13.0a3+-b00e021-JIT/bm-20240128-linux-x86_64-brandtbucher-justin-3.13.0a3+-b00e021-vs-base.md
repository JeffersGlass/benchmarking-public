# Results vs. base

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b00e021
- commit date: 2024-01-28
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3+-a16a9f9 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| chameleon      | 7.15 ms                                                                | 7.07 ms: 1.01x faster                                          |
| docutils       | 2.66 sec                                                               | 2.66 sec: 1.00x faster                                         |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3+-a16a9f9 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_memoization    | 574 ms                                                                 | 564 ms: 1.02x faster                                           |
| async_tree_memoization_tg | 584 ms                                                                 | 575 ms: 1.02x faster                                           |
| async_tree_io             | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                         |
| async_tree_io_tg          | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                         |
| async_tree_none_tg        | 451 ms                                                                 | 448 ms: 1.01x faster                                           |
| Geometric mean            | (ref)                                                                  | 1.01x faster                                                   |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3+-a16a9f9 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 107 ms                                                                 | 104 ms: 1.04x faster                                           |
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x faster                                           |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                   |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3+-a16a9f9 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 228 ms                                                                 | 219 ms: 1.04x faster                                           |
| regex_effbot   | 3.65 ms                                                                | 3.53 ms: 1.03x faster                                          |
| regex_compile  | 142 ms                                                                 | 140 ms: 1.02x faster                                           |
| regex_v8       | 24.9 ms                                                                | 24.5 ms: 1.02x faster                                          |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3+-a16a9f9 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps         | 10.6 ms                                                                | 10.3 ms: 1.03x faster                                          |
| unpickle_list      | 5.28 us                                                                | 5.18 us: 1.02x faster                                          |
| pickle_pure_python | 297 us                                                                 | 292 us: 1.02x faster                                           |
| tomli_loads        | 2.22 sec                                                               | 2.21 sec: 1.00x faster                                         |
| json_loads         | 28.1 us                                                                | 28.3 us: 1.01x slower                                          |
| pickle_dict        | 34.0 us                                                                | 34.3 us: 1.01x slower                                          |
| pickle             | 11.4 us                                                                | 11.5 us: 1.01x slower                                          |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (7): xml_etree_parse, pickle_list, xml_etree_iterparse, unpickle_pure_python, xml_etree_process, xml_etree_generate, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3+-a16a9f9 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                          |
| python_startup_no_site | 8.74 ms                                                                | 8.84 ms: 1.01x slower                                          |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                   |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                 | bm-20240128-linux-x86_64-python-a16a9f978f42b8a09297-3.13.0a3+-a16a9f9 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| unpack_sequence           | 51.7 ns                                                                | 42.1 ns: 1.23x faster                                          |
| logging_silent            | 107 ns                                                                 | 102 ns: 1.05x faster                                           |
| deepcopy_memo             | 39.4 us                                                                | 37.6 us: 1.05x faster                                          |
| pprint_pformat            | 1.73 sec                                                               | 1.65 sec: 1.04x faster                                         |
| regex_dna                 | 228 ms                                                                 | 219 ms: 1.04x faster                                           |
| nbody                     | 107 ms                                                                 | 104 ms: 1.04x faster                                           |
| regex_effbot              | 3.65 ms                                                                | 3.53 ms: 1.03x faster                                          |
| coverage                  | 96.1 ms                                                                | 93.4 ms: 1.03x faster                                          |
| json_dumps                | 10.6 ms                                                                | 10.3 ms: 1.03x faster                                          |
| pprint_safe_repr          | 819 ms                                                                 | 798 ms: 1.03x faster                                           |
| raytrace                  | 288 ms                                                                 | 282 ms: 1.02x faster                                           |
| coroutines                | 22.4 ms                                                                | 22.0 ms: 1.02x faster                                          |
| unpickle_list             | 5.28 us                                                                | 5.18 us: 1.02x faster                                          |
| crypto_pyaes              | 79.0 ms                                                                | 77.5 ms: 1.02x faster                                          |
| fannkuch                  | 441 ms                                                                 | 432 ms: 1.02x faster                                           |
| logging_simple            | 5.88 us                                                                | 5.77 us: 1.02x faster                                          |
| regex_compile             | 142 ms                                                                 | 140 ms: 1.02x faster                                           |
| async_tree_memoization    | 574 ms                                                                 | 564 ms: 1.02x faster                                           |
| meteor_contest            | 112 ms                                                                 | 110 ms: 1.02x faster                                           |
| async_tree_memoization_tg | 584 ms                                                                 | 575 ms: 1.02x faster                                           |
| pickle_pure_python        | 297 us                                                                 | 292 us: 1.02x faster                                           |
| regex_v8                  | 24.9 ms                                                                | 24.5 ms: 1.02x faster                                          |
| go                        | 152 ms                                                                 | 150 ms: 1.02x faster                                           |
| async_tree_io             | 1.19 sec                                                               | 1.18 sec: 1.01x faster                                         |
| richards                  | 47.5 ms                                                                | 46.8 ms: 1.01x faster                                          |
| comprehensions            | 19.7 us                                                                | 19.4 us: 1.01x faster                                          |
| pyflate                   | 524 ms                                                                 | 517 ms: 1.01x faster                                           |
| async_tree_io_tg          | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                         |
| chameleon                 | 7.15 ms                                                                | 7.07 ms: 1.01x faster                                          |
| deepcopy                  | 347 us                                                                 | 344 us: 1.01x faster                                           |
| sympy_expand              | 482 ms                                                                 | 478 ms: 1.01x faster                                           |
| deltablue                 | 4.10 ms                                                                | 4.06 ms: 1.01x faster                                          |
| sympy_integrate           | 21.0 ms                                                                | 20.9 ms: 1.01x faster                                          |
| async_tree_none_tg        | 451 ms                                                                 | 448 ms: 1.01x faster                                           |
| logging_format            | 6.48 us                                                                | 6.44 us: 1.01x faster                                          |
| hexiom                    | 8.10 ms                                                                | 8.05 ms: 1.01x faster                                          |
| asyncio_tcp               | 494 ms                                                                 | 491 ms: 1.01x faster                                           |
| sympy_sum                 | 160 ms                                                                 | 160 ms: 1.01x faster                                           |
| sqlite_synth              | 2.81 us                                                                | 2.80 us: 1.01x faster                                          |
| scimark_fft               | 383 ms                                                                 | 381 ms: 1.01x faster                                           |
| tomli_loads               | 2.22 sec                                                               | 2.21 sec: 1.00x faster                                         |
| sqlglot_optimize          | 56.3 ms                                                                | 56.1 ms: 1.00x faster                                          |
| docutils                  | 2.66 sec                                                               | 2.66 sec: 1.00x faster                                         |
| pidigits                  | 188 ms                                                                 | 188 ms: 1.00x faster                                           |
| dulwich_log               | 68.0 ms                                                                | 68.4 ms: 1.01x slower                                          |
| json_loads                | 28.1 us                                                                | 28.3 us: 1.01x slower                                          |
| pickle_dict               | 34.0 us                                                                | 34.3 us: 1.01x slower                                          |
| pickle                    | 11.4 us                                                                | 11.5 us: 1.01x slower                                          |
| generators                | 29.5 ms                                                                | 29.7 ms: 1.01x slower                                          |
| python_startup            | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                          |
| python_startup_no_site    | 8.74 ms                                                                | 8.84 ms: 1.01x slower                                          |
| json                      | 5.19 ms                                                                | 5.27 ms: 1.02x slower                                          |
| scimark_lu                | 113 ms                                                                 | 115 ms: 1.02x slower                                           |
| telco                     | 8.51 ms                                                                | 8.65 ms: 1.02x slower                                          |
| nqueens                   | 89.4 ms                                                                | 91.4 ms: 1.02x slower                                          |
| chaos                     | 70.1 ms                                                                | 71.8 ms: 1.02x slower                                          |
| create_gc_cycles          | 1.45 ms                                                                | 1.49 ms: 1.03x slower                                          |
| gc_traversal              | 3.60 ms                                                                | 3.71 ms: 1.03x slower                                          |
| mdp                       | 2.62 sec                                                               | 2.71 sec: 1.03x slower                                         |
| pycparser                 | 1.17 sec                                                               | 1.21 sec: 1.04x slower                                         |
| Geometric mean            | (ref)                                                                  | 1.01x faster                                                   |

Benchmark hidden because not significant (33): scimark_monte_carlo, richards_super, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, deepcopy_reduce, async_tree_none, mypy2, scimark_sor, sqlglot_transpile, sympy_str, dask, scimark_sparse_mat_mult, xml_etree_parse, sqlglot_normalize, float, pickle_list, tornado_http, asyncio_tcp_ssl, xml_etree_iterparse, asyncio_websockets, bench_mp_pool, 2to3, sqlglot_parse, bench_thread_pool, spectral_norm, unpickle_pure_python, xml_etree_process, async_generators, xml_etree_generate, pathlib, typing_runtime_protocols, unpickle, mako


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x