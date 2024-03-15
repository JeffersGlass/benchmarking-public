
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 233 ms: 1.21x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.65 ms: 1.43x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.73 sec: 1.22x faster                                                          |
| tornado_http   | 118 ms                                                          | 93.7 ms: 1.26x faster                                                           |
| Geometric mean | (ref)                                                           | 1.28x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 250 ms: 1.37x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 314 ms: 1.30x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 587 ms: 1.27x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 239 ms: 1.26x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 301 ms: 1.25x faster                                                            |
| async_tree_io              | 754 ms                                                          | 613 ms: 1.23x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 488 ms: 1.18x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 505 ms: 1.17x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 72.6 ms: 1.73x faster                                                           |
| float          | 76.1 ms                                                         | 52.4 ms: 1.45x faster                                                           |
| pidigits       | 203 ms                                                          | 197 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                           | 1.37x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 95.4 ms: 1.55x faster                                                           |
| regex_v8       | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                           |
| regex_effbot   | 1.82 ms                                                         | 1.98 ms: 1.09x slower                                                           |
| regex_dna      | 122 ms                                                          | 138 ms: 1.13x slower                                                            |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 139 us: 1.66x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 205 us: 1.50x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.65 ms: 1.47x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.62 sec: 1.42x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 40.8 ms: 1.35x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 58.5 ms: 1.23x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 66.6 ms: 1.13x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.98 us: 1.10x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 111 ms: 1.03x faster                                                            |
| pickle               | 7.99 us                                                         | 7.92 us: 1.01x faster                                                           |
| json_loads           | 20.0 us                                                         | 19.9 us: 1.01x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.24 us: 1.01x faster                                                           |
| unpickle             | 9.23 us                                                         | 10.0 us: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.18x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.1 ms: 1.05x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.4 ms: 1.09x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.01 ms: 1.47x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 93.8 us: 5.10x faster                                                           |
| generators                 | 52.2 ms                                                         | 23.1 ms: 2.26x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 31.1 ns: 2.10x faster                                                           |
| logging_silent             | 119 ns                                                          | 57.6 ns: 2.07x faster                                                           |
| comprehensions             | 22.1 us                                                         | 11.1 us: 1.98x faster                                                           |
| spectral_norm              | 122 ms                                                          | 64.3 ms: 1.89x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.23 ms: 1.84x faster                                                           |
| richards_super             | 58.7 ms                                                         | 32.4 ms: 1.81x faster                                                           |
| chaos                      | 84.4 ms                                                         | 46.7 ms: 1.81x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 22.4 us: 1.78x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 4.24 ms: 1.77x faster                                                           |
| nbody                      | 126 ms                                                          | 72.6 ms: 1.73x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 866 us: 1.72x faster                                                            |
| raytrace                   | 327 ms                                                          | 191 ms: 1.71x faster                                                            |
| scimark_lu                 | 102 ms                                                          | 59.8 ms: 1.71x faster                                                           |
| richards                   | 48.8 ms                                                         | 28.8 ms: 1.69x faster                                                           |
| scimark_sor                | 135 ms                                                          | 80.8 ms: 1.67x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 139 us: 1.66x faster                                                            |
| coroutines                 | 23.7 ms                                                         | 14.5 ms: 1.63x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.09 ms: 1.63x faster                                                           |
| nqueens                    | 111 ms                                                          | 71.4 ms: 1.56x faster                                                           |
| regex_compile              | 148 ms                                                          | 95.4 ms: 1.55x faster                                                           |
| go                         | 147 ms                                                          | 95.3 ms: 1.54x faster                                                           |
| pyflate                    | 471 ms                                                          | 307 ms: 1.54x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 46.2 ms: 1.53x faster                                                           |
| crypto_pyaes               | 79.4 ms                                                         | 52.3 ms: 1.52x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 205 us: 1.50x faster                                                            |
| json_dumps                 | 9.80 ms                                                         | 6.65 ms: 1.47x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 101 ms: 1.47x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 2.88 ms: 1.47x faster                                                           |
| mako                       | 10.3 ms                                                         | 7.01 ms: 1.47x faster                                                           |
| scimark_fft                | 291 ms                                                          | 199 ms: 1.46x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.16 sec: 1.46x faster                                                          |
| float                      | 76.1 ms                                                         | 52.4 ms: 1.45x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 570 ms: 1.44x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.65 ms: 1.43x faster                                                           |
| sympy_str                  | 283 ms                                                          | 198 ms: 1.43x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.62 sec: 1.42x faster                                                          |
| sympy_integrate            | 19.9 ms                                                         | 14.1 ms: 1.42x faster                                                           |
| deepcopy                   | 381 us                                                          | 270 us: 1.41x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.38 us: 1.39x faster                                                           |
| logging_simple             | 10.8 us                                                         | 7.85 us: 1.38x faster                                                           |
| async_tree_none            | 343 ms                                                          | 250 ms: 1.37x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.34 us: 1.37x faster                                                           |
| fannkuch                   | 399 ms                                                          | 292 ms: 1.37x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 40.8 ms: 1.35x faster                                                           |
| sympy_expand               | 462 ms                                                          | 344 ms: 1.34x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 38.9 ms: 1.33x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 314 ms: 1.30x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.61 sec: 1.29x faster                                                          |
| pycparser                  | 1.04 sec                                                        | 812 ms: 1.28x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 587 ms: 1.27x faster                                                            |
| tornado_http               | 118 ms                                                          | 93.7 ms: 1.26x faster                                                           |
| async_tree_none_tg         | 301 ms                                                          | 239 ms: 1.26x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 301 ms: 1.25x faster                                                            |
| async_tree_io              | 754 ms                                                          | 613 ms: 1.23x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 58.5 ms: 1.23x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.73 sec: 1.22x faster                                                          |
| 2to3                       | 282 ms                                                          | 233 ms: 1.21x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 75.9 ms: 1.20x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 663 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 488 ms: 1.18x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.83 us: 1.18x faster                                                           |
| dask                       | 355 ms                                                          | 302 ms: 1.18x faster                                                            |
| json                       | 4.78 ms                                                         | 4.09 ms: 1.17x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 505 ms: 1.17x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 66.6 ms: 1.13x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.98 us: 1.10x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.04 ms: 1.09x faster                                                           |
| pidigits                   | 203 ms                                                          | 197 ms: 1.03x faster                                                            |
| xml_etree_parse            | 114 ms                                                          | 111 ms: 1.03x faster                                                            |
| pickle                     | 7.99 us                                                         | 7.92 us: 1.01x faster                                                           |
| json_loads                 | 20.0 us                                                         | 19.9 us: 1.01x faster                                                           |
| pickle_list                | 3.27 us                                                         | 3.24 us: 1.01x faster                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 71.9 ms: 1.01x slower                                                           |
| async_generators           | 260 ms                                                          | 265 ms: 1.02x slower                                                            |
| gc_traversal               | 1.38 ms                                                         | 1.41 ms: 1.02x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| python_startup             | 22.0 ms                                                         | 23.1 ms: 1.05x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.2 ms: 1.07x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 664 us: 1.07x slower                                                            |
| python_startup_no_site     | 18.8 ms                                                         | 20.4 ms: 1.09x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.98 ms: 1.09x slower                                                           |
| unpickle                   | 9.23 us                                                         | 10.0 us: 1.09x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 89.5 ms: 1.12x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.99 ms: 1.13x slower                                                           |
| regex_dna                  | 122 ms                                                          | 138 ms: 1.13x slower                                                            |
| sqlglot_normalize          | 113 ms                                                          | 202 ms: 1.78x slower                                                            |
| coverage                   | 58.0 ms                                                         | 473 ms: 8.16x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.30x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: unknown