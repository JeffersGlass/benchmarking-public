
# Results vs. 3.11.0

- fork: python
- ref: v3.11.8
- machine: windows-x86
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 277 ms: 1.02x faster                                            |
| docutils       | 2.10 sec                                                        | 2.00 sec: 1.05x faster                                          |
| tornado_http   | 118 ms                                                          | 114 ms: 1.04x faster                                            |
| Geometric mean | (ref)                                                           | 1.02x faster                                                    |

Benchmark hidden because not significant (2): chameleon, html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io_tg           | 746 ms                                                          | 699 ms: 1.07x faster                                            |
| async_tree_memoization     | 408 ms                                                          | 392 ms: 1.04x faster                                            |
| async_tree_none            | 343 ms                                                          | 329 ms: 1.04x faster                                            |
| async_tree_none_tg         | 301 ms                                                          | 291 ms: 1.03x faster                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 565 ms: 1.02x faster                                            |
| async_tree_io              | 754 ms                                                          | 740 ms: 1.02x faster                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 372 ms: 1.01x faster                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 600 ms: 1.02x slower                                            |
| Geometric mean             | (ref)                                                           | 1.03x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 117 ms: 1.08x faster                                            |
| float          | 76.1 ms                                                         | 71.6 ms: 1.06x faster                                           |
| pidigits       | 203 ms                                                          | 197 ms: 1.03x faster                                            |
| Geometric mean | (ref)                                                           | 1.06x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 140 ms: 1.05x faster                                            |
| regex_dna      | 122 ms                                                          | 117 ms: 1.04x faster                                            |
| regex_v8       | 15.2 ms                                                         | 15.3 ms: 1.01x slower                                           |
| regex_effbot   | 1.82 ms                                                         | 1.85 ms: 1.02x slower                                           |
| Geometric mean | (ref)                                                           | 1.02x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|---------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpickle_list       | 3.28 us                                                         | 2.57 us: 1.28x faster                                           |
| pickle              | 7.99 us                                                         | 7.53 us: 1.06x faster                                           |
| xml_etree_process   | 55.0 ms                                                         | 52.1 ms: 1.06x faster                                           |
| xml_etree_generate  | 71.6 ms                                                         | 68.5 ms: 1.05x faster                                           |
| tomli_loads         | 2.31 sec                                                        | 2.24 sec: 1.03x faster                                          |
| pickle_pure_python  | 309 us                                                          | 299 us: 1.03x faster                                            |
| xml_etree_iterparse | 75.6 ms                                                         | 73.4 ms: 1.03x faster                                           |
| unpickle            | 9.23 us                                                         | 9.04 us: 1.02x faster                                           |
| pickle_list         | 3.27 us                                                         | 3.20 us: 1.02x faster                                           |
| xml_etree_parse     | 114 ms                                                          | 114 ms: 1.01x faster                                            |
| pickle_dict         | 20.1 us                                                         | 20.0 us: 1.00x faster                                           |
| Geometric mean      | (ref)                                                           | 1.04x faster                                                    |

Benchmark hidden because not significant (3): unpickle_pure_python, json_dumps, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 18.8 ms                                                         | 17.9 ms: 1.05x faster                                           |
| python_startup         | 22.0 ms                                                         | 21.4 ms: 1.03x faster                                           |
| Geometric mean         | (ref)                                                           | 1.04x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 10.3 ms                                                         | 9.58 ms: 1.07x faster                                           |
| genshi_xml      | 61.2 ms                                                         | 59.5 ms: 1.03x faster                                           |
| django_template | 37.4 ms                                                         | 37.6 ms: 1.01x slower                                           |
| Geometric mean  | (ref)                                                           | 1.02x faster                                                    |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpickle_list              | 3.28 us                                                         | 2.57 us: 1.28x faster                                           |
| unpack_sequence            | 65.2 ns                                                         | 58.6 ns: 1.11x faster                                           |
| json                       | 4.78 ms                                                         | 4.29 ms: 1.11x faster                                           |
| pyflate                    | 471 ms                                                          | 426 ms: 1.11x faster                                            |
| async_generators           | 260 ms                                                          | 238 ms: 1.09x faster                                            |
| crypto_pyaes               | 79.4 ms                                                         | 73.4 ms: 1.08x faster                                           |
| nbody                      | 126 ms                                                          | 117 ms: 1.08x faster                                            |
| richards                   | 48.8 ms                                                         | 45.5 ms: 1.07x faster                                           |
| mako                       | 10.3 ms                                                         | 9.58 ms: 1.07x faster                                           |
| pathlib                    | 79.9 ms                                                         | 74.7 ms: 1.07x faster                                           |
| async_tree_io_tg           | 746 ms                                                          | 699 ms: 1.07x faster                                            |
| asyncio_tcp                | 787 ms                                                          | 738 ms: 1.07x faster                                            |
| scimark_sor                | 135 ms                                                          | 127 ms: 1.06x faster                                            |
| float                      | 76.1 ms                                                         | 71.6 ms: 1.06x faster                                           |
| pickle                     | 7.99 us                                                         | 7.53 us: 1.06x faster                                           |
| aiohttp                    | 1.17 ms                                                         | 1.10 ms: 1.06x faster                                           |
| generators                 | 52.2 ms                                                         | 49.4 ms: 1.06x faster                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 4.01 ms: 1.06x faster                                           |
| xml_etree_process          | 55.0 ms                                                         | 52.1 ms: 1.06x faster                                           |
| sqlglot_normalize          | 113 ms                                                          | 107 ms: 1.05x faster                                            |
| regex_compile              | 148 ms                                                          | 140 ms: 1.05x faster                                            |
| python_startup_no_site     | 18.8 ms                                                         | 17.9 ms: 1.05x faster                                           |
| docutils                   | 2.10 sec                                                        | 2.00 sec: 1.05x faster                                          |
| scimark_lu                 | 102 ms                                                          | 97.6 ms: 1.05x faster                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.71 ms: 1.05x faster                                           |
| telco                      | 5.29 ms                                                         | 5.06 ms: 1.05x faster                                           |
| xml_etree_generate         | 71.6 ms                                                         | 68.5 ms: 1.05x faster                                           |
| richards_super             | 58.7 ms                                                         | 56.2 ms: 1.04x faster                                           |
| deltablue                  | 4.10 ms                                                         | 3.93 ms: 1.04x faster                                           |
| logging_silent             | 119 ns                                                          | 114 ns: 1.04x faster                                            |
| sqlite_synth               | 2.15 us                                                         | 2.06 us: 1.04x faster                                           |
| regex_dna                  | 122 ms                                                          | 117 ms: 1.04x faster                                            |
| async_tree_memoization     | 408 ms                                                          | 392 ms: 1.04x faster                                            |
| async_tree_none            | 343 ms                                                          | 329 ms: 1.04x faster                                            |
| pprint_safe_repr           | 819 ms                                                          | 787 ms: 1.04x faster                                            |
| hexiom                     | 7.51 ms                                                         | 7.22 ms: 1.04x faster                                           |
| sqlglot_optimize           | 51.8 ms                                                         | 49.9 ms: 1.04x faster                                           |
| sqlalchemy_imperative      | 15.4 ms                                                         | 14.9 ms: 1.04x faster                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.63 sec: 1.04x faster                                          |
| sqlalchemy_declarative     | 115 ms                                                          | 111 ms: 1.04x faster                                            |
| comprehensions             | 22.1 us                                                         | 21.3 us: 1.04x faster                                           |
| sqlglot_parse              | 1.49 ms                                                         | 1.44 ms: 1.04x faster                                           |
| tornado_http               | 118 ms                                                          | 114 ms: 1.04x faster                                            |
| deepcopy_memo              | 40.0 us                                                         | 38.7 us: 1.04x faster                                           |
| coroutines                 | 23.7 ms                                                         | 22.9 ms: 1.03x faster                                           |
| dulwich_log                | 62.8 ms                                                         | 60.7 ms: 1.03x faster                                           |
| async_tree_none_tg         | 301 ms                                                          | 291 ms: 1.03x faster                                            |
| tomli_loads                | 2.31 sec                                                        | 2.24 sec: 1.03x faster                                          |
| pickle_pure_python         | 309 us                                                          | 299 us: 1.03x faster                                            |
| logging_simple             | 10.8 us                                                         | 10.5 us: 1.03x faster                                           |
| logging_format             | 11.5 us                                                         | 11.1 us: 1.03x faster                                           |
| sympy_str                  | 283 ms                                                          | 274 ms: 1.03x faster                                            |
| pidigits                   | 203 ms                                                          | 197 ms: 1.03x faster                                            |
| nqueens                    | 111 ms                                                          | 108 ms: 1.03x faster                                            |
| dask                       | 355 ms                                                          | 345 ms: 1.03x faster                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 73.4 ms: 1.03x faster                                           |
| genshi_xml                 | 61.2 ms                                                         | 59.5 ms: 1.03x faster                                           |
| raytrace                   | 327 ms                                                          | 318 ms: 1.03x faster                                            |
| python_startup             | 22.0 ms                                                         | 21.4 ms: 1.03x faster                                           |
| spectral_norm              | 122 ms                                                          | 118 ms: 1.03x faster                                            |
| pylint                     | 418 ms                                                          | 407 ms: 1.03x faster                                            |
| sympy_integrate            | 19.9 ms                                                         | 19.4 ms: 1.02x faster                                           |
| create_gc_cycles           | 618 us                                                          | 605 us: 1.02x faster                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 565 ms: 1.02x faster                                            |
| unpickle                   | 9.23 us                                                         | 9.04 us: 1.02x faster                                           |
| pickle_list                | 3.27 us                                                         | 3.20 us: 1.02x faster                                           |
| typing_runtime_protocols   | 478 us                                                          | 469 us: 1.02x faster                                            |
| async_tree_io              | 754 ms                                                          | 740 ms: 1.02x faster                                            |
| sympy_sum                  | 149 ms                                                          | 146 ms: 1.02x faster                                            |
| thrift                     | 801 us                                                          | 786 us: 1.02x faster                                            |
| 2to3                       | 282 ms                                                          | 277 ms: 1.02x faster                                            |
| gc_traversal               | 1.38 ms                                                         | 1.35 ms: 1.02x faster                                           |
| deepcopy                   | 381 us                                                          | 375 us: 1.02x faster                                            |
| mypy2                      | 626 ms                                                          | 616 ms: 1.02x faster                                            |
| sympy_expand               | 462 ms                                                          | 455 ms: 1.02x faster                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 372 ms: 1.01x faster                                            |
| deepcopy_reduce            | 3.32 us                                                         | 3.27 us: 1.01x faster                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.01x faster                                          |
| scimark_fft                | 291 ms                                                          | 288 ms: 1.01x faster                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 70.1 ms: 1.01x faster                                           |
| pycparser                  | 1.04 sec                                                        | 1.03 sec: 1.01x faster                                          |
| xml_etree_parse            | 114 ms                                                          | 114 ms: 1.01x faster                                            |
| pickle_dict                | 20.1 us                                                         | 20.0 us: 1.00x faster                                           |
| chaos                      | 84.4 ms                                                         | 84.1 ms: 1.00x faster                                           |
| flaskblogging              | 2.03 sec                                                        | 2.03 sec: 1.00x slower                                          |
| django_template            | 37.4 ms                                                         | 37.6 ms: 1.01x slower                                           |
| regex_v8                   | 15.2 ms                                                         | 15.3 ms: 1.01x slower                                           |
| meteor_contest             | 90.9 ms                                                         | 92.1 ms: 1.01x slower                                           |
| coverage                   | 58.0 ms                                                         | 59.0 ms: 1.02x slower                                           |
| regex_effbot               | 1.82 ms                                                         | 1.85 ms: 1.02x slower                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 600 ms: 1.02x slower                                            |
| go                         | 147 ms                                                          | 150 ms: 1.02x slower                                            |
| bench_mp_pool              | 70.9 ms                                                         | 72.8 ms: 1.03x slower                                           |
| fannkuch                   | 399 ms                                                          | 413 ms: 1.03x slower                                            |
| mdp                        | 2.07 sec                                                        | 2.18 sec: 1.05x slower                                          |
| Geometric mean             | (ref)                                                           | 1.03x faster                                                    |

Benchmark hidden because not significant (7): bench_thread_pool, unpickle_pure_python, html5lib, json_dumps, genshi_text, json_loads, chameleon


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown