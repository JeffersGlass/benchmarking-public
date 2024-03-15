
# Results vs. 3.11.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 232 ms: 1.22x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.76 ms: 1.40x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.71 sec: 1.22x faster                                                          |
| tornado_http   | 118 ms                                                          | 93.8 ms: 1.26x faster                                                           |
| Geometric mean | (ref)                                                           | 1.27x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 244 ms: 1.41x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 303 ms: 1.35x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 571 ms: 1.31x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 290 ms: 1.30x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 232 ms: 1.30x faster                                                            |
| async_tree_io              | 754 ms                                                          | 587 ms: 1.28x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 499 ms: 1.18x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 493 ms: 1.17x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.29x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 78.1 ms: 1.61x faster                                                           |
| float          | 76.1 ms                                                         | 54.4 ms: 1.40x faster                                                           |
| pidigits       | 203 ms                                                          | 197 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.32x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 96.1 ms: 1.53x faster                                                           |
| regex_dna      | 122 ms                                                          | 119 ms: 1.02x faster                                                            |
| regex_v8       | 15.2 ms                                                         | 15.7 ms: 1.04x slower                                                           |
| regex_effbot   | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 141 us: 1.64x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 206 us: 1.50x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.69 ms: 1.46x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.59 sec: 1.45x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 40.9 ms: 1.35x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 59.3 ms: 1.21x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 64.6 ms: 1.17x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.88 us: 1.14x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pickle               | 7.99 us                                                         | 7.83 us: 1.02x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.9 us: 1.01x faster                                                           |
| json_loads           | 20.0 us                                                         | 19.8 us: 1.01x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.23 us: 1.01x faster                                                           |
| unpickle             | 9.23 us                                                         | 9.91 us: 1.07x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.19x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.7 ms: 1.03x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.4 ms: 1.09x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 6.86 ms: 1.50x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 88.6 us: 5.40x faster                                                           |
| generators                 | 52.2 ms                                                         | 22.5 ms: 2.32x faster                                                           |
| logging_silent             | 119 ns                                                          | 57.3 ns: 2.08x faster                                                           |
| comprehensions             | 22.1 us                                                         | 11.4 us: 1.94x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.15 ms: 1.91x faster                                                           |
| spectral_norm              | 122 ms                                                          | 64.4 ms: 1.89x faster                                                           |
| chaos                      | 84.4 ms                                                         | 46.3 ms: 1.82x faster                                                           |
| richards_super             | 58.7 ms                                                         | 32.9 ms: 1.78x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 4.25 ms: 1.77x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 853 us: 1.75x faster                                                            |
| unpack_sequence            | 65.2 ns                                                         | 37.5 ns: 1.74x faster                                                           |
| raytrace                   | 327 ms                                                          | 189 ms: 1.74x faster                                                            |
| scimark_lu                 | 102 ms                                                          | 59.2 ms: 1.73x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 23.6 us: 1.70x faster                                                           |
| richards                   | 48.8 ms                                                         | 28.9 ms: 1.69x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.4 ms: 1.65x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.08 ms: 1.65x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 141 us: 1.64x faster                                                            |
| nbody                      | 126 ms                                                          | 78.1 ms: 1.61x faster                                                           |
| scimark_sor                | 135 ms                                                          | 84.1 ms: 1.61x faster                                                           |
| nqueens                    | 111 ms                                                          | 69.5 ms: 1.60x faster                                                           |
| scimark_monte_carlo        | 70.8 ms                                                         | 45.1 ms: 1.57x faster                                                           |
| regex_compile              | 148 ms                                                          | 96.1 ms: 1.53x faster                                                           |
| pyflate                    | 471 ms                                                          | 309 ms: 1.52x faster                                                            |
| go                         | 147 ms                                                          | 96.7 ms: 1.52x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 206 us: 1.50x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 52.9 ms: 1.50x faster                                                           |
| mako                       | 10.3 ms                                                         | 6.86 ms: 1.50x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 100 ms: 1.49x faster                                                            |
| fannkuch                   | 399 ms                                                          | 269 ms: 1.49x faster                                                            |
| json_dumps                 | 9.80 ms                                                         | 6.69 ms: 1.46x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.59 sec: 1.45x faster                                                          |
| sympy_str                  | 283 ms                                                          | 197 ms: 1.44x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 2.98 ms: 1.42x faster                                                           |
| scimark_fft                | 291 ms                                                          | 206 ms: 1.42x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.20 sec: 1.41x faster                                                          |
| deepcopy                   | 381 us                                                          | 271 us: 1.41x faster                                                            |
| async_tree_none            | 343 ms                                                          | 244 ms: 1.41x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.76 ms: 1.40x faster                                                           |
| float                      | 76.1 ms                                                         | 54.4 ms: 1.40x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 14.3 ms: 1.39x faster                                                           |
| logging_simple             | 10.8 us                                                         | 7.79 us: 1.39x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 591 ms: 1.39x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.40 us: 1.38x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.36 us: 1.37x faster                                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 38.2 ms: 1.36x faster                                                           |
| sympy_expand               | 462 ms                                                          | 343 ms: 1.35x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 303 ms: 1.35x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 40.9 ms: 1.35x faster                                                           |
| pycparser                  | 1.04 sec                                                        | 794 ms: 1.31x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 571 ms: 1.31x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 290 ms: 1.30x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 232 ms: 1.30x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.60 sec: 1.29x faster                                                          |
| async_tree_io              | 754 ms                                                          | 587 ms: 1.28x faster                                                            |
| tornado_http               | 118 ms                                                          | 93.8 ms: 1.26x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.71 sec: 1.22x faster                                                          |
| 2to3                       | 282 ms                                                          | 232 ms: 1.22x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 648 ms: 1.21x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 59.3 ms: 1.21x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 75.8 ms: 1.20x faster                                                           |
| json                       | 4.78 ms                                                         | 4.03 ms: 1.19x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 499 ms: 1.18x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 493 ms: 1.17x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 64.6 ms: 1.17x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 991 us: 1.15x faster                                                            |
| unpickle_list              | 3.28 us                                                         | 2.88 us: 1.14x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 1.96 us: 1.10x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pidigits                   | 203 ms                                                          | 197 ms: 1.03x faster                                                            |
| regex_dna                  | 122 ms                                                          | 119 ms: 1.02x faster                                                            |
| pickle                     | 7.99 us                                                         | 7.83 us: 1.02x faster                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.02x faster                                                          |
| pickle_dict                | 20.1 us                                                         | 19.9 us: 1.01x faster                                                           |
| json_loads                 | 20.0 us                                                         | 19.8 us: 1.01x faster                                                           |
| pickle_list                | 3.27 us                                                         | 3.23 us: 1.01x faster                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 71.8 ms: 1.01x slower                                                           |
| python_startup             | 22.0 ms                                                         | 22.7 ms: 1.03x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 15.7 ms: 1.04x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 651 us: 1.05x slower                                                            |
| pathlib                    | 79.9 ms                                                         | 85.1 ms: 1.06x slower                                                           |
| async_generators           | 260 ms                                                          | 277 ms: 1.07x slower                                                            |
| unpickle                   | 9.23 us                                                         | 9.91 us: 1.07x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.4 ms: 1.09x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.84 ms: 1.10x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 196 ms: 1.73x slower                                                            |
| coverage                   | 58.0 ms                                                         | 474 ms: 8.17x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.31x faster                                                                    |

Benchmark hidden because not significant (1): gc_traversal
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: unknown