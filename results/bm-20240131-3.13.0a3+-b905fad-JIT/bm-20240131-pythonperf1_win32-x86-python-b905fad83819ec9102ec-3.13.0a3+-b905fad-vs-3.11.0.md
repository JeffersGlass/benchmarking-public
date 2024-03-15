
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.17x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 263 ms: 1.07x faster                                                            |
| chameleon      | 8.08 ms                                                         | 6.44 ms: 1.26x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.87 sec: 1.12x faster                                                          |
| tornado_http   | 118 ms                                                          | 101 ms: 1.17x faster                                                            |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 265 ms: 1.29x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 333 ms: 1.23x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 253 ms: 1.19x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 630 ms: 1.18x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 319 ms: 1.18x faster                                                            |
| async_tree_io              | 754 ms                                                          | 640 ms: 1.18x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 516 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 529 ms: 1.12x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.18x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 56.2 ms: 1.35x faster                                                           |
| nbody          | 126 ms                                                          | 93.7 ms: 1.34x faster                                                           |
| pidigits       | 203 ms                                                          | 202 ms: 1.00x faster                                                            |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 114 ms: 1.30x faster                                                            |
| regex_dna      | 122 ms                                                          | 124 ms: 1.02x slower                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.92 ms: 1.05x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 159 us: 1.45x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 7.06 ms: 1.39x faster                                                           |
| pickle_pure_python   | 309 us                                                          | 224 us: 1.38x faster                                                            |
| tomli_loads          | 2.31 sec                                                        | 1.69 sec: 1.37x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 42.8 ms: 1.29x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 61.7 ms: 1.16x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 69.4 ms: 1.09x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 3.12 us: 1.05x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 110 ms: 1.04x faster                                                            |
| json_loads           | 20.0 us                                                         | 20.3 us: 1.01x slower                                                           |
| pickle               | 7.99 us                                                         | 8.16 us: 1.02x slower                                                           |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.14x faster                                                                    |

Benchmark hidden because not significant (2): pickle_list, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.3 ms: 1.06x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 21.0 ms: 1.11x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.09x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.84 ms: 1.31x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 99.3 us: 4.82x faster                                                           |
| generators                 | 52.2 ms                                                         | 24.2 ms: 2.16x faster                                                           |
| logging_silent             | 119 ns                                                          | 67.1 ns: 1.78x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.58 ms: 1.59x faster                                                           |
| spectral_norm              | 122 ms                                                          | 77.0 ms: 1.58x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 15.1 ms: 1.57x faster                                                           |
| richards_super             | 58.7 ms                                                         | 37.5 ms: 1.56x faster                                                           |
| scimark_sor                | 135 ms                                                          | 88.3 ms: 1.53x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 26.3 us: 1.52x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 980 us: 1.52x faster                                                            |
| richards                   | 48.8 ms                                                         | 32.1 ms: 1.52x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 67.6 ms: 1.51x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 159 us: 1.45x faster                                                            |
| comprehensions             | 22.1 us                                                         | 15.2 us: 1.45x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.25 ms: 1.43x faster                                                           |
| chaos                      | 84.4 ms                                                         | 59.4 ms: 1.42x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 7.06 ms: 1.39x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 47.1 ns: 1.38x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 224 us: 1.38x faster                                                            |
| raytrace                   | 327 ms                                                          | 237 ms: 1.38x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.69 sec: 1.37x faster                                                          |
| float                      | 76.1 ms                                                         | 56.2 ms: 1.35x faster                                                           |
| nbody                      | 126 ms                                                          | 93.7 ms: 1.34x faster                                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.17 ms: 1.33x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.52 us: 1.31x faster                                                           |
| mako                       | 10.3 ms                                                         | 7.84 ms: 1.31x faster                                                           |
| deepcopy                   | 381 us                                                          | 292 us: 1.31x faster                                                            |
| sympy_sum                  | 149 ms                                                          | 114 ms: 1.31x faster                                                            |
| logging_simple             | 10.8 us                                                         | 8.29 us: 1.30x faster                                                           |
| regex_compile              | 148 ms                                                          | 114 ms: 1.30x faster                                                            |
| async_tree_none            | 343 ms                                                          | 265 ms: 1.29x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 42.8 ms: 1.29x faster                                                           |
| crypto_pyaes               | 79.4 ms                                                         | 61.9 ms: 1.28x faster                                                           |
| sympy_str                  | 283 ms                                                          | 221 ms: 1.28x faster                                                            |
| logging_format             | 11.5 us                                                         | 9.01 us: 1.27x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 6.44 ms: 1.26x faster                                                           |
| nqueens                    | 111 ms                                                          | 89.0 ms: 1.25x faster                                                           |
| fannkuch                   | 399 ms                                                          | 325 ms: 1.23x faster                                                            |
| pyflate                    | 471 ms                                                          | 384 ms: 1.23x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 333 ms: 1.23x faster                                                            |
| sympy_expand               | 462 ms                                                          | 380 ms: 1.22x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 869 ms: 1.20x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 16.7 ms: 1.19x faster                                                           |
| async_tree_none_tg         | 301 ms                                                          | 253 ms: 1.19x faster                                                            |
| go                         | 147 ms                                                          | 124 ms: 1.19x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 630 ms: 1.18x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 319 ms: 1.18x faster                                                            |
| async_tree_io              | 754 ms                                                          | 640 ms: 1.18x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.84 us: 1.17x faster                                                           |
| tornado_http               | 118 ms                                                          | 101 ms: 1.17x faster                                                            |
| scimark_fft                | 291 ms                                                          | 250 ms: 1.16x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 61.7 ms: 1.16x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 678 ms: 1.16x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 45.4 ms: 1.14x faster                                                           |
| json                       | 4.78 ms                                                         | 4.22 ms: 1.13x faster                                                           |
| dask                       | 355 ms                                                          | 315 ms: 1.13x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.87 sec: 1.12x faster                                                          |
| hexiom                     | 7.51 ms                                                         | 6.71 ms: 1.12x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 516 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 529 ms: 1.12x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.52 sec: 1.12x faster                                                          |
| mdp                        | 2.07 sec                                                        | 1.87 sec: 1.11x faster                                                          |
| pprint_safe_repr           | 819 ms                                                          | 743 ms: 1.10x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 69.4 ms: 1.09x faster                                                           |
| 2to3                       | 282 ms                                                          | 263 ms: 1.07x faster                                                            |
| bench_thread_pool          | 1.14 ms                                                         | 1.06 ms: 1.07x faster                                                           |
| meteor_contest             | 90.9 ms                                                         | 85.6 ms: 1.06x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 3.12 us: 1.05x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 110 ms: 1.04x faster                                                            |
| pidigits                   | 203 ms                                                          | 202 ms: 1.00x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 71.6 ms: 1.01x slower                                                           |
| json_loads                 | 20.0 us                                                         | 20.3 us: 1.01x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.41 ms: 1.02x slower                                                           |
| pickle                     | 7.99 us                                                         | 8.16 us: 1.02x slower                                                           |
| regex_dna                  | 122 ms                                                          | 124 ms: 1.02x slower                                                            |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| regex_effbot               | 1.82 ms                                                         | 1.92 ms: 1.05x slower                                                           |
| python_startup             | 22.0 ms                                                         | 23.3 ms: 1.06x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 75.1 ms: 1.06x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 667 us: 1.08x slower                                                            |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.10x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 21.0 ms: 1.11x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 89.6 ms: 1.12x slower                                                           |
| async_generators           | 260 ms                                                          | 299 ms: 1.15x slower                                                            |
| telco                      | 5.29 ms                                                         | 6.51 ms: 1.23x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 232 ms: 2.05x slower                                                            |
| coverage                   | 58.0 ms                                                         | 483 ms: 8.32x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.17x faster                                                                    |

Benchmark hidden because not significant (2): pickle_list, pickle_dict
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown