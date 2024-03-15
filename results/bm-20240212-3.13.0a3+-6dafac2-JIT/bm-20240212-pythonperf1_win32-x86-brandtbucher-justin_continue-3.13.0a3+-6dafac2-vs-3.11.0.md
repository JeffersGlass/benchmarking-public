
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_continue
- machine: windows-x86
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 247 ms: 1.14x faster                                                             |
| chameleon      | 8.08 ms                                                         | 5.91 ms: 1.37x faster                                                            |
| docutils       | 2.10 sec                                                        | 1.77 sec: 1.19x faster                                                           |
| tornado_http   | 118 ms                                                          | 96.4 ms: 1.23x faster                                                            |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 250 ms: 1.37x faster                                                             |
| async_tree_memoization     | 408 ms                                                          | 313 ms: 1.30x faster                                                             |
| async_tree_io_tg           | 746 ms                                                          | 590 ms: 1.26x faster                                                             |
| async_tree_none_tg         | 301 ms                                                          | 239 ms: 1.26x faster                                                             |
| async_tree_io              | 754 ms                                                          | 601 ms: 1.25x faster                                                             |
| async_tree_memoization_tg  | 378 ms                                                          | 302 ms: 1.25x faster                                                             |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 510 ms: 1.16x faster                                                             |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 501 ms: 1.15x faster                                                             |
| Geometric mean             | (ref)                                                           | 1.25x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 53.8 ms: 1.41x faster                                                            |
| nbody          | 126 ms                                                          | 93.5 ms: 1.35x faster                                                            |
| pidigits       | 203 ms                                                          | 201 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 103 ms: 1.43x faster                                                             |
| regex_dna      | 122 ms                                                          | 123 ms: 1.01x slower                                                             |
| regex_effbot   | 1.82 ms                                                         | 1.91 ms: 1.05x slower                                                            |
| regex_v8       | 15.2 ms                                                         | 16.1 ms: 1.06x slower                                                            |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 155 us: 1.50x faster                                                             |
| pickle_pure_python   | 309 us                                                          | 210 us: 1.47x faster                                                             |
| tomli_loads          | 2.31 sec                                                        | 1.60 sec: 1.45x faster                                                           |
| json_dumps           | 9.80 ms                                                         | 6.84 ms: 1.43x faster                                                            |
| xml_etree_process    | 55.0 ms                                                         | 41.5 ms: 1.33x faster                                                            |
| xml_etree_generate   | 71.6 ms                                                         | 58.4 ms: 1.23x faster                                                            |
| unpickle_list        | 3.28 us                                                         | 2.82 us: 1.16x faster                                                            |
| xml_etree_iterparse  | 75.6 ms                                                         | 67.8 ms: 1.11x faster                                                            |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                             |
| pickle_dict          | 20.1 us                                                         | 19.7 us: 1.02x faster                                                            |
| pickle_list          | 3.27 us                                                         | 3.37 us: 1.03x slower                                                            |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.10x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.17x faster                                                                     |

Benchmark hidden because not significant (2): pickle, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.3 ms: 1.01x slower                                                            |
| python_startup_no_site | 18.8 ms                                                         | 20.2 ms: 1.07x slower                                                            |
| Geometric mean         | (ref)                                                           | 1.04x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.60 ms: 1.35x faster                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 94.9 us: 5.04x faster                                                            |
| generators                 | 52.2 ms                                                         | 22.5 ms: 2.32x faster                                                            |
| logging_silent             | 119 ns                                                          | 61.0 ns: 1.96x faster                                                            |
| richards_super             | 58.7 ms                                                         | 33.5 ms: 1.75x faster                                                            |
| deltablue                  | 4.10 ms                                                         | 2.37 ms: 1.73x faster                                                            |
| richards                   | 48.8 ms                                                         | 28.5 ms: 1.71x faster                                                            |
| deepcopy_memo              | 40.0 us                                                         | 23.6 us: 1.70x faster                                                            |
| scimark_lu                 | 102 ms                                                          | 60.5 ms: 1.69x faster                                                            |
| coroutines                 | 23.7 ms                                                         | 14.4 ms: 1.65x faster                                                            |
| sqlglot_parse              | 1.49 ms                                                         | 920 us: 1.62x faster                                                             |
| scimark_sor                | 135 ms                                                          | 83.5 ms: 1.62x faster                                                            |
| spectral_norm              | 122 ms                                                          | 75.5 ms: 1.61x faster                                                            |
| unpack_sequence            | 65.2 ns                                                         | 41.3 ns: 1.58x faster                                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.16 ms: 1.54x faster                                                            |
| unpickle_pure_python       | 231 us                                                          | 155 us: 1.50x faster                                                             |
| comprehensions             | 22.1 us                                                         | 15.0 us: 1.48x faster                                                            |
| pickle_pure_python         | 309 us                                                          | 210 us: 1.47x faster                                                             |
| raytrace                   | 327 ms                                                          | 224 ms: 1.46x faster                                                             |
| tomli_loads                | 2.31 sec                                                        | 1.60 sec: 1.45x faster                                                           |
| chaos                      | 84.4 ms                                                         | 58.5 ms: 1.44x faster                                                            |
| json_dumps                 | 9.80 ms                                                         | 6.84 ms: 1.43x faster                                                            |
| regex_compile              | 148 ms                                                          | 103 ms: 1.43x faster                                                             |
| float                      | 76.1 ms                                                         | 53.8 ms: 1.41x faster                                                            |
| deepcopy                   | 381 us                                                          | 277 us: 1.37x faster                                                             |
| async_tree_none            | 343 ms                                                          | 250 ms: 1.37x faster                                                             |
| chameleon                  | 8.08 ms                                                         | 5.91 ms: 1.37x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.43 us: 1.36x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 110 ms: 1.36x faster                                                             |
| mako                       | 10.3 ms                                                         | 7.60 ms: 1.35x faster                                                            |
| logging_simple             | 10.8 us                                                         | 8.01 us: 1.35x faster                                                            |
| nbody                      | 126 ms                                                          | 93.5 ms: 1.35x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.60 us: 1.33x faster                                                            |
| sympy_str                  | 283 ms                                                          | 213 ms: 1.33x faster                                                             |
| xml_etree_process          | 55.0 ms                                                         | 41.5 ms: 1.33x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.22 ms: 1.31x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 313 ms: 1.30x faster                                                             |
| crypto_pyaes               | 79.4 ms                                                         | 61.4 ms: 1.29x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 15.6 ms: 1.27x faster                                                            |
| go                         | 147 ms                                                          | 116 ms: 1.27x faster                                                             |
| pycparser                  | 1.04 sec                                                        | 821 ms: 1.27x faster                                                             |
| pyflate                    | 471 ms                                                          | 372 ms: 1.27x faster                                                             |
| fannkuch                   | 399 ms                                                          | 315 ms: 1.27x faster                                                             |
| async_tree_io_tg           | 746 ms                                                          | 590 ms: 1.26x faster                                                             |
| sympy_expand               | 462 ms                                                          | 366 ms: 1.26x faster                                                             |
| async_tree_none_tg         | 301 ms                                                          | 239 ms: 1.26x faster                                                             |
| asyncio_tcp                | 787 ms                                                          | 627 ms: 1.25x faster                                                             |
| async_tree_io              | 754 ms                                                          | 601 ms: 1.25x faster                                                             |
| async_tree_memoization_tg  | 378 ms                                                          | 302 ms: 1.25x faster                                                             |
| sqlglot_optimize           | 51.8 ms                                                         | 42.1 ms: 1.23x faster                                                            |
| tornado_http               | 118 ms                                                          | 96.4 ms: 1.23x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 58.4 ms: 1.23x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.39 sec: 1.22x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 670 ms: 1.22x faster                                                             |
| nqueens                    | 111 ms                                                          | 91.6 ms: 1.22x faster                                                            |
| dask                       | 355 ms                                                          | 296 ms: 1.20x faster                                                             |
| hexiom                     | 7.51 ms                                                         | 6.30 ms: 1.19x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.77 sec: 1.19x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.82 us: 1.16x faster                                                            |
| scimark_fft                | 291 ms                                                          | 251 ms: 1.16x faster                                                             |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 510 ms: 1.16x faster                                                             |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 501 ms: 1.15x faster                                                             |
| 2to3                       | 282 ms                                                          | 247 ms: 1.14x faster                                                             |
| json                       | 4.78 ms                                                         | 4.19 ms: 1.14x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.89 us: 1.14x faster                                                            |
| bench_thread_pool          | 1.14 ms                                                         | 1.01 ms: 1.13x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 67.8 ms: 1.11x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.86 sec: 1.11x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 82.0 ms: 1.11x faster                                                            |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                             |
| scimark_monte_carlo        | 70.8 ms                                                         | 68.3 ms: 1.04x faster                                                            |
| pickle_dict                | 20.1 us                                                         | 19.7 us: 1.02x faster                                                            |
| pidigits                   | 203 ms                                                          | 201 ms: 1.01x faster                                                             |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.9 sec: 1.01x faster                                                           |
| regex_dna                  | 122 ms                                                          | 123 ms: 1.01x slower                                                             |
| python_startup             | 22.0 ms                                                         | 22.3 ms: 1.01x slower                                                            |
| pickle_list                | 3.27 us                                                         | 3.37 us: 1.03x slower                                                            |
| create_gc_cycles           | 618 us                                                          | 646 us: 1.05x slower                                                             |
| regex_effbot               | 1.82 ms                                                         | 1.91 ms: 1.05x slower                                                            |
| pathlib                    | 79.9 ms                                                         | 84.1 ms: 1.05x slower                                                            |
| regex_v8                   | 15.2 ms                                                         | 16.1 ms: 1.06x slower                                                            |
| async_generators           | 260 ms                                                          | 277 ms: 1.07x slower                                                             |
| python_startup_no_site     | 18.8 ms                                                         | 20.2 ms: 1.07x slower                                                            |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.10x slower                                                            |
| telco                      | 5.29 ms                                                         | 6.56 ms: 1.24x slower                                                            |
| sqlglot_normalize          | 113 ms                                                          | 215 ms: 1.90x slower                                                             |
| coverage                   | 58.0 ms                                                         | 467 ms: 8.05x slower                                                             |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                     |

Benchmark hidden because not significant (4): bench_mp_pool, pickle, json_loads, gc_traversal
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: unknown