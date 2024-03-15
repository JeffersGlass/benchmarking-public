
# Results vs. 3.11.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 252 ms: 1.12x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.98 ms: 1.35x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                          |
| tornado_http   | 118 ms                                                          | 98.6 ms: 1.20x faster                                                           |
| Geometric mean | (ref)                                                           | 1.20x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 259 ms: 1.32x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 327 ms: 1.25x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 242 ms: 1.24x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 305 ms: 1.24x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 608 ms: 1.23x faster                                                            |
| async_tree_io              | 754 ms                                                          | 620 ms: 1.22x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 512 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 501 ms: 1.15x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 53.8 ms: 1.42x faster                                                           |
| nbody          | 126 ms                                                          | 94.2 ms: 1.34x faster                                                           |
| pidigits       | 203 ms                                                          | 201 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 108 ms: 1.37x faster                                                            |
| regex_dna      | 122 ms                                                          | 120 ms: 1.02x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.87 ms: 1.03x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 15.7 ms: 1.04x slower                                                           |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 158 us: 1.46x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.88 ms: 1.42x faster                                                           |
| pickle_pure_python   | 309 us                                                          | 219 us: 1.41x faster                                                            |
| tomli_loads          | 2.31 sec                                                        | 1.66 sec: 1.39x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 42.6 ms: 1.29x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 60.8 ms: 1.18x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 65.7 ms: 1.15x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.96 us: 1.10x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 108 ms: 1.06x faster                                                            |
| json_loads           | 20.0 us                                                         | 19.8 us: 1.01x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.28 us: 1.00x slower                                                           |
| pickle               | 7.99 us                                                         | 8.09 us: 1.01x slower                                                           |
| unpickle             | 9.23 us                                                         | 10.3 us: 1.11x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.0 ms: 1.05x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.8 ms: 1.11x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.31 ms: 1.41x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 97.1 us: 4.93x faster                                                           |
| generators                 | 52.2 ms                                                         | 24.5 ms: 2.13x faster                                                           |
| logging_silent             | 119 ns                                                          | 67.7 ns: 1.76x faster                                                           |
| spectral_norm              | 122 ms                                                          | 71.2 ms: 1.71x faster                                                           |
| richards_super             | 58.7 ms                                                         | 35.1 ms: 1.67x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.57 ms: 1.59x faster                                                           |
| comprehensions             | 22.1 us                                                         | 13.9 us: 1.59x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 25.3 us: 1.58x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 15.1 ms: 1.57x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 957 us: 1.56x faster                                                            |
| richards                   | 48.8 ms                                                         | 31.5 ms: 1.55x faster                                                           |
| scimark_sor                | 135 ms                                                          | 88.3 ms: 1.53x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 68.4 ms: 1.50x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 44.1 ns: 1.48x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.21 ms: 1.48x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 158 us: 1.46x faster                                                            |
| chaos                      | 84.4 ms                                                         | 59.0 ms: 1.43x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.88 ms: 1.42x faster                                                           |
| float                      | 76.1 ms                                                         | 53.8 ms: 1.42x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 219 us: 1.41x faster                                                            |
| mako                       | 10.3 ms                                                         | 7.31 ms: 1.41x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.66 sec: 1.39x faster                                                          |
| raytrace                   | 327 ms                                                          | 238 ms: 1.38x faster                                                            |
| regex_compile              | 148 ms                                                          | 108 ms: 1.37x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.11 ms: 1.36x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 110 ms: 1.36x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.98 ms: 1.35x faster                                                           |
| deepcopy                   | 381 us                                                          | 285 us: 1.34x faster                                                            |
| nbody                      | 126 ms                                                          | 94.2 ms: 1.34x faster                                                           |
| async_tree_none            | 343 ms                                                          | 259 ms: 1.32x faster                                                            |
| fannkuch                   | 399 ms                                                          | 303 ms: 1.32x faster                                                            |
| sympy_str                  | 283 ms                                                          | 216 ms: 1.31x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 60.7 ms: 1.31x faster                                                           |
| logging_simple             | 10.8 us                                                         | 8.30 us: 1.30x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.55 us: 1.30x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 42.6 ms: 1.29x faster                                                           |
| pyflate                    | 471 ms                                                          | 369 ms: 1.28x faster                                                            |
| logging_format             | 11.5 us                                                         | 9.00 us: 1.27x faster                                                           |
| nqueens                    | 111 ms                                                          | 87.7 ms: 1.27x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 15.7 ms: 1.27x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 327 ms: 1.25x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 632 ms: 1.24x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 242 ms: 1.24x faster                                                            |
| scimark_fft                | 291 ms                                                          | 235 ms: 1.24x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 305 ms: 1.24x faster                                                            |
| go                         | 147 ms                                                          | 119 ms: 1.23x faster                                                            |
| sympy_expand               | 462 ms                                                          | 376 ms: 1.23x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 608 ms: 1.23x faster                                                            |
| async_tree_io              | 754 ms                                                          | 620 ms: 1.22x faster                                                            |
| tornado_http               | 118 ms                                                          | 98.6 ms: 1.20x faster                                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 43.2 ms: 1.20x faster                                                           |
| pycparser                  | 1.04 sec                                                        | 876 ms: 1.19x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 60.8 ms: 1.18x faster                                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.44 sec: 1.17x faster                                                          |
| pprint_safe_repr           | 819 ms                                                          | 702 ms: 1.17x faster                                                            |
| hexiom                     | 7.51 ms                                                         | 6.47 ms: 1.16x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                          |
| json                       | 4.78 ms                                                         | 4.14 ms: 1.16x faster                                                           |
| dask                       | 355 ms                                                          | 307 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 512 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 501 ms: 1.15x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.87 us: 1.15x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 65.7 ms: 1.15x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.84 sec: 1.12x faster                                                          |
| 2to3                       | 282 ms                                                          | 252 ms: 1.12x faster                                                            |
| bench_thread_pool          | 1.14 ms                                                         | 1.03 ms: 1.11x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.96 us: 1.10x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 83.5 ms: 1.09x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 108 ms: 1.06x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 68.7 ms: 1.03x faster                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.7 sec: 1.02x faster                                                          |
| regex_dna                  | 122 ms                                                          | 120 ms: 1.02x faster                                                            |
| json_loads                 | 20.0 us                                                         | 19.8 us: 1.01x faster                                                           |
| pidigits                   | 203 ms                                                          | 201 ms: 1.01x faster                                                            |
| pickle_list                | 3.27 us                                                         | 3.28 us: 1.00x slower                                                           |
| pickle                     | 7.99 us                                                         | 8.09 us: 1.01x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.87 ms: 1.03x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 15.7 ms: 1.04x slower                                                           |
| python_startup             | 22.0 ms                                                         | 23.0 ms: 1.05x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 646 us: 1.05x slower                                                            |
| pathlib                    | 79.9 ms                                                         | 84.1 ms: 1.05x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 74.7 ms: 1.05x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.8 ms: 1.11x slower                                                           |
| async_generators           | 260 ms                                                          | 289 ms: 1.11x slower                                                            |
| unpickle                   | 9.23 us                                                         | 10.3 us: 1.11x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.98 ms: 1.13x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 218 ms: 1.93x slower                                                            |
| coverage                   | 58.0 ms                                                         | 466 ms: 8.03x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.21x faster                                                                    |

Benchmark hidden because not significant (2): gc_traversal, pickle_dict
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown