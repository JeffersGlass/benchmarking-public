
# Results vs. 3.11.0

- fork: mdboom
- ref: aa_test
- machine: windows-x86
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 252 ms: 1.12x faster                                               |
| chameleon      | 8.08 ms                                                         | 5.83 ms: 1.38x faster                                              |
| docutils       | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                             |
| tornado_http   | 118 ms                                                          | 98.6 ms: 1.20x faster                                              |
| Geometric mean | (ref)                                                           | 1.21x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 255 ms: 1.34x faster                                               |
| async_tree_memoization     | 408 ms                                                          | 317 ms: 1.29x faster                                               |
| async_tree_memoization_tg  | 378 ms                                                          | 301 ms: 1.25x faster                                               |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                               |
| async_tree_io_tg           | 746 ms                                                          | 597 ms: 1.25x faster                                               |
| async_tree_io              | 754 ms                                                          | 615 ms: 1.23x faster                                               |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 503 ms: 1.15x faster                                               |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 517 ms: 1.14x faster                                               |
| Geometric mean             | (ref)                                                           | 1.24x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 88.6 ms: 1.42x faster                                              |
| float          | 76.1 ms                                                         | 54.0 ms: 1.41x faster                                              |
| pidigits       | 203 ms                                                          | 199 ms: 1.02x faster                                               |
| Geometric mean | (ref)                                                           | 1.27x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 108 ms: 1.36x faster                                               |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.03x slower                                              |
| regex_v8       | 15.2 ms                                                         | 15.8 ms: 1.04x slower                                              |
| Geometric mean | (ref)                                                           | 1.06x faster                                                       |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 158 us: 1.47x faster                                               |
| json_dumps           | 9.80 ms                                                         | 6.96 ms: 1.41x faster                                              |
| pickle_pure_python   | 309 us                                                          | 222 us: 1.39x faster                                               |
| tomli_loads          | 2.31 sec                                                        | 1.67 sec: 1.39x faster                                             |
| xml_etree_process    | 55.0 ms                                                         | 42.6 ms: 1.29x faster                                              |
| xml_etree_generate   | 71.6 ms                                                         | 61.1 ms: 1.17x faster                                              |
| xml_etree_iterparse  | 75.6 ms                                                         | 66.6 ms: 1.14x faster                                              |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                               |
| unpickle_list        | 3.28 us                                                         | 3.13 us: 1.05x faster                                              |
| pickle_list          | 3.27 us                                                         | 3.18 us: 1.03x faster                                              |
| pickle_dict          | 20.1 us                                                         | 20.0 us: 1.01x faster                                              |
| pickle               | 7.99 us                                                         | 8.07 us: 1.01x slower                                              |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.10x slower                                              |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                       |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                              |
| python_startup_no_site | 18.8 ms                                                         | 20.8 ms: 1.11x slower                                              |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.44 ms: 1.38x faster                                              |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 98.6 us: 4.85x faster                                              |
| generators                 | 52.2 ms                                                         | 24.5 ms: 2.13x faster                                              |
| logging_silent             | 119 ns                                                          | 67.8 ns: 1.76x faster                                              |
| richards_super             | 58.7 ms                                                         | 35.5 ms: 1.65x faster                                              |
| spectral_norm              | 122 ms                                                          | 74.1 ms: 1.64x faster                                              |
| deltablue                  | 4.10 ms                                                         | 2.55 ms: 1.61x faster                                              |
| coroutines                 | 23.7 ms                                                         | 14.8 ms: 1.60x faster                                              |
| richards                   | 48.8 ms                                                         | 30.9 ms: 1.58x faster                                              |
| comprehensions             | 22.1 us                                                         | 14.1 us: 1.57x faster                                              |
| deepcopy_memo              | 40.0 us                                                         | 25.7 us: 1.56x faster                                              |
| sqlglot_parse              | 1.49 ms                                                         | 961 us: 1.55x faster                                               |
| scimark_sor                | 135 ms                                                          | 88.3 ms: 1.53x faster                                              |
| scimark_lu                 | 102 ms                                                          | 68.2 ms: 1.50x faster                                              |
| sqlglot_transpile          | 1.78 ms                                                         | 1.21 ms: 1.47x faster                                              |
| unpickle_pure_python       | 231 us                                                          | 158 us: 1.47x faster                                               |
| nbody                      | 126 ms                                                          | 88.6 ms: 1.42x faster                                              |
| float                      | 76.1 ms                                                         | 54.0 ms: 1.41x faster                                              |
| json_dumps                 | 9.80 ms                                                         | 6.96 ms: 1.41x faster                                              |
| unpack_sequence            | 65.2 ns                                                         | 46.5 ns: 1.40x faster                                              |
| chaos                      | 84.4 ms                                                         | 60.2 ms: 1.40x faster                                              |
| pickle_pure_python         | 309 us                                                          | 222 us: 1.39x faster                                               |
| tomli_loads                | 2.31 sec                                                        | 1.67 sec: 1.39x faster                                             |
| chameleon                  | 8.08 ms                                                         | 5.83 ms: 1.38x faster                                              |
| mako                       | 10.3 ms                                                         | 7.44 ms: 1.38x faster                                              |
| raytrace                   | 327 ms                                                          | 238 ms: 1.38x faster                                               |
| deepcopy_reduce            | 3.32 us                                                         | 2.43 us: 1.37x faster                                              |
| regex_compile              | 148 ms                                                          | 108 ms: 1.36x faster                                               |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.11 ms: 1.36x faster                                              |
| sympy_sum                  | 149 ms                                                          | 110 ms: 1.35x faster                                               |
| async_tree_none            | 343 ms                                                          | 255 ms: 1.34x faster                                               |
| deepcopy                   | 381 us                                                          | 286 us: 1.33x faster                                               |
| sympy_str                  | 283 ms                                                          | 216 ms: 1.31x faster                                               |
| crypto_pyaes               | 79.4 ms                                                         | 61.4 ms: 1.29x faster                                              |
| xml_etree_process          | 55.0 ms                                                         | 42.6 ms: 1.29x faster                                              |
| async_tree_memoization     | 408 ms                                                          | 317 ms: 1.29x faster                                               |
| logging_simple             | 10.8 us                                                         | 8.42 us: 1.28x faster                                              |
| asyncio_tcp                | 787 ms                                                          | 615 ms: 1.28x faster                                               |
| nqueens                    | 111 ms                                                          | 87.8 ms: 1.27x faster                                              |
| fannkuch                   | 399 ms                                                          | 315 ms: 1.27x faster                                               |
| sympy_integrate            | 19.9 ms                                                         | 15.7 ms: 1.27x faster                                              |
| logging_format             | 11.5 us                                                         | 9.07 us: 1.26x faster                                              |
| async_tree_memoization_tg  | 378 ms                                                          | 301 ms: 1.25x faster                                               |
| async_tree_none_tg         | 301 ms                                                          | 241 ms: 1.25x faster                                               |
| async_tree_io_tg           | 746 ms                                                          | 597 ms: 1.25x faster                                               |
| pyflate                    | 471 ms                                                          | 379 ms: 1.24x faster                                               |
| go                         | 147 ms                                                          | 120 ms: 1.23x faster                                               |
| async_tree_io              | 754 ms                                                          | 615 ms: 1.23x faster                                               |
| sympy_expand               | 462 ms                                                          | 379 ms: 1.22x faster                                               |
| scimark_fft                | 291 ms                                                          | 241 ms: 1.21x faster                                               |
| tornado_http               | 118 ms                                                          | 98.6 ms: 1.20x faster                                              |
| pycparser                  | 1.04 sec                                                        | 872 ms: 1.20x faster                                               |
| sqlglot_optimize           | 51.8 ms                                                         | 43.5 ms: 1.19x faster                                              |
| pprint_pformat             | 1.70 sec                                                        | 1.43 sec: 1.18x faster                                             |
| xml_etree_generate         | 71.6 ms                                                         | 61.1 ms: 1.17x faster                                              |
| pprint_safe_repr           | 819 ms                                                          | 700 ms: 1.17x faster                                               |
| dask                       | 355 ms                                                          | 305 ms: 1.16x faster                                               |
| docutils                   | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                             |
| hexiom                     | 7.51 ms                                                         | 6.54 ms: 1.15x faster                                              |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 503 ms: 1.15x faster                                               |
| sqlite_synth               | 2.15 us                                                         | 1.87 us: 1.15x faster                                              |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 517 ms: 1.14x faster                                               |
| json                       | 4.78 ms                                                         | 4.19 ms: 1.14x faster                                              |
| xml_etree_iterparse        | 75.6 ms                                                         | 66.6 ms: 1.14x faster                                              |
| bench_thread_pool          | 1.14 ms                                                         | 1.01 ms: 1.12x faster                                              |
| mdp                        | 2.07 sec                                                        | 1.84 sec: 1.12x faster                                             |
| 2to3                       | 282 ms                                                          | 252 ms: 1.12x faster                                               |
| meteor_contest             | 90.9 ms                                                         | 84.6 ms: 1.07x faster                                              |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                               |
| unpickle_list              | 3.28 us                                                         | 3.13 us: 1.05x faster                                              |
| pickle_list                | 3.27 us                                                         | 3.18 us: 1.03x faster                                              |
| scimark_monte_carlo        | 70.8 ms                                                         | 69.3 ms: 1.02x faster                                              |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.7 sec: 1.02x faster                                             |
| pidigits                   | 203 ms                                                          | 199 ms: 1.02x faster                                               |
| pickle_dict                | 20.1 us                                                         | 20.0 us: 1.01x faster                                              |
| pickle                     | 7.99 us                                                         | 8.07 us: 1.01x slower                                              |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.03x slower                                              |
| python_startup             | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                              |
| regex_v8                   | 15.2 ms                                                         | 15.8 ms: 1.04x slower                                              |
| pathlib                    | 79.9 ms                                                         | 83.6 ms: 1.05x slower                                              |
| bench_mp_pool              | 70.9 ms                                                         | 74.7 ms: 1.05x slower                                              |
| create_gc_cycles           | 618 us                                                          | 652 us: 1.06x slower                                               |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.10x slower                                              |
| python_startup_no_site     | 18.8 ms                                                         | 20.8 ms: 1.11x slower                                              |
| async_generators           | 260 ms                                                          | 291 ms: 1.12x slower                                               |
| telco                      | 5.29 ms                                                         | 6.35 ms: 1.20x slower                                              |
| sqlglot_normalize          | 113 ms                                                          | 221 ms: 1.96x slower                                               |
| coverage                   | 58.0 ms                                                         | 474 ms: 8.17x slower                                               |
| Geometric mean             | (ref)                                                           | 1.20x faster                                                       |

Benchmark hidden because not significant (3): json_loads, regex_dna, gc_traversal
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown