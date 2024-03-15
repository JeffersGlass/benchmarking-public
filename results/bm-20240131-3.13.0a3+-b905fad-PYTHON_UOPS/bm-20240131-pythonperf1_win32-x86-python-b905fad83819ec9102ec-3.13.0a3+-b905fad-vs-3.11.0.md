
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.23x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 247 ms: 1.14x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.94 ms: 1.36x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.4 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 252 ms: 1.36x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 318 ms: 1.28x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 302 ms: 1.25x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 243 ms: 1.24x faster                                                            |
| async_tree_io              | 754 ms                                                          | 611 ms: 1.23x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 606 ms: 1.23x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 516 ms: 1.14x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 506 ms: 1.14x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 87.6 ms: 1.44x faster                                                           |
| float          | 76.1 ms                                                         | 61.4 ms: 1.24x faster                                                           |
| pidigits       | 203 ms                                                          | 199 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 107 ms: 1.38x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.3 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                    |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 152 us: 1.52x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 213 us: 1.45x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.94 ms: 1.41x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.67 sec: 1.39x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 42.0 ms: 1.31x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 59.6 ms: 1.20x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 69.7 ms: 1.08x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 3.13 us: 1.05x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 111 ms: 1.03x faster                                                            |
| pickle               | 7.99 us                                                         | 7.87 us: 1.01x faster                                                           |
| json_loads           | 20.0 us                                                         | 20.5 us: 1.02x slower                                                           |
| pickle_list          | 3.27 us                                                         | 3.35 us: 1.03x slower                                                           |
| unpickle             | 9.23 us                                                         | 9.92 us: 1.08x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.3 ms: 1.06x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.9 ms: 1.11x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.09x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 8.19 ms: 1.25x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 91.3 us: 5.24x faster                                                           |
| generators                 | 52.2 ms                                                         | 23.2 ms: 2.25x faster                                                           |
| logging_silent             | 119 ns                                                          | 60.2 ns: 1.98x faster                                                           |
| richards_super             | 58.7 ms                                                         | 33.6 ms: 1.75x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.3 ms: 1.66x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 24.4 us: 1.64x faster                                                           |
| scimark_sor                | 135 ms                                                          | 82.6 ms: 1.64x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 62.8 ms: 1.63x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 921 us: 1.62x faster                                                            |
| unpack_sequence            | 65.2 ns                                                         | 40.4 ns: 1.62x faster                                                           |
| richards                   | 48.8 ms                                                         | 30.4 ms: 1.60x faster                                                           |
| comprehensions             | 22.1 us                                                         | 13.8 us: 1.60x faster                                                           |
| chaos                      | 84.4 ms                                                         | 54.5 ms: 1.55x faster                                                           |
| raytrace                   | 327 ms                                                          | 211 ms: 1.55x faster                                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.16 ms: 1.54x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 152 us: 1.52x faster                                                            |
| pickle_pure_python         | 309 us                                                          | 213 us: 1.45x faster                                                            |
| nbody                      | 126 ms                                                          | 87.6 ms: 1.44x faster                                                           |
| nqueens                    | 111 ms                                                          | 78.2 ms: 1.42x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.88 ms: 1.42x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.94 ms: 1.41x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.36 us: 1.41x faster                                                           |
| go                         | 147 ms                                                          | 105 ms: 1.40x faster                                                            |
| spectral_norm              | 122 ms                                                          | 87.2 ms: 1.40x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 5.39 ms: 1.39x faster                                                           |
| deepcopy                   | 381 us                                                          | 274 us: 1.39x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.67 sec: 1.39x faster                                                          |
| pyflate                    | 471 ms                                                          | 340 ms: 1.38x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 57.5 ms: 1.38x faster                                                           |
| regex_compile              | 148 ms                                                          | 107 ms: 1.38x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 109 ms: 1.37x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.24 sec: 1.37x faster                                                          |
| chameleon                  | 8.08 ms                                                         | 5.94 ms: 1.36x faster                                                           |
| async_tree_none            | 343 ms                                                          | 252 ms: 1.36x faster                                                            |
| fannkuch                   | 399 ms                                                          | 295 ms: 1.36x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 52.3 ms: 1.35x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 607 ms: 1.35x faster                                                            |
| logging_simple             | 10.8 us                                                         | 8.06 us: 1.34x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 42.0 ms: 1.31x faster                                                           |
| sympy_str                  | 283 ms                                                          | 216 ms: 1.31x faster                                                            |
| scimark_fft                | 291 ms                                                          | 224 ms: 1.30x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.84 us: 1.30x faster                                                           |
| sympy_integrate            | 19.9 ms                                                         | 15.4 ms: 1.29x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 318 ms: 1.28x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 41.3 ms: 1.26x faster                                                           |
| mako                       | 10.3 ms                                                         | 8.19 ms: 1.25x faster                                                           |
| async_tree_memoization_tg  | 378 ms                                                          | 302 ms: 1.25x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.41 ms: 1.24x faster                                                           |
| async_tree_none_tg         | 301 ms                                                          | 243 ms: 1.24x faster                                                            |
| float                      | 76.1 ms                                                         | 61.4 ms: 1.24x faster                                                           |
| async_tree_io              | 754 ms                                                          | 611 ms: 1.23x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 606 ms: 1.23x faster                                                            |
| sympy_expand               | 462 ms                                                          | 378 ms: 1.22x faster                                                            |
| tornado_http               | 118 ms                                                          | 97.4 ms: 1.21x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.71 sec: 1.21x faster                                                          |
| xml_etree_generate         | 71.6 ms                                                         | 59.6 ms: 1.20x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 656 ms: 1.20x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 871 ms: 1.20x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                          |
| sqlite_synth               | 2.15 us                                                         | 1.87 us: 1.15x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 516 ms: 1.14x faster                                                            |
| 2to3                       | 282 ms                                                          | 247 ms: 1.14x faster                                                            |
| dask                       | 355 ms                                                          | 311 ms: 1.14x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 506 ms: 1.14x faster                                                            |
| json                       | 4.78 ms                                                         | 4.20 ms: 1.14x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 80.5 ms: 1.13x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 69.7 ms: 1.08x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.05 ms: 1.08x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 3.13 us: 1.05x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 111 ms: 1.03x faster                                                            |
| pidigits                   | 203 ms                                                          | 199 ms: 1.02x faster                                                            |
| pickle                     | 7.99 us                                                         | 7.87 us: 1.01x faster                                                           |
| async_generators           | 260 ms                                                          | 264 ms: 1.02x slower                                                            |
| json_loads                 | 20.0 us                                                         | 20.5 us: 1.02x slower                                                           |
| pickle_list                | 3.27 us                                                         | 3.35 us: 1.03x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.42 ms: 1.03x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 73.4 ms: 1.03x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| regex_effbot               | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| python_startup             | 22.0 ms                                                         | 23.3 ms: 1.06x slower                                                           |
| unpickle                   | 9.23 us                                                         | 9.92 us: 1.08x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 664 us: 1.08x slower                                                            |
| regex_v8                   | 15.2 ms                                                         | 16.3 ms: 1.08x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 88.7 ms: 1.11x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 20.9 ms: 1.11x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.18 ms: 1.17x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 213 ms: 1.89x slower                                                            |
| coverage                   | 58.0 ms                                                         | 481 ms: 8.29x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                    |

Benchmark hidden because not significant (2): pickle_dict, regex_dna
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: unknown