
# Results vs. 3.11.0

- fork: python
- ref: 5a1b5316af648ae79bb9
- machine: windows-x86
- commit hash: 5a1b531
- commit date: 2023-12-03
- overall geometric mean: 1.05x slower
- HPT reliability: 99.82%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 312 ms: 1.10x slower                                                            |
| chameleon      | 8.08 ms                                                         | 9.94 ms: 1.23x slower                                                           |
| docutils       | 2.10 sec                                                        | 2.15 sec: 1.02x slower                                                          |
| tornado_http   | 118 ms                                                          | 113 ms: 1.05x faster                                                            |
| Geometric mean | (ref)                                                           | 1.07x slower                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|---------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none           | 343 ms                                                          | 330 ms: 1.04x faster                                                            |
| async_tree_memoization    | 408 ms                                                          | 412 ms: 1.01x slower                                                            |
| async_tree_io_tg          | 746 ms                                                          | 769 ms: 1.03x slower                                                            |
| async_tree_io             | 754 ms                                                          | 782 ms: 1.04x slower                                                            |
| async_tree_memoization_tg | 378 ms                                                          | 395 ms: 1.05x slower                                                            |
| async_tree_none_tg        | 301 ms                                                          | 317 ms: 1.05x slower                                                            |
| Geometric mean            | (ref)                                                           | 1.02x slower                                                                    |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 98.2 ms: 1.28x faster                                                           |
| float          | 76.1 ms                                                         | 68.7 ms: 1.11x faster                                                           |
| pidigits       | 203 ms                                                          | 200 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.13x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 149 ms: 1.01x slower                                                            |
| regex_dna      | 122 ms                                                          | 123 ms: 1.01x slower                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.94 ms: 1.06x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 17.2 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_list        | 3.28 us                                                         | 2.71 us: 1.21x faster                                                           |
| json_dumps           | 9.80 ms                                                         | 8.30 ms: 1.18x faster                                                           |
| pickle               | 7.99 us                                                         | 7.54 us: 1.06x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 2.21 sec: 1.05x faster                                                          |
| pickle_list          | 3.27 us                                                         | 3.17 us: 1.03x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 111 ms: 1.03x faster                                                            |
| pickle_dict          | 20.1 us                                                         | 19.8 us: 1.02x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 78.3 ms: 1.04x slower                                                           |
| json_loads           | 20.0 us                                                         | 21.0 us: 1.05x slower                                                           |
| unpickle             | 9.23 us                                                         | 9.71 us: 1.05x slower                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 83.0 ms: 1.16x slower                                                           |
| xml_etree_process    | 55.0 ms                                                         | 64.6 ms: 1.17x slower                                                           |
| pickle_pure_python   | 309 us                                                          | 385 us: 1.25x slower                                                            |
| unpickle_pure_python | 231 us                                                          | 304 us: 1.31x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.03x slower                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.5 ms: 1.09x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 8.09 ms: 1.27x faster                                                           |

All benchmarks:
===============

