
# Results vs. 3.11.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.27x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 241 ms: 1.17x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.62 ms: 1.44x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.77 sec: 1.19x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.5 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 250 ms: 1.37x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 313 ms: 1.30x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 234 ms: 1.29x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 585 ms: 1.28x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 296 ms: 1.27x faster                                                            |
| async_tree_io              | 754 ms                                                          | 602 ms: 1.25x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 495 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 507 ms: 1.16x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.26x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 79.5 ms: 1.58x faster                                                           |
| float          | 76.1 ms                                                         | 56.4 ms: 1.35x faster                                                           |
| pidigits       | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.30x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 104 ms: 1.42x faster                                                            |
| regex_dna      | 122 ms                                                          | 120 ms: 1.01x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.1 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 148 us: 1.56x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 206 us: 1.50x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.72 ms: 1.46x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.65 sec: 1.40x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 40.4 ms: 1.36x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 58.5 ms: 1.22x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 66.3 ms: 1.14x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.89 us: 1.13x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 108 ms: 1.06x faster                                                            |
| pickle               | 7.99 us                                                         | 7.84 us: 1.02x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.9 us: 1.01x faster                                                           |
| json_loads           | 20.0 us                                                         | 19.9 us: 1.01x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.25 us: 1.00x faster                                                           |
| unpickle             | 9.23 us                                                         | 9.82 us: 1.06x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.18x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.1 ms: 1.01x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 19.9 ms: 1.06x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.03x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.57 ms: 1.36x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 88.4 us: 5.41x faster                                                           |
| generators                 | 52.2 ms                                                         | 22.3 ms: 2.34x faster                                                           |
| logging_silent             | 119 ns                                                          | 59.1 ns: 2.02x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.31 ms: 1.77x faster                                                           |
| richards_super             | 58.7 ms                                                         | 33.5 ms: 1.75x faster                                                           |
| comprehensions             | 22.1 us                                                         | 12.6 us: 1.75x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 23.1 us: 1.73x faster                                                           |
| scimark_sor                | 135 ms                                                          | 78.4 ms: 1.73x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 38.6 ns: 1.69x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.2 ms: 1.68x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 905 us: 1.65x faster                                                            |
| scimark_lu                 | 102 ms                                                          | 62.3 ms: 1.64x faster                                                           |
| richards                   | 48.8 ms                                                         | 29.8 ms: 1.64x faster                                                           |
| raytrace                   | 327 ms                                                          | 205 ms: 1.60x faster                                                            |
| nbody                      | 126 ms                                                          | 79.5 ms: 1.58x faster                                                           |
| chaos                      | 84.4 ms                                                         | 53.5 ms: 1.58x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 148 us: 1.56x faster                                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.14 ms: 1.56x faster                                                           |
| spectral_norm              | 122 ms                                                          | 78.1 ms: 1.56x faster                                                           |
| nqueens                    | 111 ms                                                          | 73.6 ms: 1.51x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 206 us: 1.50x faster                                                            |
| hexiom                     | 7.51 ms                                                         | 5.06 ms: 1.48x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.72 ms: 1.46x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 5.62 ms: 1.44x faster                                                           |
| pyflate                    | 471 ms                                                          | 329 ms: 1.43x faster                                                            |
| go                         | 147 ms                                                          | 103 ms: 1.42x faster                                                            |
| regex_compile              | 148 ms                                                          | 104 ms: 1.42x faster                                                            |
| deepcopy                   | 381 us                                                          | 270 us: 1.41x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.65 sec: 1.40x faster                                                          |
| crypto_pyaes               | 79.4 ms                                                         | 56.6 ms: 1.40x faster                                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.22 sec: 1.39x faster                                                          |
| fannkuch                   | 399 ms                                                          | 287 ms: 1.39x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 108 ms: 1.38x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 51.3 ms: 1.38x faster                                                           |
| scimark_fft                | 291 ms                                                          | 211 ms: 1.38x faster                                                            |
| async_tree_none            | 343 ms                                                          | 250 ms: 1.37x faster                                                            |
| pprint_safe_repr           | 819 ms                                                          | 598 ms: 1.37x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 40.4 ms: 1.36x faster                                                           |
| logging_simple             | 10.8 us                                                         | 7.95 us: 1.36x faster                                                           |
| mako                       | 10.3 ms                                                         | 7.57 ms: 1.36x faster                                                           |
| float                      | 76.1 ms                                                         | 56.4 ms: 1.35x faster                                                           |
| sympy_str                  | 283 ms                                                          | 211 ms: 1.34x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.15 ms: 1.34x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.57 us: 1.34x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 15.0 ms: 1.32x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.52 us: 1.31x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 313 ms: 1.30x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 611 ms: 1.29x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 234 ms: 1.29x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 40.4 ms: 1.28x faster                                                           |
| async_tree_io_tg           | 746 ms                                                          | 585 ms: 1.28x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 296 ms: 1.27x faster                                                            |
| sympy_expand               | 462 ms                                                          | 369 ms: 1.25x faster                                                            |
| async_tree_io              | 754 ms                                                          | 602 ms: 1.25x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 837 ms: 1.25x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 58.5 ms: 1.22x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.70 sec: 1.22x faster                                                          |
| tornado_http               | 118 ms                                                          | 97.5 ms: 1.21x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.77 sec: 1.19x faster                                                          |
| meteor_contest             | 90.9 ms                                                         | 76.8 ms: 1.18x faster                                                           |
| dask                       | 355 ms                                                          | 302 ms: 1.17x faster                                                            |
| 2to3                       | 282 ms                                                          | 241 ms: 1.17x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 495 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 507 ms: 1.16x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.86 us: 1.16x faster                                                           |
| json                       | 4.78 ms                                                         | 4.19 ms: 1.14x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 66.3 ms: 1.14x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.00 ms: 1.14x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.89 us: 1.13x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 108 ms: 1.06x faster                                                            |
| pidigits                   | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| bench_mp_pool              | 70.9 ms                                                         | 69.5 ms: 1.02x faster                                                           |
| pickle                     | 7.99 us                                                         | 7.84 us: 1.02x faster                                                           |
| regex_dna                  | 122 ms                                                          | 120 ms: 1.01x faster                                                            |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| pickle_dict                | 20.1 us                                                         | 19.9 us: 1.01x faster                                                           |
| json_loads                 | 20.0 us                                                         | 19.9 us: 1.01x faster                                                           |
| pickle_list                | 3.27 us                                                         | 3.25 us: 1.00x faster                                                           |
| python_startup             | 22.0 ms                                                         | 22.1 ms: 1.01x slower                                                           |
| async_generators           | 260 ms                                                          | 265 ms: 1.02x slower                                                            |
| regex_effbot               | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 646 us: 1.05x slower                                                            |
| pathlib                    | 79.9 ms                                                         | 84.0 ms: 1.05x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 19.9 ms: 1.06x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.1 ms: 1.06x slower                                                           |
| unpickle                   | 9.23 us                                                         | 9.82 us: 1.06x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.86 ms: 1.11x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 207 ms: 1.83x slower                                                            |
| coverage                   | 58.0 ms                                                         | 469 ms: 8.09x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.27x faster                                                                    |

Benchmark hidden because not significant (1): gc_traversal
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: unknown