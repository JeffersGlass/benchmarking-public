
# Results vs. 3.11.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 246 ms: 1.15x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.94 ms: 1.36x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.84 sec: 1.14x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.4 ms: 1.22x faster                                                           |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 248 ms: 1.38x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 311 ms: 1.31x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 234 ms: 1.28x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 584 ms: 1.28x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 297 ms: 1.27x faster                                                            |
| async_tree_io              | 754 ms                                                          | 600 ms: 1.26x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 491 ms: 1.17x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 504 ms: 1.17x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.26x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 80.8 ms: 1.56x faster                                                           |
| float          | 76.1 ms                                                         | 61.6 ms: 1.23x faster                                                           |
| pidigits       | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 121 ms: 1.22x faster                                                            |
| regex_dna      | 122 ms                                                          | 119 ms: 1.02x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.4 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_pure_python   | 309 us                                                          | 216 us: 1.43x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.87 ms: 1.43x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.66 sec: 1.39x faster                                                          |
| unpickle_pure_python | 231 us                                                          | 171 us: 1.35x faster                                                            |
| xml_etree_process    | 55.0 ms                                                         | 42.4 ms: 1.30x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 59.8 ms: 1.20x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.81 us: 1.17x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.1 ms: 1.11x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pickle               | 7.99 us                                                         | 7.77 us: 1.03x faster                                                           |
| json_loads           | 20.0 us                                                         | 19.8 us: 1.01x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 20.2 us: 1.01x slower                                                           |
| unpickle             | 9.23 us                                                         | 9.86 us: 1.07x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.16x faster                                                                    |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.1 ms: 1.01x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 19.9 ms: 1.06x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.03x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.65 ms: 1.34x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 94.3 us: 5.08x faster                                                           |
| generators                 | 52.2 ms                                                         | 23.2 ms: 2.25x faster                                                           |
| logging_silent             | 119 ns                                                          | 61.6 ns: 1.94x faster                                                           |
| richards_super             | 58.7 ms                                                         | 33.2 ms: 1.77x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.43 ms: 1.68x faster                                                           |
| richards                   | 48.8 ms                                                         | 29.6 ms: 1.65x faster                                                           |
| chaos                      | 84.4 ms                                                         | 52.2 ms: 1.62x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 25.0 us: 1.60x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.9 ms: 1.60x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 948 us: 1.57x faster                                                            |
| nbody                      | 126 ms                                                          | 80.8 ms: 1.56x faster                                                           |
| spectral_norm              | 122 ms                                                          | 78.4 ms: 1.55x faster                                                           |
| comprehensions             | 22.1 us                                                         | 14.4 us: 1.53x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.20 ms: 1.49x faster                                                           |
| fannkuch                   | 399 ms                                                          | 277 ms: 1.44x faster                                                            |
| scimark_sor                | 135 ms                                                          | 93.9 ms: 1.44x faster                                                           |
| crypto_pyaes               | 79.4 ms                                                         | 55.4 ms: 1.43x faster                                                           |
| raytrace                   | 327 ms                                                          | 229 ms: 1.43x faster                                                            |
| pickle_pure_python         | 309 us                                                          | 216 us: 1.43x faster                                                            |
| json_dumps                 | 9.80 ms                                                         | 6.87 ms: 1.43x faster                                                           |
| nqueens                    | 111 ms                                                          | 80.1 ms: 1.39x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.66 sec: 1.39x faster                                                          |
| async_tree_none            | 343 ms                                                          | 248 ms: 1.38x faster                                                            |
| scimark_fft                | 291 ms                                                          | 212 ms: 1.38x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.10 ms: 1.37x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 5.94 ms: 1.36x faster                                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.25 sec: 1.36x faster                                                          |
| unpickle_pure_python       | 231 us                                                          | 171 us: 1.35x faster                                                            |
| pyflate                    | 471 ms                                                          | 348 ms: 1.35x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 52.5 ms: 1.35x faster                                                           |
| logging_simple             | 10.8 us                                                         | 8.02 us: 1.35x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 608 ms: 1.35x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 111 ms: 1.34x faster                                                            |
| mako                       | 10.3 ms                                                         | 7.65 ms: 1.34x faster                                                           |
| deepcopy                   | 381 us                                                          | 285 us: 1.34x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.59 us: 1.33x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.50 us: 1.33x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 311 ms: 1.31x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 42.4 ms: 1.30x faster                                                           |
| sympy_str                  | 283 ms                                                          | 218 ms: 1.30x faster                                                            |
| hexiom                     | 7.51 ms                                                         | 5.80 ms: 1.30x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 79.3 ms: 1.29x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 50.7 ns: 1.29x faster                                                           |
| async_tree_none_tg         | 301 ms                                                          | 234 ms: 1.28x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 584 ms: 1.28x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 297 ms: 1.27x faster                                                            |
| go                         | 147 ms                                                          | 116 ms: 1.27x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 15.8 ms: 1.26x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 624 ms: 1.26x faster                                                            |
| async_tree_io              | 754 ms                                                          | 600 ms: 1.26x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.66 sec: 1.24x faster                                                          |
| float                      | 76.1 ms                                                         | 61.6 ms: 1.23x faster                                                           |
| regex_compile              | 148 ms                                                          | 121 ms: 1.22x faster                                                            |
| tornado_http               | 118 ms                                                          | 97.4 ms: 1.22x faster                                                           |
| sympy_expand               | 462 ms                                                          | 383 ms: 1.21x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 59.8 ms: 1.20x faster                                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 43.3 ms: 1.20x faster                                                           |
| pycparser                  | 1.04 sec                                                        | 879 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 491 ms: 1.17x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 504 ms: 1.17x faster                                                            |
| unpickle_list              | 3.28 us                                                         | 2.81 us: 1.17x faster                                                           |
| 2to3                       | 282 ms                                                          | 246 ms: 1.15x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.84 sec: 1.14x faster                                                          |
| meteor_contest             | 90.9 ms                                                         | 80.7 ms: 1.13x faster                                                           |
| json                       | 4.78 ms                                                         | 4.25 ms: 1.13x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.1 ms: 1.11x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.04 ms: 1.09x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 2.00 us: 1.07x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pickle                     | 7.99 us                                                         | 7.77 us: 1.03x faster                                                           |
| pidigits                   | 203 ms                                                          | 198 ms: 1.03x faster                                                            |
| regex_dna                  | 122 ms                                                          | 119 ms: 1.02x faster                                                            |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.9 sec: 1.01x faster                                                          |
| json_loads                 | 20.0 us                                                         | 19.8 us: 1.01x faster                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 70.1 ms: 1.01x faster                                                           |
| pickle_dict                | 20.1 us                                                         | 20.2 us: 1.01x slower                                                           |
| python_startup             | 22.0 ms                                                         | 22.1 ms: 1.01x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.41 ms: 1.03x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 19.9 ms: 1.06x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 658 us: 1.06x slower                                                            |
| unpickle                   | 9.23 us                                                         | 9.86 us: 1.07x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 85.8 ms: 1.07x slower                                                           |
| async_generators           | 260 ms                                                          | 280 ms: 1.08x slower                                                            |
| regex_v8                   | 15.2 ms                                                         | 16.4 ms: 1.08x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.08 ms: 1.15x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 225 ms: 1.99x slower                                                            |
| coverage                   | 58.0 ms                                                         | 470 ms: 8.09x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                    |

Benchmark hidden because not significant (1): pickle_list
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: unknown