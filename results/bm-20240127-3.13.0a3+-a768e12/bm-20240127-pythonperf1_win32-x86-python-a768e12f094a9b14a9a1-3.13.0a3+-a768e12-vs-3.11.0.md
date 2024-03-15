
# Results vs. 3.11.0

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-x86
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.28x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 241 ms: 1.17x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.74 ms: 1.41x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.73 sec: 1.21x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.8 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 257 ms: 1.33x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 324 ms: 1.26x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 308 ms: 1.22x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 615 ms: 1.21x faster                                                            |
| async_tree_io              | 754 ms                                                          | 627 ms: 1.20x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 522 ms: 1.13x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 520 ms: 1.11x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.21x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 74.8 ms: 1.68x faster                                                           |
| float          | 76.1 ms                                                         | 54.5 ms: 1.40x faster                                                           |
| pidigits       | 203 ms                                                          | 199 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                           | 1.34x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 97.1 ms: 1.52x faster                                                           |
| regex_dna      | 122 ms                                                          | 123 ms: 1.01x slower                                                            |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.05x slower                                                           |
| regex_effbot   | 1.82 ms                                                         | 1.94 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.08x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 140 us: 1.65x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 198 us: 1.56x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.71 ms: 1.46x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.62 sec: 1.43x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 40.9 ms: 1.35x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 59.0 ms: 1.21x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.3 ms: 1.11x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 3.05 us: 1.08x faster                                                           |
| pickle               | 7.99 us                                                         | 7.79 us: 1.02x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 112 ms: 1.02x faster                                                            |
| pickle_list          | 3.27 us                                                         | 3.25 us: 1.01x faster                                                           |
| json_loads           | 20.0 us                                                         | 20.4 us: 1.02x slower                                                           |
| unpickle             | 9.23 us                                                         | 10.0 us: 1.08x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.18x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.9 ms: 1.09x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 21.5 ms: 1.15x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.12x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.12 ms: 1.44x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 89.6 us: 5.34x faster                                                           |
| generators                 | 52.2 ms                                                         | 22.6 ms: 2.31x faster                                                           |
| logging_silent             | 119 ns                                                          | 58.4 ns: 2.04x faster                                                           |
| comprehensions             | 22.1 us                                                         | 11.3 us: 1.95x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 35.7 ns: 1.82x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 4.17 ms: 1.80x faster                                                           |
| spectral_norm              | 122 ms                                                          | 68.1 ms: 1.79x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.34 ms: 1.75x faster                                                           |
| chaos                      | 84.4 ms                                                         | 48.9 ms: 1.73x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 23.3 us: 1.72x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 59.9 ms: 1.71x faster                                                           |
| nbody                      | 126 ms                                                          | 74.8 ms: 1.68x faster                                                           |
| richards_super             | 58.7 ms                                                         | 35.1 ms: 1.67x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 140 us: 1.65x faster                                                            |
| scimark_sor                | 135 ms                                                          | 82.6 ms: 1.64x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 923 us: 1.61x faster                                                            |
| coroutines                 | 23.7 ms                                                         | 14.9 ms: 1.59x faster                                                           |
| richards                   | 48.8 ms                                                         | 30.8 ms: 1.58x faster                                                           |
| nqueens                    | 111 ms                                                          | 70.7 ms: 1.58x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 198 us: 1.56x faster                                                            |
| raytrace                   | 327 ms                                                          | 212 ms: 1.55x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 46.0 ms: 1.54x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.16 ms: 1.54x faster                                                           |
| regex_compile              | 148 ms                                                          | 97.1 ms: 1.52x faster                                                           |
| fannkuch                   | 399 ms                                                          | 269 ms: 1.49x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.23 us: 1.48x faster                                                           |
| pyflate                    | 471 ms                                                          | 319 ms: 1.48x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.15 sec: 1.48x faster                                                          |
| scimark_fft                | 291 ms                                                          | 197 ms: 1.48x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 53.9 ms: 1.47x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 102 ms: 1.46x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 2.90 ms: 1.46x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.71 ms: 1.46x faster                                                           |
| deepcopy                   | 381 us                                                          | 263 us: 1.45x faster                                                            |
| mako                       | 10.3 ms                                                         | 7.12 ms: 1.44x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 569 ms: 1.44x faster                                                            |
| sympy_str                  | 283 ms                                                          | 197 ms: 1.43x faster                                                            |
| go                         | 147 ms                                                          | 103 ms: 1.43x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.62 sec: 1.43x faster                                                          |
| chameleon                  | 8.08 ms                                                         | 5.74 ms: 1.41x faster                                                           |
| float                      | 76.1 ms                                                         | 54.5 ms: 1.40x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 14.3 ms: 1.39x faster                                                           |
| logging_simple             | 10.8 us                                                         | 7.88 us: 1.37x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.43 us: 1.36x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 40.9 ms: 1.35x faster                                                           |
| sympy_expand               | 462 ms                                                          | 344 ms: 1.34x faster                                                            |
| async_tree_none            | 343 ms                                                          | 257 ms: 1.33x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 791 ms: 1.32x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 39.9 ms: 1.30x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.61 sec: 1.28x faster                                                          |
| async_tree_memoization     | 408 ms                                                          | 324 ms: 1.26x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 308 ms: 1.22x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 59.0 ms: 1.21x faster                                                           |
| async_tree_io_tg           | 746 ms                                                          | 615 ms: 1.21x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.73 sec: 1.21x faster                                                          |
| tornado_http               | 118 ms                                                          | 97.8 ms: 1.21x faster                                                           |
| async_tree_io              | 754 ms                                                          | 627 ms: 1.20x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 75.7 ms: 1.20x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 1.82 us: 1.18x faster                                                           |
| 2to3                       | 282 ms                                                          | 241 ms: 1.17x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 671 ms: 1.17x faster                                                            |
| json                       | 4.78 ms                                                         | 4.08 ms: 1.17x faster                                                           |
| dask                       | 355 ms                                                          | 304 ms: 1.17x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 522 ms: 1.13x faster                                                            |
| bench_thread_pool          | 1.14 ms                                                         | 1.03 ms: 1.11x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 520 ms: 1.11x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.3 ms: 1.11x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 3.05 us: 1.08x faster                                                           |
| pickle                     | 7.99 us                                                         | 7.79 us: 1.02x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 112 ms: 1.02x faster                                                            |
| pidigits                   | 203 ms                                                          | 199 ms: 1.02x faster                                                            |
| pickle_list                | 3.27 us                                                         | 3.25 us: 1.01x faster                                                           |
| regex_dna                  | 122 ms                                                          | 123 ms: 1.01x slower                                                            |
| json_loads                 | 20.0 us                                                         | 20.4 us: 1.02x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.42 ms: 1.03x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| async_generators           | 260 ms                                                          | 269 ms: 1.04x slower                                                            |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.05x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 657 us: 1.06x slower                                                            |
| regex_effbot               | 1.82 ms                                                         | 1.94 ms: 1.06x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 75.4 ms: 1.06x slower                                                           |
| unpickle                   | 9.23 us                                                         | 10.0 us: 1.08x slower                                                           |
| python_startup             | 22.0 ms                                                         | 23.9 ms: 1.09x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 88.8 ms: 1.11x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.97 ms: 1.13x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 21.5 ms: 1.15x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 205 ms: 1.82x slower                                                            |
| coverage                   | 58.0 ms                                                         | 484 ms: 8.34x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.28x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: unknown