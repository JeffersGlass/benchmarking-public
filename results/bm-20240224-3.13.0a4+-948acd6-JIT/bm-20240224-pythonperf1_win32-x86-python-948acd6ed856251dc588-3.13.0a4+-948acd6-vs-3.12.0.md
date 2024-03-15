
# Results vs. 3.12.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 268 ms: 1.05x faster                                                            |
| chameleon      | 7.75 ms                                                         | 6.29 ms: 1.23x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.93 sec: 1.03x faster                                                          |
| tornado_http   | 105 ms                                                          | 99.6 ms: 1.05x faster                                                           |
| Geometric mean | (ref)                                                           | 1.09x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 267 ms: 1.11x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 316 ms: 1.11x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 252 ms: 1.10x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 332 ms: 1.09x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 619 ms: 1.09x faster                                                            |
| async_tree_io              | 693 ms                                                          | 635 ms: 1.09x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 518 ms: 1.09x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 506 ms: 1.08x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 55.3 ms: 1.39x faster                                                           |
| nbody          | 127 ms                                                          | 98.2 ms: 1.29x faster                                                           |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| regex_dna      | 127 ms                                                          | 123 ms: 1.03x faster                                                            |
| regex_compile  | 129 ms                                                          | 135 ms: 1.04x slower                                                            |
| regex_v8       | 15.0 ms                                                         | 16.3 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.00x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| tomli_loads          | 2.20 sec                                                        | 1.74 sec: 1.26x faster                                                          |
| pickle_pure_python   | 286 us                                                          | 231 us: 1.24x faster                                                            |
| xml_etree_process    | 53.2 ms                                                         | 43.7 ms: 1.22x faster                                                           |
| unpickle_pure_python | 210 us                                                          | 178 us: 1.18x faster                                                            |
| xml_etree_generate   | 72.1 ms                                                         | 61.6 ms: 1.17x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 67.0 ms: 1.16x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.19 us: 1.05x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 108 ms: 1.04x faster                                                            |
| json_dumps           | 7.40 ms                                                         | 7.13 ms: 1.04x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 19.8 us: 1.01x faster                                                           |
| json_loads           | 20.4 us                                                         | 20.7 us: 1.02x slower                                                           |
| unpickle             | 9.71 us                                                         | 10.1 us: 1.04x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                    |

Benchmark hidden because not significant (2): pickle, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 26.1 ms: 1.17x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 23.7 ms: 1.24x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.20x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.44 ms: 1.34x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 23.9 ms: 1.61x faster                                                           |
| logging_silent             | 101 ns                                                          | 67.6 ns: 1.49x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 27.0 us: 1.42x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.9 ms: 1.40x faster                                                           |
| float                      | 76.7 ms                                                         | 55.3 ms: 1.39x faster                                                           |
| spectral_norm              | 104 ms                                                          | 75.0 ms: 1.38x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.44 ms: 1.34x faster                                                           |
| typing_runtime_protocols   | 126 us                                                          | 96.3 us: 1.31x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.75 ms: 1.30x faster                                                           |
| nbody                      | 127 ms                                                          | 98.2 ms: 1.29x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.74 sec: 1.26x faster                                                          |
| pickle_pure_python         | 286 us                                                          | 231 us: 1.24x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 6.29 ms: 1.23x faster                                                           |
| deepcopy                   | 360 us                                                          | 294 us: 1.23x faster                                                            |
| xml_etree_process          | 53.2 ms                                                         | 43.7 ms: 1.22x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.67 us: 1.21x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 1.04 ms: 1.19x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.24 ms: 1.19x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 178 us: 1.18x faster                                                            |
| comprehensions             | 19.2 us                                                         | 16.4 us: 1.17x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 61.6 ms: 1.17x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.31 ms: 1.17x faster                                                           |
| xml_etree_iterparse        | 77.6 ms                                                         | 67.0 ms: 1.16x faster                                                           |
| logging_simple             | 9.75 us                                                         | 8.50 us: 1.15x faster                                                           |
| logging_format             | 10.4 us                                                         | 9.10 us: 1.14x faster                                                           |
| async_tree_none            | 298 ms                                                          | 267 ms: 1.11x faster                                                            |
| chaos                      | 69.4 ms                                                         | 62.3 ms: 1.11x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 62.4 ms: 1.11x faster                                                           |
| async_tree_memoization_tg  | 350 ms                                                          | 316 ms: 1.11x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 252 ms: 1.10x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 332 ms: 1.09x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 619 ms: 1.09x faster                                                            |
| async_tree_io              | 693 ms                                                          | 635 ms: 1.09x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 518 ms: 1.09x faster                                                            |
| raytrace                   | 308 ms                                                          | 283 ms: 1.09x faster                                                            |
| scimark_lu                 | 93.2 ms                                                         | 86.0 ms: 1.08x faster                                                           |
| scimark_sor                | 130 ms                                                          | 120 ms: 1.08x faster                                                            |
| pycparser                  | 978 ms                                                          | 904 ms: 1.08x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 506 ms: 1.08x faster                                                            |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 85.0 ms: 1.07x faster                                                           |
| bench_thread_pool          | 1.10 ms                                                         | 1.03 ms: 1.07x faster                                                           |
| sympy_sum                  | 123 ms                                                          | 116 ms: 1.06x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 1.96 us: 1.06x faster                                                           |
| fannkuch                   | 354 ms                                                          | 335 ms: 1.06x faster                                                            |
| pickle_list                | 3.37 us                                                         | 3.19 us: 1.05x faster                                                           |
| tornado_http               | 105 ms                                                          | 99.6 ms: 1.05x faster                                                           |
| scimark_fft                | 271 ms                                                          | 257 ms: 1.05x faster                                                            |
| 2to3                       | 280 ms                                                          | 268 ms: 1.05x faster                                                            |
| richards_super             | 46.5 ms                                                         | 44.5 ms: 1.04x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 108 ms: 1.04x faster                                                            |
| pyflate                    | 424 ms                                                          | 406 ms: 1.04x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.39 ms: 1.04x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 17.0 sec: 1.04x faster                                                          |
| json_dumps                 | 7.40 ms                                                         | 7.13 ms: 1.04x faster                                                           |
| sympy_str                  | 240 ms                                                          | 232 ms: 1.03x faster                                                            |
| regex_dna                  | 127 ms                                                          | 123 ms: 1.03x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 47.0 ms: 1.03x faster                                                           |
| docutils                   | 1.98 sec                                                        | 1.93 sec: 1.03x faster                                                          |
| sympy_integrate            | 17.5 ms                                                         | 17.1 ms: 1.03x faster                                                           |
| richards                   | 41.3 ms                                                         | 40.8 ms: 1.01x faster                                                           |
| pickle_dict                | 19.9 us                                                         | 19.8 us: 1.01x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 74.8 ms: 1.01x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 86.6 ms: 1.00x faster                                                           |
| mdp                        | 1.91 sec                                                        | 1.92 sec: 1.00x slower                                                          |
| sympy_expand               | 398 ms                                                          | 402 ms: 1.01x slower                                                            |
| json                       | 4.15 ms                                                         | 4.21 ms: 1.01x slower                                                           |
| json_loads                 | 20.4 us                                                         | 20.7 us: 1.02x slower                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 67.5 ms: 1.02x slower                                                           |
| async_generators           | 313 ms                                                          | 319 ms: 1.02x slower                                                            |
| go                         | 137 ms                                                          | 142 ms: 1.03x slower                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.56 sec: 1.04x slower                                                          |
| unpickle                   | 9.71 us                                                         | 10.1 us: 1.04x slower                                                           |
| regex_compile              | 129 ms                                                          | 135 ms: 1.04x slower                                                            |
| pprint_safe_repr           | 721 ms                                                          | 760 ms: 1.06x slower                                                            |
| regex_v8                   | 15.0 ms                                                         | 16.3 ms: 1.08x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.21 ms: 1.13x slower                                                           |
| hexiom                     | 6.82 ms                                                         | 7.89 ms: 1.16x slower                                                           |
| python_startup             | 22.4 ms                                                         | 26.1 ms: 1.17x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 23.7 ms: 1.24x slower                                                           |
| unpack_sequence            | 62.5 ns                                                         | 85.7 ns: 1.37x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 241 ms: 2.41x slower                                                            |
| coverage                   | 48.4 ms                                                         | 496 ms: 10.23x slower                                                           |
| Geometric mean             | (ref)                                                           | 1.04x faster                                                                    |

Benchmark hidden because not significant (6): asyncio_tcp, create_gc_cycles, pidigits, nqueens, pickle, unpickle_list
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown