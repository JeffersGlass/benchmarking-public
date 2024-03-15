
# Results vs. 3.11.0

- fork: python
- ref: 68a7b78cd5185cbd9456
- machine: windows-x86
- commit hash: 68a7b78
- commit date: 2024-01-18
- overall geometric mean: 1.25x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 241 ms: 1.17x faster                                                            |
| chameleon      | 8.08 ms                                                         | 5.80 ms: 1.39x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.79 sec: 1.17x faster                                                          |
| tornado_http   | 118 ms                                                          | 101 ms: 1.17x faster                                                            |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 247 ms: 1.39x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 310 ms: 1.32x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 584 ms: 1.28x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 297 ms: 1.27x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 237 ms: 1.27x faster                                                            |
| async_tree_io              | 754 ms                                                          | 602 ms: 1.25x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 511 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 502 ms: 1.15x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.26x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 86.8 ms: 1.45x faster                                                           |
| float          | 76.1 ms                                                         | 59.3 ms: 1.28x faster                                                           |
| pidigits       | 203 ms                                                          | 199 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 104 ms: 1.42x faster                                                            |
| regex_dna      | 122 ms                                                          | 121 ms: 1.01x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.05x slower                                                           |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 156 us: 1.48x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 210 us: 1.47x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.72 ms: 1.46x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.65 sec: 1.40x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 41.2 ms: 1.34x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 59.9 ms: 1.20x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.0 ms: 1.11x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.99 us: 1.10x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 111 ms: 1.03x faster                                                            |
| json_loads           | 20.0 us                                                         | 19.8 us: 1.01x faster                                                           |
| pickle               | 7.99 us                                                         | 7.89 us: 1.01x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 20.0 us: 1.00x faster                                                           |
| pickle_list          | 3.27 us                                                         | 3.31 us: 1.01x slower                                                           |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.16x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.3 ms: 1.06x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 21.0 ms: 1.12x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.09x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.77 ms: 1.32x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 90.3 us: 5.30x faster                                                           |
| generators                 | 52.2 ms                                                         | 23.3 ms: 2.24x faster                                                           |
| logging_silent             | 119 ns                                                          | 60.1 ns: 1.98x faster                                                           |
| richards_super             | 58.7 ms                                                         | 32.5 ms: 1.80x faster                                                           |
| richards                   | 48.8 ms                                                         | 28.8 ms: 1.70x faster                                                           |
| scimark_sor                | 135 ms                                                          | 81.2 ms: 1.67x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 24.1 us: 1.66x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.3 ms: 1.66x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 900 us: 1.66x faster                                                            |
| scimark_lu                 | 102 ms                                                          | 62.7 ms: 1.63x faster                                                           |
| comprehensions             | 22.1 us                                                         | 13.6 us: 1.63x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 40.3 ns: 1.62x faster                                                           |
| raytrace                   | 327 ms                                                          | 207 ms: 1.58x faster                                                            |
| chaos                      | 84.4 ms                                                         | 53.6 ms: 1.57x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.14 ms: 1.57x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 156 us: 1.48x faster                                                            |
| pickle_pure_python         | 309 us                                                          | 210 us: 1.47x faster                                                            |
| deltablue                  | 4.10 ms                                                         | 2.81 ms: 1.46x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.72 ms: 1.46x faster                                                           |
| nbody                      | 126 ms                                                          | 86.8 ms: 1.45x faster                                                           |
| nqueens                    | 111 ms                                                          | 77.1 ms: 1.45x faster                                                           |
| deepcopy                   | 381 us                                                          | 266 us: 1.43x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 55.4 ms: 1.43x faster                                                           |
| regex_compile              | 148 ms                                                          | 104 ms: 1.42x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.19 sec: 1.42x faster                                                          |
| hexiom                     | 7.51 ms                                                         | 5.29 ms: 1.42x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.65 sec: 1.40x faster                                                          |
| go                         | 147 ms                                                          | 105 ms: 1.40x faster                                                            |
| pprint_safe_repr           | 819 ms                                                          | 585 ms: 1.40x faster                                                            |
| pyflate                    | 471 ms                                                          | 337 ms: 1.40x faster                                                            |
| chameleon                  | 8.08 ms                                                         | 5.80 ms: 1.39x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 107 ms: 1.39x faster                                                            |
| async_tree_none            | 343 ms                                                          | 247 ms: 1.39x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.41 us: 1.38x faster                                                           |
| logging_simple             | 10.8 us                                                         | 7.94 us: 1.36x faster                                                           |
| spectral_norm              | 122 ms                                                          | 89.4 ms: 1.36x faster                                                           |
| fannkuch                   | 399 ms                                                          | 294 ms: 1.36x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 52.5 ms: 1.35x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 41.2 ms: 1.34x faster                                                           |
| sympy_str                  | 283 ms                                                          | 212 ms: 1.33x faster                                                            |
| logging_format             | 11.5 us                                                         | 8.60 us: 1.33x faster                                                           |
| mako                       | 10.3 ms                                                         | 7.77 ms: 1.32x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 310 ms: 1.32x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 15.2 ms: 1.31x faster                                                           |
| pycparser                  | 1.04 sec                                                        | 812 ms: 1.28x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 40.4 ms: 1.28x faster                                                           |
| float                      | 76.1 ms                                                         | 59.3 ms: 1.28x faster                                                           |
| async_tree_io_tg           | 746 ms                                                          | 584 ms: 1.28x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 297 ms: 1.27x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 237 ms: 1.27x faster                                                            |
| sympy_expand               | 462 ms                                                          | 365 ms: 1.27x faster                                                            |
| scimark_fft                | 291 ms                                                          | 231 ms: 1.26x faster                                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.37 ms: 1.26x faster                                                           |
| async_tree_io              | 754 ms                                                          | 602 ms: 1.25x faster                                                            |
| asyncio_tcp                | 787 ms                                                          | 639 ms: 1.23x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 59.9 ms: 1.20x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.79 sec: 1.17x faster                                                          |
| json                       | 4.78 ms                                                         | 4.07 ms: 1.17x faster                                                           |
| tornado_http               | 118 ms                                                          | 101 ms: 1.17x faster                                                            |
| dask                       | 355 ms                                                          | 303 ms: 1.17x faster                                                            |
| 2to3                       | 282 ms                                                          | 241 ms: 1.17x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 511 ms: 1.15x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 78.8 ms: 1.15x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 502 ms: 1.15x faster                                                            |
| mdp                        | 2.07 sec                                                        | 1.80 sec: 1.15x faster                                                          |
| sqlite_synth               | 2.15 us                                                         | 1.91 us: 1.12x faster                                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.0 ms: 1.11x faster                                                           |
| unpickle_list              | 3.28 us                                                         | 2.99 us: 1.10x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.06 ms: 1.08x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 111 ms: 1.03x faster                                                            |
| pidigits                   | 203 ms                                                          | 199 ms: 1.02x faster                                                            |
| json_loads                 | 20.0 us                                                         | 19.8 us: 1.01x faster                                                           |
| pickle                     | 7.99 us                                                         | 7.89 us: 1.01x faster                                                           |
| regex_dna                  | 122 ms                                                          | 121 ms: 1.01x faster                                                            |
| pickle_dict                | 20.1 us                                                         | 20.0 us: 1.00x faster                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.39 ms: 1.01x slower                                                           |
| pickle_list                | 3.27 us                                                         | 3.31 us: 1.01x slower                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.3 sec: 1.02x slower                                                          |
| regex_effbot               | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                                           |
| async_generators           | 260 ms                                                          | 272 ms: 1.05x slower                                                            |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.05x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 651 us: 1.05x slower                                                            |
| python_startup             | 22.0 ms                                                         | 23.3 ms: 1.06x slower                                                           |
| telco                      | 5.29 ms                                                         | 5.65 ms: 1.07x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 75.8 ms: 1.07x slower                                                           |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.09x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 87.7 ms: 1.10x slower                                                           |
| python_startup_no_site     | 18.8 ms                                                         | 21.0 ms: 1.12x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 207 ms: 1.83x slower                                                            |
| coverage                   | 58.0 ms                                                         | 474 ms: 8.16x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.25x faster                                                                    |
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: unknown