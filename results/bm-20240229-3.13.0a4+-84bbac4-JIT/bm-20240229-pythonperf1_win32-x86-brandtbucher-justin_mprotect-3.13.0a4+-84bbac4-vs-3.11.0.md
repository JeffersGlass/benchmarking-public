# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: windows-x86
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 260 ms: 1.09x faster                                                             |
| chameleon      | 8.08 ms                                                         | 5.66 ms: 1.43x faster                                                            |
| docutils       | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                           |
| tornado_http   | 118 ms                                                          | 96.7 ms: 1.22x faster                                                            |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 258 ms: 1.33x faster                                                             |
| async_tree_memoization     | 408 ms                                                          | 323 ms: 1.27x faster                                                             |
| async_tree_none_tg         | 301 ms                                                          | 242 ms: 1.24x faster                                                             |
| async_tree_memoization_tg  | 378 ms                                                          | 304 ms: 1.24x faster                                                             |
| async_tree_io_tg           | 746 ms                                                          | 605 ms: 1.23x faster                                                             |
| async_tree_io              | 754 ms                                                          | 624 ms: 1.21x faster                                                             |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 504 ms: 1.14x faster                                                             |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 517 ms: 1.14x faster                                                             |
| Geometric mean             | (ref)                                                           | 1.22x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 54.9 ms: 1.39x faster                                                            |
| nbody          | 126 ms                                                          | 96.4 ms: 1.31x faster                                                            |
| pidigits       | 203 ms                                                          | 198 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 109 ms: 1.35x faster                                                             |
| regex_dna      | 122 ms                                                          | 121 ms: 1.01x faster                                                             |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                            |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                            |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 309 us                                                          | 210 us: 1.47x faster                                                             |
| json_dumps           | 9.80 ms                                                         | 6.86 ms: 1.43x faster                                                            |
| unpickle_pure_python | 231 us                                                          | 171 us: 1.35x faster                                                             |
| tomli_loads          | 2.31 sec                                                        | 1.72 sec: 1.34x faster                                                           |
| xml_etree_process    | 55.0 ms                                                         | 42.1 ms: 1.31x faster                                                            |
| xml_etree_generate   | 71.6 ms                                                         | 59.6 ms: 1.20x faster                                                            |
| unpickle_list        | 3.28 us                                                         | 2.81 us: 1.17x faster                                                            |
| xml_etree_iterparse  | 75.6 ms                                                         | 67.3 ms: 1.12x faster                                                            |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.04x faster                                                             |
| pickle_list          | 3.27 us                                                         | 3.17 us: 1.03x faster                                                            |
| pickle               | 7.99 us                                                         | 7.94 us: 1.01x faster                                                            |
| pickle_dict          | 20.1 us                                                         | 20.0 us: 1.00x faster                                                            |
| json_loads           | 20.0 us                                                         | 20.1 us: 1.00x slower                                                            |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.09x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.16x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 25.7 ms: 1.17x slower                                                            |
| python_startup_no_site | 18.8 ms                                                         | 23.6 ms: 1.26x slower                                                            |
| Geometric mean         | (ref)                                                           | 1.21x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.30 ms: 1.41x faster                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 92.1 us: 5.19x faster                                                            |
| generators                 | 52.2 ms                                                         | 23.0 ms: 2.27x faster                                                            |
| logging_silent             | 119 ns                                                          | 59.6 ns: 2.00x faster                                                            |
| spectral_norm              | 122 ms                                                          | 71.2 ms: 1.71x faster                                                            |
| coroutines                 | 23.7 ms                                                         | 14.1 ms: 1.68x faster                                                            |
| deepcopy_memo              | 40.0 us                                                         | 24.3 us: 1.65x faster                                                            |
| deltablue                  | 4.10 ms                                                         | 2.59 ms: 1.58x faster                                                            |
| sqlglot_parse              | 1.49 ms                                                         | 979 us: 1.52x faster                                                             |
| unpack_sequence            | 65.2 ns                                                         | 43.1 ns: 1.51x faster                                                            |
| comprehensions             | 22.1 us                                                         | 14.6 us: 1.51x faster                                                            |
| richards_super             | 58.7 ms                                                         | 39.2 ms: 1.50x faster                                                            |
| pickle_pure_python         | 309 us                                                          | 210 us: 1.47x faster                                                             |
| sqlglot_transpile          | 1.78 ms                                                         | 1.23 ms: 1.45x faster                                                            |
| json_dumps                 | 9.80 ms                                                         | 6.86 ms: 1.43x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.66 ms: 1.43x faster                                                            |
| mako                       | 10.3 ms                                                         | 7.30 ms: 1.41x faster                                                            |
| chaos                      | 84.4 ms                                                         | 60.3 ms: 1.40x faster                                                            |
| richards                   | 48.8 ms                                                         | 34.9 ms: 1.40x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 107 ms: 1.39x faster                                                             |
| float                      | 76.1 ms                                                         | 54.9 ms: 1.39x faster                                                            |
| deepcopy                   | 381 us                                                          | 278 us: 1.37x faster                                                             |
| scimark_sor                | 135 ms                                                          | 100 ms: 1.35x faster                                                             |
| unpickle_pure_python       | 231 us                                                          | 171 us: 1.35x faster                                                             |
| regex_compile              | 148 ms                                                          | 109 ms: 1.35x faster                                                             |
| sympy_str                  | 283 ms                                                          | 210 ms: 1.35x faster                                                             |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.15 ms: 1.34x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.72 sec: 1.34x faster                                                           |
| async_tree_none            | 343 ms                                                          | 258 ms: 1.33x faster                                                             |
| logging_simple             | 10.8 us                                                         | 8.15 us: 1.33x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.51 us: 1.32x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 60.3 ms: 1.32x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.74 us: 1.31x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 42.1 ms: 1.31x faster                                                            |
| nbody                      | 126 ms                                                          | 96.4 ms: 1.31x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 15.4 ms: 1.30x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 323 ms: 1.27x faster                                                             |
| sympy_expand               | 462 ms                                                          | 370 ms: 1.25x faster                                                             |
| scimark_fft                | 291 ms                                                          | 233 ms: 1.25x faster                                                             |
| async_tree_none_tg         | 301 ms                                                          | 242 ms: 1.24x faster                                                             |
| async_tree_memoization_tg  | 378 ms                                                          | 304 ms: 1.24x faster                                                             |
| pyflate                    | 471 ms                                                          | 382 ms: 1.23x faster                                                             |
| async_tree_io_tg           | 746 ms                                                          | 605 ms: 1.23x faster                                                             |
| asyncio_tcp                | 787 ms                                                          | 638 ms: 1.23x faster                                                             |
| scimark_lu                 | 102 ms                                                          | 83.5 ms: 1.23x faster                                                            |
| tornado_http               | 118 ms                                                          | 96.7 ms: 1.22x faster                                                            |
| go                         | 147 ms                                                          | 120 ms: 1.22x faster                                                             |
| nqueens                    | 111 ms                                                          | 91.4 ms: 1.22x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 859 ms: 1.21x faster                                                             |
| hexiom                     | 7.51 ms                                                         | 6.21 ms: 1.21x faster                                                            |
| async_tree_io              | 754 ms                                                          | 624 ms: 1.21x faster                                                             |
| xml_etree_generate         | 71.6 ms                                                         | 59.6 ms: 1.20x faster                                                            |
| raytrace                   | 327 ms                                                          | 275 ms: 1.19x faster                                                             |
| mdp                        | 2.07 sec                                                        | 1.74 sec: 1.19x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.81 us: 1.17x faster                                                            |
| fannkuch                   | 399 ms                                                          | 344 ms: 1.16x faster                                                             |
| docutils                   | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 504 ms: 1.14x faster                                                             |
| sqlglot_optimize           | 51.8 ms                                                         | 45.3 ms: 1.14x faster                                                            |
| json                       | 4.78 ms                                                         | 4.19 ms: 1.14x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 517 ms: 1.14x faster                                                             |
| pprint_pformat             | 1.70 sec                                                        | 1.51 sec: 1.12x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 67.3 ms: 1.12x faster                                                            |
| pprint_safe_repr           | 819 ms                                                          | 735 ms: 1.11x faster                                                             |
| sqlite_synth               | 2.15 us                                                         | 1.93 us: 1.11x faster                                                            |
| bench_thread_pool          | 1.14 ms                                                         | 1.03 ms: 1.10x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 82.8 ms: 1.10x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 64.9 ms: 1.09x faster                                                            |
| 2to3                       | 282 ms                                                          | 260 ms: 1.09x faster                                                             |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.04x faster                                                             |
| pickle_list                | 3.27 us                                                         | 3.17 us: 1.03x faster                                                            |
| pidigits                   | 203 ms                                                          | 198 ms: 1.02x faster                                                             |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.01x faster                                                           |
| regex_dna                  | 122 ms                                                          | 121 ms: 1.01x faster                                                             |
| pickle                     | 7.99 us                                                         | 7.94 us: 1.01x faster                                                            |
| pickle_dict                | 20.1 us                                                         | 20.0 us: 1.00x faster                                                            |
| json_loads                 | 20.0 us                                                         | 20.1 us: 1.00x slower                                                            |
| gc_traversal               | 1.38 ms                                                         | 1.42 ms: 1.03x slower                                                            |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                            |
| bench_mp_pool              | 70.9 ms                                                         | 73.9 ms: 1.04x slower                                                            |
| pathlib                    | 79.9 ms                                                         | 84.2 ms: 1.05x slower                                                            |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                            |
| create_gc_cycles           | 618 us                                                          | 665 us: 1.08x slower                                                             |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.09x slower                                                            |
| async_generators           | 260 ms                                                          | 292 ms: 1.12x slower                                                             |
| dask                       | 355 ms                                                          | 413 ms: 1.16x slower                                                             |
| python_startup             | 22.0 ms                                                         | 25.7 ms: 1.17x slower                                                            |
| telco                      | 5.29 ms                                                         | 6.43 ms: 1.21x slower                                                            |
| python_startup_no_site     | 18.8 ms                                                         | 23.6 ms: 1.26x slower                                                            |
| sqlglot_normalize          | 113 ms                                                          | 216 ms: 1.91x slower                                                             |
| coverage                   | 58.0 ms                                                         | 477 ms: 8.21x slower                                                             |
| Geometric mean             | (ref)                                                           | 1.19x faster                                                                     |
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: unknown