| Benchmark                 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|---------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 478 us                                                          | 132 us: 3.63x faster                                                            |
| spectral_norm             | 122 ms                                                          | 89.8 ms: 1.35x faster                                                           |
| nbody                     | 126 ms                                                          | 98.2 ms: 1.28x faster                                                           |
| mako                      | 10.3 ms                                                         | 8.09 ms: 1.27x faster                                                           |
| comprehensions            | 22.1 us                                                         | 17.8 us: 1.24x faster                                                           |
| scimark_fft               | 291 ms                                                          | 236 ms: 1.23x faster                                                            |
| scimark_sparse_mat_mult   | 4.23 ms                                                         | 3.45 ms: 1.23x faster                                                           |
| unpickle_list             | 3.28 us                                                         | 2.71 us: 1.21x faster                                                           |
| crypto_pyaes              | 79.4 ms                                                         | 66.0 ms: 1.20x faster                                                           |
| json_dumps                | 9.80 ms                                                         | 8.30 ms: 1.18x faster                                                           |
| sympy_sum                 | 149 ms                                                          | 127 ms: 1.17x faster                                                            |
| asyncio_tcp               | 787 ms                                                          | 674 ms: 1.17x faster                                                            |
| sqlite_synth              | 2.15 us                                                         | 1.89 us: 1.14x faster                                                           |
| chaos                     | 84.4 ms                                                         | 74.5 ms: 1.13x faster                                                           |
| nqueens                   | 111 ms                                                          | 99.7 ms: 1.12x faster                                                           |
| float                     | 76.1 ms                                                         | 68.7 ms: 1.11x faster                                                           |
| json                      | 4.78 ms                                                         | 4.41 ms: 1.08x faster                                                           |
| sympy_str                 | 283 ms                                                          | 264 ms: 1.07x faster                                                            |
| pickle                    | 7.99 us                                                         | 7.54 us: 1.06x faster                                                           |
| tornado_http              | 118 ms                                                          | 113 ms: 1.05x faster                                                            |
| tomli_loads               | 2.31 sec                                                        | 2.21 sec: 1.05x faster                                                          |
| async_tree_none           | 343 ms                                                          | 330 ms: 1.04x faster                                                            |
| pickle_list               | 3.27 us                                                         | 3.17 us: 1.03x faster                                                           |
| xml_etree_parse           | 114 ms                                                          | 111 ms: 1.03x faster                                                            |
| sympy_integrate           | 19.9 ms                                                         | 19.4 ms: 1.03x faster                                                           |
| deltablue                 | 4.10 ms                                                         | 4.01 ms: 1.02x faster                                                           |
| pickle_dict               | 20.1 us                                                         | 19.8 us: 1.02x faster                                                           |
| pidigits                  | 203 ms                                                          | 200 ms: 1.01x faster                                                            |
| hexiom                    | 7.51 ms                                                         | 7.45 ms: 1.01x faster                                                           |
| dask                      | 355 ms                                                          | 353 ms: 1.01x faster                                                            |
| logging_format            | 11.5 us                                                         | 11.5 us: 1.00x slower                                                           |
| mdp                       | 2.07 sec                                                        | 2.08 sec: 1.00x slower                                                          |
| async_tree_memoization    | 408 ms                                                          | 412 ms: 1.01x slower                                                            |
| gc_traversal              | 1.38 ms                                                         | 1.39 ms: 1.01x slower                                                           |
| regex_compile             | 148 ms                                                          | 149 ms: 1.01x slower                                                            |
| regex_dna                 | 122 ms                                                          | 123 ms: 1.01x slower                                                            |
| asyncio_tcp_ssl           | 17.1 sec                                                        | 17.3 sec: 1.02x slower                                                          |
| bench_mp_pool             | 70.9 ms                                                         | 72.4 ms: 1.02x slower                                                           |
| docutils                  | 2.10 sec                                                        | 2.15 sec: 1.02x slower                                                          |
| async_tree_io_tg          | 746 ms                                                          | 769 ms: 1.03x slower                                                            |
| meteor_contest            | 90.9 ms                                                         | 93.7 ms: 1.03x slower                                                           |
| pyflate                   | 471 ms                                                          | 488 ms: 1.04x slower                                                            |
| xml_etree_iterparse       | 75.6 ms                                                         | 78.3 ms: 1.04x slower                                                           |
| bench_thread_pool         | 1.14 ms                                                         | 1.18 ms: 1.04x slower                                                           |
| async_tree_io             | 754 ms                                                          | 782 ms: 1.04x slower                                                            |
| create_gc_cycles          | 618 us                                                          | 642 us: 1.04x slower                                                            |
| python_startup            | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                                           |
| async_tree_memoization_tg | 378 ms                                                          | 395 ms: 1.05x slower                                                            |
| json_loads                | 20.0 us                                                         | 21.0 us: 1.05x slower                                                           |
| async_tree_none_tg        | 301 ms                                                          | 317 ms: 1.05x slower                                                            |
| unpickle                  | 9.23 us                                                         | 9.71 us: 1.05x slower                                                           |
| regex_effbot              | 1.82 ms                                                         | 1.94 ms: 1.06x slower                                                           |
| sqlglot_normalize         | 113 ms                                                          | 120 ms: 1.06x slower                                                            |
| sqlglot_parse             | 1.49 ms                                                         | 1.60 ms: 1.07x slower                                                           |
| sqlglot_transpile         | 1.78 ms                                                         | 1.93 ms: 1.08x slower                                                           |
| raytrace                  | 327 ms                                                          | 354 ms: 1.08x slower                                                            |
| python_startup_no_site    | 18.8 ms                                                         | 20.5 ms: 1.09x slower                                                           |
| generators                | 52.2 ms                                                         | 56.9 ms: 1.09x slower                                                           |
| sqlglot_optimize          | 51.8 ms                                                         | 56.6 ms: 1.09x slower                                                           |
| 2to3                      | 282 ms                                                          | 312 ms: 1.10x slower                                                            |
| pycparser                 | 1.04 sec                                                        | 1.15 sec: 1.11x slower                                                          |
| pathlib                   | 79.9 ms                                                         | 89.6 ms: 1.12x slower                                                           |
| pprint_pformat            | 1.70 sec                                                        | 1.90 sec: 1.12x slower                                                          |
| scimark_monte_carlo       | 70.8 ms                                                         | 79.6 ms: 1.12x slower                                                           |
| regex_v8                  | 15.2 ms                                                         | 17.2 ms: 1.14x slower                                                           |
| pprint_safe_repr          | 819 ms                                                          | 936 ms: 1.14x slower                                                            |
| richards_super            | 58.7 ms                                                         | 67.7 ms: 1.15x slower                                                           |
| xml_etree_generate        | 71.6 ms                                                         | 83.0 ms: 1.16x slower                                                           |
| deepcopy                  | 381 us                                                          | 443 us: 1.16x slower                                                            |
| deepcopy_reduce           | 3.32 us                                                         | 3.89 us: 1.17x slower                                                           |
| xml_etree_process         | 55.0 ms                                                         | 64.6 ms: 1.17x slower                                                           |
| chameleon                 | 8.08 ms                                                         | 9.94 ms: 1.23x slower                                                           |
| pickle_pure_python        | 309 us                                                          | 385 us: 1.25x slower                                                            |
| go                        | 147 ms                                                          | 185 ms: 1.26x slower                                                            |
| richards                  | 48.8 ms                                                         | 61.5 ms: 1.26x slower                                                           |
| deepcopy_memo             | 40.0 us                                                         | 50.7 us: 1.27x slower                                                           |
| scimark_lu                | 102 ms                                                          | 133 ms: 1.30x slower                                                            |
| logging_silent            | 119 ns                                                          | 156 ns: 1.31x slower                                                            |
| unpickle_pure_python      | 231 us                                                          | 304 us: 1.31x slower                                                            |
| telco                     | 5.29 ms                                                         | 7.09 ms: 1.34x slower                                                           |
| coroutines                | 23.7 ms                                                         | 31.9 ms: 1.34x slower                                                           |
| async_generators          | 260 ms                                                          | 357 ms: 1.38x slower                                                            |
| scimark_sor               | 135 ms                                                          | 186 ms: 1.38x slower                                                            |
| unpack_sequence           | 65.2 ns                                                         | 97.7 ns: 1.50x slower                                                           |
| coverage                  | 58.0 ms                                                         | 774 ms: 13.34x slower                                                           |
| Geometric mean            | (ref)                                                           | 1.05x slower                                                                    |

Benchmark hidden because not significant (5): fannkuch, logging_simple, sympy_expand, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.82% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown