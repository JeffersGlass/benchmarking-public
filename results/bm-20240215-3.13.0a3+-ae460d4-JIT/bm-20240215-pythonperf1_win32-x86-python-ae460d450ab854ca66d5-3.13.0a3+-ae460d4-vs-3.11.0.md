
# Results vs. 3.11.0

- fork: python
- ref: ae460d450ab854ca66d5
- machine: windows-x86
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 252 ms: 1.12x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.96 ms: 1.35x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.8 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 256 ms: 1.34x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 320 ms: 1.28x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 601 ms: 1.24x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 243 ms: 1.24x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 305 ms: 1.24x faster                                                            |
| async_tree_io              | 754 ms                                                          | 611 ms: 1.23x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 498 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 511 ms: 1.16x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 54.5 ms: 1.40x faster                                                           |
| nbody          | 126 ms                                                          | 92.6 ms: 1.36x faster                                                           |
| pidigits       | 203 ms                                                          | 200 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 108 ms: 1.37x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                    |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| tomli_loads          | 2.31 sec                                                        | 1.61 sec: 1.44x faster                                                          |
| unpickle_pure_python | 231 us                                                          | 161 us: 1.44x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.91 ms: 1.42x faster                                                           |
| pickle_pure_python   | 309 us                                                          | 224 us: 1.38x faster                                                            |
| xml_etree_process    | 55.0 ms                                                         | 43.3 ms: 1.27x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 61.7 ms: 1.16x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.0 ms: 1.11x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 3.08 us: 1.06x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 113 ms: 1.01x faster                                                            |
| json_loads           | 20.0 us                                                         | 20.0 us: 1.00x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 20.0 us: 1.00x faster                                                           |
| pickle               | 7.99 us                                                         | 8.08 us: 1.01x slower                                                           |
| unpickle             | 9.23 us                                                         | 10.3 us: 1.12x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.14x faster                                                                    |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.4 ms: 1.02x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.4 ms: 1.09x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.31 ms: 1.41x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 98.1 us: 4.88x faster                                                           |
| generators                 | 52.2 ms                                                         | 24.7 ms: 2.11x faster                                                           |
| logging_silent             | 119 ns                                                          | 66.7 ns: 1.79x faster                                                           |
| spectral_norm              | 122 ms                                                          | 70.6 ms: 1.72x faster                                                           |
| richards_super             | 58.7 ms                                                         | 35.6 ms: 1.65x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.57 ms: 1.60x faster                                                           |
| richards                   | 48.8 ms                                                         | 31.2 ms: 1.56x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 15.2 ms: 1.56x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 960 us: 1.55x faster                                                            |
| comprehensions             | 22.1 us                                                         | 14.3 us: 1.55x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 26.4 us: 1.52x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 69.1 ms: 1.48x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.21 ms: 1.47x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.61 sec: 1.44x faster                                                          |
| unpickle_pure_python       | 231 us                                                          | 161 us: 1.44x faster                                                            |
| scimark_sor                | 135 ms                                                          | 94.1 ms: 1.44x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.91 ms: 1.42x faster                                                           |
| chaos                      | 84.4 ms                                                         | 60.0 ms: 1.41x faster                                                           |
| mako                       | 10.3 ms                                                         | 7.31 ms: 1.41x faster                                                           |
| float                      | 76.1 ms                                                         | 54.5 ms: 1.40x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 46.9 ns: 1.39x faster                                                           |
| raytrace                   | 327 ms                                                          | 237 ms: 1.38x faster                                                            |
| pickle_pure_python         | 309 us                                                          | 224 us: 1.38x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 109 ms: 1.37x faster                                                            |
| regex_compile              | 148 ms                                                          | 108 ms: 1.37x faster                                                            |
| nbody                      | 126 ms                                                          | 92.6 ms: 1.36x faster                                                           |
| deepcopy                   | 381 us                                                          | 280 us: 1.36x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.96 ms: 1.35x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.45 us: 1.35x faster                                                           |
| async_tree_none            | 343 ms                                                          | 256 ms: 1.34x faster                                                            |
| sympy_str                  | 283 ms                                                          | 214 ms: 1.33x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.20 ms: 1.32x faster                                                           |
| logging_simple             | 10.8 us                                                         | 8.25 us: 1.31x faster                                                           |
| fannkuch                   | 399 ms                                                          | 306 ms: 1.31x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 61.5 ms: 1.29x faster                                                           |
| nqueens                    | 111 ms                                                          | 87.0 ms: 1.28x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.95 us: 1.28x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 320 ms: 1.28x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 617 ms: 1.28x faster                                                            |
| pyflate                    | 471 ms                                                          | 370 ms: 1.27x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 43.3 ms: 1.27x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 15.7 ms: 1.27x faster                                                           |
| async_tree_io_tg           | 746 ms                                                          | 601 ms: 1.24x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 243 ms: 1.24x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 305 ms: 1.24x faster                                                            |
| sympy_expand               | 462 ms                                                          | 374 ms: 1.24x faster                                                            |
| async_tree_io              | 754 ms                                                          | 611 ms: 1.23x faster                                                            |
| go                         | 147 ms                                                          | 120 ms: 1.23x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 861 ms: 1.21x faster                                                            |
| tornado_http               | 118 ms                                                          | 97.8 ms: 1.21x faster                                                           |
| scimark_fft                | 291 ms                                                          | 242 ms: 1.21x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 43.5 ms: 1.19x faster                                                           |
| dask                       | 355 ms                                                          | 301 ms: 1.18x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.45 sec: 1.17x faster                                                          |
| pprint_safe_repr           | 819 ms                                                          | 703 ms: 1.17x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                          |
| xml_etree_generate         | 71.6 ms                                                         | 61.7 ms: 1.16x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 498 ms: 1.16x faster                                                            |
| hexiom                     | 7.51 ms                                                         | 6.50 ms: 1.16x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 511 ms: 1.16x faster                                                            |
| json                       | 4.78 ms                                                         | 4.19 ms: 1.14x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.82 sec: 1.14x faster                                                          |
| sqlite_synth               | 2.15 us                                                         | 1.89 us: 1.13x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.01 ms: 1.12x faster                                                           |
| 2to3                       | 282 ms                                                          | 252 ms: 1.12x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.0 ms: 1.11x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 84.2 ms: 1.08x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 3.08 us: 1.06x faster                                                           |
| pidigits                   | 203 ms                                                          | 200 ms: 1.02x faster                                                            |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.02x faster                                                          |
| xml_etree_parse            | 114 ms                                                          | 113 ms: 1.01x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 70.2 ms: 1.01x faster                                                           |
| json_loads                 | 20.0 us                                                         | 20.0 us: 1.00x faster                                                           |
| pickle_dict                | 20.1 us                                                         | 20.0 us: 1.00x faster                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 71.2 ms: 1.00x slower                                                           |
| pickle                     | 7.99 us                                                         | 8.08 us: 1.01x slower                                                           |
| python_startup             | 22.0 ms                                                         | 22.4 ms: 1.02x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 646 us: 1.05x slower                                                            |
| pathlib                    | 79.9 ms                                                         | 84.3 ms: 1.05x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.4 ms: 1.09x slower                                                           |
| async_generators           | 260 ms                                                          | 290 ms: 1.12x slower                                                            |
| unpickle                   | 9.23 us                                                         | 10.3 us: 1.12x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.11 ms: 1.15x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 224 ms: 1.98x slower                                                            |
| coverage                   | 58.0 ms                                                         | 483 ms: 8.33x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.20x faster                                                                    |

Benchmark hidden because not significant (3): gc_traversal, pickle_list, regex_dna
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown