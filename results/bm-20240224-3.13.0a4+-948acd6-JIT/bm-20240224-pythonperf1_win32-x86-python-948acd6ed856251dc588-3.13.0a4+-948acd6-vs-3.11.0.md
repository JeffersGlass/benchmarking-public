
# Results vs. 3.11.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 268 ms: 1.06x faster                                                            |
| chameleon      | 8.08 ms                                                         | 6.29 ms: 1.28x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.93 sec: 1.09x faster                                                          |
| tornado_http   | 118 ms                                                          | 99.6 ms: 1.19x faster                                                           |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 267 ms: 1.28x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 332 ms: 1.23x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 619 ms: 1.21x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 252 ms: 1.20x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 316 ms: 1.20x faster                                                            |
| async_tree_io              | 754 ms                                                          | 635 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 506 ms: 1.14x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 518 ms: 1.14x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.20x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 55.3 ms: 1.37x faster                                                           |
| nbody          | 126 ms                                                          | 98.2 ms: 1.28x faster                                                           |
| pidigits       | 203 ms                                                          | 199 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 135 ms: 1.09x faster                                                            |
| regex_dna      | 122 ms                                                          | 123 ms: 1.01x slower                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.3 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.01x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.80 ms                                                         | 7.13 ms: 1.37x faster                                                           |
| pickle_pure_python   | 309 us                                                          | 231 us: 1.34x faster                                                            |
| tomli_loads          | 2.31 sec                                                        | 1.74 sec: 1.33x faster                                                          |
| unpickle_pure_python | 231 us                                                          | 178 us: 1.30x faster                                                            |
| xml_etree_process    | 55.0 ms                                                         | 43.7 ms: 1.26x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 61.6 ms: 1.16x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 67.0 ms: 1.13x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.97 us: 1.10x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 108 ms: 1.05x faster                                                            |
| pickle               | 7.99 us                                                         | 7.80 us: 1.02x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.19 us: 1.02x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.8 us: 1.02x faster                                                           |
| json_loads           | 20.0 us                                                         | 20.7 us: 1.03x slower                                                           |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 26.1 ms: 1.19x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 23.7 ms: 1.26x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.22x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.44 ms: 1.38x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 96.3 us: 4.97x faster                                                           |
| generators                 | 52.2 ms                                                         | 23.9 ms: 2.18x faster                                                           |
| logging_silent             | 119 ns                                                          | 67.6 ns: 1.76x faster                                                           |
| spectral_norm              | 122 ms                                                          | 75.0 ms: 1.62x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.9 ms: 1.59x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.75 ms: 1.49x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 27.0 us: 1.48x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 1.04 ms: 1.43x faster                                                           |
| mako                       | 10.3 ms                                                         | 7.44 ms: 1.38x faster                                                           |
| float                      | 76.1 ms                                                         | 55.3 ms: 1.37x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 7.13 ms: 1.37x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.31 ms: 1.37x faster                                                           |
| chaos                      | 84.4 ms                                                         | 62.3 ms: 1.35x faster                                                           |
| comprehensions             | 22.1 us                                                         | 16.4 us: 1.35x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 231 us: 1.34x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.74 sec: 1.33x faster                                                          |
| richards_super             | 58.7 ms                                                         | 44.5 ms: 1.32x faster                                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.24 ms: 1.31x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 178 us: 1.30x faster                                                            |
| deepcopy                   | 381 us                                                          | 294 us: 1.30x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 116 ms: 1.29x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 6.29 ms: 1.28x faster                                                           |
| async_tree_none            | 343 ms                                                          | 267 ms: 1.28x faster                                                            |
| nbody                      | 126 ms                                                          | 98.2 ms: 1.28x faster                                                           |
| crypto_pyaes               | 79.4 ms                                                         | 62.4 ms: 1.27x faster                                                           |
| logging_simple             | 10.8 us                                                         | 8.50 us: 1.27x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 43.7 ms: 1.26x faster                                                           |
| logging_format             | 11.5 us                                                         | 9.10 us: 1.26x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.67 us: 1.24x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 332 ms: 1.23x faster                                                            |
| sympy_str                  | 283 ms                                                          | 232 ms: 1.22x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 619 ms: 1.21x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 653 ms: 1.20x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 252 ms: 1.20x faster                                                            |
| richards                   | 48.8 ms                                                         | 40.8 ms: 1.20x faster                                                           |
| async_tree_memoization_tg  | 378 ms                                                          | 316 ms: 1.20x faster                                                            |
| fannkuch                   | 399 ms                                                          | 335 ms: 1.19x faster                                                            |
| scimark_lu                 | 102 ms                                                          | 86.0 ms: 1.19x faster                                                           |
| nqueens                    | 111 ms                                                          | 93.7 ms: 1.19x faster                                                           |
| tornado_http               | 118 ms                                                          | 99.6 ms: 1.19x faster                                                           |
| async_tree_io              | 754 ms                                                          | 635 ms: 1.19x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 61.6 ms: 1.16x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 17.1 ms: 1.16x faster                                                           |
| pyflate                    | 471 ms                                                          | 406 ms: 1.16x faster                                                            |
| raytrace                   | 327 ms                                                          | 283 ms: 1.16x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 904 ms: 1.15x faster                                                            |
| sympy_expand               | 462 ms                                                          | 402 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 506 ms: 1.14x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 518 ms: 1.14x faster                                                            |
| json                       | 4.78 ms                                                         | 4.21 ms: 1.13x faster                                                           |
| scimark_fft                | 291 ms                                                          | 257 ms: 1.13x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 67.0 ms: 1.13x faster                                                           |
| scimark_sor                | 135 ms                                                          | 120 ms: 1.13x faster                                                            |
| unpickle_list              | 3.28 us                                                         | 2.97 us: 1.10x faster                                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 47.0 ms: 1.10x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 1.96 us: 1.10x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.03 ms: 1.10x faster                                                           |
| regex_compile              | 148 ms                                                          | 135 ms: 1.09x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.93 sec: 1.09x faster                                                          |
| pprint_pformat             | 1.70 sec                                                        | 1.56 sec: 1.09x faster                                                          |
| pprint_safe_repr           | 819 ms                                                          | 760 ms: 1.08x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.92 sec: 1.08x faster                                                          |
| 2to3                       | 282 ms                                                          | 268 ms: 1.06x faster                                                            |
| xml_etree_parse            | 114 ms                                                          | 108 ms: 1.05x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 86.6 ms: 1.05x faster                                                           |
| scimark_monte_carlo        | 70.8 ms                                                         | 67.5 ms: 1.05x faster                                                           |
| go                         | 147 ms                                                          | 142 ms: 1.04x faster                                                            |
| pickle                     | 7.99 us                                                         | 7.80 us: 1.02x faster                                                           |
| pickle_list                | 3.27 us                                                         | 3.19 us: 1.02x faster                                                           |
| pidigits                   | 203 ms                                                          | 199 ms: 1.02x faster                                                            |
| pickle_dict                | 20.1 us                                                         | 19.8 us: 1.02x faster                                                           |
| regex_dna                  | 122 ms                                                          | 123 ms: 1.01x slower                                                            |
| json_loads                 | 20.0 us                                                         | 20.7 us: 1.03x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 649 us: 1.05x slower                                                            |
| hexiom                     | 7.51 ms                                                         | 7.89 ms: 1.05x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 74.8 ms: 1.06x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 85.0 ms: 1.06x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.3 ms: 1.07x slower                                                           |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.09x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.21 ms: 1.17x slower                                                           |
| python_startup             | 22.0 ms                                                         | 26.1 ms: 1.19x slower                                                           |
| async_generators           | 260 ms                                                          | 319 ms: 1.23x slower                                                            |
| python_startup_no_site     | 18.8 ms                                                         | 23.7 ms: 1.26x slower                                                           |
| unpack_sequence            | 65.2 ns                                                         | 85.7 ns: 1.31x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 241 ms: 2.13x slower                                                            |
| coverage                   | 58.0 ms                                                         | 496 ms: 8.54x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (2): asyncio_tcp_ssl, gc_traversal
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown