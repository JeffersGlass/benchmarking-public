
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: windows-x86
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.22x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 255 ms: 1.11x faster                                                    |
| chameleon      | 8.08 ms                                                         | 6.09 ms: 1.33x faster                                                   |
| docutils       | 2.10 sec                                                        | 1.82 sec: 1.15x faster                                                  |
| tornado_http   | 118 ms                                                          | 98.2 ms: 1.21x faster                                                   |
| Geometric mean | (ref)                                                           | 1.20x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 257 ms: 1.33x faster                                                    |
| async_tree_memoization     | 408 ms                                                          | 324 ms: 1.26x faster                                                    |
| async_tree_memoization_tg  | 378 ms                                                          | 307 ms: 1.23x faster                                                    |
| async_tree_io_tg           | 746 ms                                                          | 609 ms: 1.23x faster                                                    |
| async_tree_io              | 754 ms                                                          | 617 ms: 1.22x faster                                                    |
| async_tree_none_tg         | 301 ms                                                          | 247 ms: 1.22x faster                                                    |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 520 ms: 1.13x faster                                                    |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 511 ms: 1.13x faster                                                    |
| Geometric mean             | (ref)                                                           | 1.22x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 55.9 ms: 1.36x faster                                                   |
| nbody          | 126 ms                                                          | 93.0 ms: 1.35x faster                                                   |
| pidigits       | 203 ms                                                          | 204 ms: 1.01x slower                                                    |
| Geometric mean | (ref)                                                           | 1.22x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 106 ms: 1.39x faster                                                    |
| regex_dna      | 122 ms                                                          | 120 ms: 1.01x faster                                                    |
| regex_effbot   | 1.82 ms                                                         | 1.92 ms: 1.05x slower                                                   |
| regex_v8       | 15.2 ms                                                         | 16.4 ms: 1.08x slower                                                   |
| Geometric mean | (ref)                                                           | 1.05x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 150 us: 1.54x faster                                                    |
| pickle_pure_python   | 309 us                                                          | 205 us: 1.51x faster                                                    |
| json_dumps           | 9.80 ms                                                         | 6.78 ms: 1.45x faster                                                   |
| tomli_loads          | 2.31 sec                                                        | 1.64 sec: 1.41x faster                                                  |
| xml_etree_process    | 55.0 ms                                                         | 41.2 ms: 1.34x faster                                                   |
| xml_etree_generate   | 71.6 ms                                                         | 59.2 ms: 1.21x faster                                                   |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.5 ms: 1.10x faster                                                   |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                    |
| unpickle_list        | 3.28 us                                                         | 3.23 us: 1.02x faster                                                   |
| pickle_dict          | 20.1 us                                                         | 20.0 us: 1.01x faster                                                   |
| pickle               | 7.99 us                                                         | 8.23 us: 1.03x slower                                                   |
| unpickle             | 9.23 us                                                         | 10.2 us: 1.10x slower                                                   |
| Geometric mean       | (ref)                                                           | 1.16x faster                                                            |

Benchmark hidden because not significant (2): pickle_list, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                                   |
| python_startup_no_site | 18.8 ms                                                         | 20.7 ms: 1.10x slower                                                   |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.75 ms: 1.33x faster                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 95.7 us: 5.00x faster                                                   |
| generators                 | 52.2 ms                                                         | 23.2 ms: 2.25x faster                                                   |
| logging_silent             | 119 ns                                                          | 60.0 ns: 1.99x faster                                                   |
| richards_super             | 58.7 ms                                                         | 31.7 ms: 1.85x faster                                                   |
| deepcopy_memo              | 40.0 us                                                         | 22.9 us: 1.75x faster                                                   |
| richards                   | 48.8 ms                                                         | 28.1 ms: 1.74x faster                                                   |
| scimark_lu                 | 102 ms                                                          | 61.4 ms: 1.67x faster                                                   |
| deltablue                  | 4.10 ms                                                         | 2.47 ms: 1.66x faster                                                   |
| sqlglot_parse              | 1.49 ms                                                         | 902 us: 1.65x faster                                                    |
| coroutines                 | 23.7 ms                                                         | 14.4 ms: 1.65x faster                                                   |
| scimark_sor                | 135 ms                                                          | 82.3 ms: 1.64x faster                                                   |
| unpack_sequence            | 65.2 ns                                                         | 40.1 ns: 1.63x faster                                                   |
| sqlglot_transpile          | 1.78 ms                                                         | 1.15 ms: 1.56x faster                                                   |
| spectral_norm              | 122 ms                                                          | 78.1 ms: 1.56x faster                                                   |
| unpickle_pure_python       | 231 us                                                          | 150 us: 1.54x faster                                                    |
| pickle_pure_python         | 309 us                                                          | 205 us: 1.51x faster                                                    |
| comprehensions             | 22.1 us                                                         | 15.1 us: 1.46x faster                                                   |
| raytrace                   | 327 ms                                                          | 225 ms: 1.45x faster                                                    |
| json_dumps                 | 9.80 ms                                                         | 6.78 ms: 1.45x faster                                                   |
| chaos                      | 84.4 ms                                                         | 58.8 ms: 1.44x faster                                                   |
| deepcopy                   | 381 us                                                          | 268 us: 1.42x faster                                                    |
| tomli_loads                | 2.31 sec                                                        | 1.64 sec: 1.41x faster                                                  |
| deepcopy_reduce            | 3.32 us                                                         | 2.39 us: 1.39x faster                                                   |
| regex_compile              | 148 ms                                                          | 106 ms: 1.39x faster                                                    |
| logging_simple             | 10.8 us                                                         | 7.90 us: 1.37x faster                                                   |
| float                      | 76.1 ms                                                         | 55.9 ms: 1.36x faster                                                   |
| sympy_sum                  | 149 ms                                                          | 110 ms: 1.36x faster                                                    |
| nbody                      | 126 ms                                                          | 93.0 ms: 1.35x faster                                                   |
| xml_etree_process          | 55.0 ms                                                         | 41.2 ms: 1.34x faster                                                   |
| async_tree_none            | 343 ms                                                          | 257 ms: 1.33x faster                                                    |
| logging_format             | 11.5 us                                                         | 8.61 us: 1.33x faster                                                   |
| chameleon                  | 8.08 ms                                                         | 6.09 ms: 1.33x faster                                                   |
| sympy_str                  | 283 ms                                                          | 214 ms: 1.33x faster                                                    |
| mako                       | 10.3 ms                                                         | 7.75 ms: 1.33x faster                                                   |
| fannkuch                   | 399 ms                                                          | 302 ms: 1.32x faster                                                    |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.23 ms: 1.31x faster                                                   |
| pyflate                    | 471 ms                                                          | 366 ms: 1.29x faster                                                    |
| nqueens                    | 111 ms                                                          | 86.6 ms: 1.29x faster                                                   |
| sympy_expand               | 462 ms                                                          | 362 ms: 1.28x faster                                                    |
| crypto_pyaes               | 79.4 ms                                                         | 62.5 ms: 1.27x faster                                                   |
| sympy_integrate            | 19.9 ms                                                         | 15.7 ms: 1.26x faster                                                   |
| pycparser                  | 1.04 sec                                                        | 826 ms: 1.26x faster                                                    |
| async_tree_memoization     | 408 ms                                                          | 324 ms: 1.26x faster                                                    |
| go                         | 147 ms                                                          | 117 ms: 1.26x faster                                                    |
| async_tree_memoization_tg  | 378 ms                                                          | 307 ms: 1.23x faster                                                    |
| async_tree_io_tg           | 746 ms                                                          | 609 ms: 1.23x faster                                                    |
| async_tree_io              | 754 ms                                                          | 617 ms: 1.22x faster                                                    |
| async_tree_none_tg         | 301 ms                                                          | 247 ms: 1.22x faster                                                    |
| sqlglot_optimize           | 51.8 ms                                                         | 42.7 ms: 1.21x faster                                                   |
| pprint_safe_repr           | 819 ms                                                          | 676 ms: 1.21x faster                                                    |
| xml_etree_generate         | 71.6 ms                                                         | 59.2 ms: 1.21x faster                                                   |
| pprint_pformat             | 1.70 sec                                                        | 1.40 sec: 1.21x faster                                                  |
| tornado_http               | 118 ms                                                          | 98.2 ms: 1.21x faster                                                   |
| asyncio_tcp                | 787 ms                                                          | 654 ms: 1.20x faster                                                    |
| scimark_fft                | 291 ms                                                          | 249 ms: 1.17x faster                                                    |
| dask                       | 355 ms                                                          | 303 ms: 1.17x faster                                                    |
| hexiom                     | 7.51 ms                                                         | 6.45 ms: 1.16x faster                                                   |
| docutils                   | 2.10 sec                                                        | 1.82 sec: 1.15x faster                                                  |
| json                       | 4.78 ms                                                         | 4.18 ms: 1.14x faster                                                   |
| sqlite_synth               | 2.15 us                                                         | 1.88 us: 1.14x faster                                                   |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 520 ms: 1.13x faster                                                    |
| bench_thread_pool          | 1.14 ms                                                         | 1.01 ms: 1.13x faster                                                   |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 511 ms: 1.13x faster                                                    |
| mdp                        | 2.07 sec                                                        | 1.84 sec: 1.13x faster                                                  |
| 2to3                       | 282 ms                                                          | 255 ms: 1.11x faster                                                    |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.5 ms: 1.10x faster                                                   |
| meteor_contest             | 90.9 ms                                                         | 84.3 ms: 1.08x faster                                                   |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                    |
| unpickle_list              | 3.28 us                                                         | 3.23 us: 1.02x faster                                                   |
| regex_dna                  | 122 ms                                                          | 120 ms: 1.01x faster                                                    |
| pickle_dict                | 20.1 us                                                         | 20.0 us: 1.01x faster                                                   |
| pidigits                   | 203 ms                                                          | 204 ms: 1.01x slower                                                    |
| pickle                     | 7.99 us                                                         | 8.23 us: 1.03x slower                                                   |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                                  |
| bench_mp_pool              | 70.9 ms                                                         | 73.8 ms: 1.04x slower                                                   |
| python_startup             | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                                   |
| gc_traversal               | 1.38 ms                                                         | 1.44 ms: 1.04x slower                                                   |
| regex_effbot               | 1.82 ms                                                         | 1.92 ms: 1.05x slower                                                   |
| create_gc_cycles           | 618 us                                                          | 662 us: 1.07x slower                                                    |
| regex_v8                   | 15.2 ms                                                         | 16.4 ms: 1.08x slower                                                   |
| python_startup_no_site     | 18.8 ms                                                         | 20.7 ms: 1.10x slower                                                   |
| unpickle                   | 9.23 us                                                         | 10.2 us: 1.10x slower                                                   |
| pathlib                    | 79.9 ms                                                         | 89.0 ms: 1.11x slower                                                   |
| telco                      | 5.29 ms                                                         | 5.94 ms: 1.12x slower                                                   |
| async_generators           | 260 ms                                                          | 295 ms: 1.13x slower                                                    |
| sqlglot_normalize          | 113 ms                                                          | 219 ms: 1.93x slower                                                    |
| coverage                   | 58.0 ms                                                         | 499 ms: 8.60x slower                                                    |
| Geometric mean             | (ref)                                                           | 1.22x faster                                                            |

Benchmark hidden because not significant (3): pickle_list, scimark_monte_carlo, json_loads
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown