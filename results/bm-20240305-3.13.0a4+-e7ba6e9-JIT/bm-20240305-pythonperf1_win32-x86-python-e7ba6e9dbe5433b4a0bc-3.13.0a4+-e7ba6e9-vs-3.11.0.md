# Results vs. 3.11.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: windows-x86
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.12x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 266 ms: 1.06x faster                                                            |
| chameleon      | 8.08 ms                                                         | 6.00 ms: 1.35x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.87 sec: 1.12x faster                                                          |
| html5lib       | 54.3 ms                                                         | 47.6 ms: 1.14x faster                                                           |
| tornado_http   | 118 ms                                                          | 99.9 ms: 1.18x faster                                                           |
| Geometric mean | (ref)                                                           | 1.17x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 271 ms: 1.27x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 339 ms: 1.21x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 634 ms: 1.18x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 258 ms: 1.17x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 325 ms: 1.16x faster                                                            |
| async_tree_io              | 754 ms                                                          | 649 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 515 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 529 ms: 1.12x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.17x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 56.4 ms: 1.35x faster                                                           |
| nbody          | 126 ms                                                          | 96.7 ms: 1.30x faster                                                           |
| pidigits       | 203 ms                                                          | 198 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 113 ms: 1.30x faster                                                            |
| regex_v8       | 15.2 ms                                                         | 16.1 ms: 1.06x slower                                                           |
| regex_dna      | 122 ms                                                          | 130 ms: 1.06x slower                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.96 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.02x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.80 ms                                                         | 7.10 ms: 1.38x faster                                                           |
| unpickle_pure_python | 231 us                                                          | 170 us: 1.36x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 228 us: 1.35x faster                                                            |
| tomli_loads          | 2.31 sec                                                        | 1.77 sec: 1.31x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 42.8 ms: 1.28x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 61.7 ms: 1.16x faster                                                           |
| unpickle_list        | 3.28 us                                                         | 2.93 us: 1.12x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 68.3 ms: 1.11x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pickle_list          | 3.27 us                                                         | 3.28 us: 1.01x slower                                                           |
| json_loads           | 20.0 us                                                         | 20.3 us: 1.01x slower                                                           |
| pickle               | 7.99 us                                                         | 8.16 us: 1.02x slower                                                           |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 26.0 ms: 1.18x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 24.0 ms: 1.28x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.23x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako            | 10.3 ms                                                         | 7.19 ms: 1.43x faster                                                           |
| genshi_xml      | 61.2 ms                                                         | 51.0 ms: 1.20x faster                                                           |
| django_template | 37.4 ms                                                         | 31.9 ms: 1.17x faster                                                           |
| genshi_text     | 26.8 ms                                                         | 23.9 ms: 1.12x faster                                                           |
| Geometric mean  | (ref)                                                           | 1.23x faster                                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 101 us: 4.76x faster                                                            |
| generators                 | 52.2 ms                                                         | 25.0 ms: 2.09x faster                                                           |
| pylint                     | 418 ms                                                          | 236 ms: 1.77x faster                                                            |
| logging_silent             | 119 ns                                                          | 68.8 ns: 1.73x faster                                                           |
| spectral_norm              | 122 ms                                                          | 73.7 ms: 1.65x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 15.2 ms: 1.56x faster                                                           |
| comprehensions             | 22.1 us                                                         | 14.6 us: 1.51x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.75 ms: 1.49x faster                                                           |
| unpack_sequence            | 65.2 ns                                                         | 44.3 ns: 1.47x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 1.03 ms: 1.45x faster                                                           |
| mako                       | 10.3 ms                                                         | 7.19 ms: 1.43x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 28.0 us: 1.43x faster                                                           |
| richards_super             | 58.7 ms                                                         | 42.3 ms: 1.39x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 7.10 ms: 1.38x faster                                                           |
| sqlglot_transpile          | 1.78 ms                                                         | 1.30 ms: 1.37x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 170 us: 1.36x faster                                                            |
| pickle_pure_python         | 309 us                                                          | 228 us: 1.35x faster                                                            |
| chaos                      | 84.4 ms                                                         | 62.4 ms: 1.35x faster                                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.14 ms: 1.35x faster                                                           |
| float                      | 76.1 ms                                                         | 56.4 ms: 1.35x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 6.00 ms: 1.35x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 112 ms: 1.33x faster                                                            |
| scimark_sor                | 135 ms                                                          | 102 ms: 1.32x faster                                                            |
| tomli_loads                | 2.31 sec                                                        | 1.77 sec: 1.31x faster                                                          |
| crypto_pyaes               | 79.4 ms                                                         | 60.8 ms: 1.31x faster                                                           |
| regex_compile              | 148 ms                                                          | 113 ms: 1.30x faster                                                            |
| nbody                      | 126 ms                                                          | 96.7 ms: 1.30x faster                                                           |
| logging_simple             | 10.8 us                                                         | 8.37 us: 1.29x faster                                                           |
| sympy_str                  | 283 ms                                                          | 219 ms: 1.29x faster                                                            |
| richards                   | 48.8 ms                                                         | 37.9 ms: 1.29x faster                                                           |
| deepcopy                   | 381 us                                                          | 296 us: 1.29x faster                                                            |
| xml_etree_process          | 55.0 ms                                                         | 42.8 ms: 1.28x faster                                                           |
| deepcopy_reduce            | 3.32 us                                                         | 2.59 us: 1.28x faster                                                           |
| async_tree_none            | 343 ms                                                          | 271 ms: 1.27x faster                                                            |
| logging_format             | 11.5 us                                                         | 9.07 us: 1.26x faster                                                           |
| pyflate                    | 471 ms                                                          | 385 ms: 1.22x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 16.3 ms: 1.22x faster                                                           |
| scimark_fft                | 291 ms                                                          | 242 ms: 1.21x faster                                                            |
| sympy_expand               | 462 ms                                                          | 383 ms: 1.21x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 339 ms: 1.21x faster                                                            |
| genshi_xml                 | 61.2 ms                                                         | 51.0 ms: 1.20x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 659 ms: 1.19x faster                                                            |
| tornado_http               | 118 ms                                                          | 99.9 ms: 1.18x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 86.9 ms: 1.18x faster                                                           |
| async_tree_io_tg           | 746 ms                                                          | 634 ms: 1.18x faster                                                            |
| nqueens                    | 111 ms                                                          | 94.7 ms: 1.18x faster                                                           |
| django_template            | 37.4 ms                                                         | 31.9 ms: 1.17x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 6.40 ms: 1.17x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.77 sec: 1.17x faster                                                          |
| async_tree_none_tg         | 301 ms                                                          | 258 ms: 1.17x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 325 ms: 1.16x faster                                                            |
| async_tree_io              | 754 ms                                                          | 649 ms: 1.16x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 61.7 ms: 1.16x faster                                                           |
| pycparser                  | 1.04 sec                                                        | 902 ms: 1.16x faster                                                            |
| raytrace                   | 327 ms                                                          | 284 ms: 1.15x faster                                                            |
| fannkuch                   | 399 ms                                                          | 347 ms: 1.15x faster                                                            |
| html5lib                   | 54.3 ms                                                         | 47.6 ms: 1.14x faster                                                           |
| go                         | 147 ms                                                          | 130 ms: 1.14x faster                                                            |
| sqlite_synth               | 2.15 us                                                         | 1.91 us: 1.13x faster                                                           |
| genshi_text                | 26.8 ms                                                         | 23.9 ms: 1.12x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 515 ms: 1.12x faster                                                            |
| docutils                   | 2.10 sec                                                        | 1.87 sec: 1.12x faster                                                          |
| unpickle_list              | 3.28 us                                                         | 2.93 us: 1.12x faster                                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.52 sec: 1.12x faster                                                          |
| json                       | 4.78 ms                                                         | 4.28 ms: 1.12x faster                                                           |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 529 ms: 1.12x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 68.3 ms: 1.11x faster                                                           |
| pprint_safe_repr           | 819 ms                                                          | 745 ms: 1.10x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 47.8 ms: 1.08x faster                                                           |
| scimark_monte_carlo        | 70.8 ms                                                         | 66.3 ms: 1.07x faster                                                           |
| bench_thread_pool          | 1.14 ms                                                         | 1.07 ms: 1.06x faster                                                           |
| 2to3                       | 282 ms                                                          | 266 ms: 1.06x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 85.9 ms: 1.06x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                            |
| pidigits                   | 203 ms                                                          | 198 ms: 1.02x faster                                                            |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| pickle_list                | 3.27 us                                                         | 3.28 us: 1.01x slower                                                           |
| json_loads                 | 20.0 us                                                         | 20.3 us: 1.01x slower                                                           |
| gc_traversal               | 1.38 ms                                                         | 1.40 ms: 1.02x slower                                                           |
| pickle                     | 7.99 us                                                         | 8.16 us: 1.02x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 74.5 ms: 1.05x slower                                                           |
| pathlib                    | 79.9 ms                                                         | 84.7 ms: 1.06x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.1 ms: 1.06x slower                                                           |
| regex_dna                  | 122 ms                                                          | 130 ms: 1.06x slower                                                            |
| regex_effbot               | 1.82 ms                                                         | 1.96 ms: 1.08x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 668 us: 1.08x slower                                                            |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.10x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.16 ms: 1.16x slower                                                           |
| async_generators           | 260 ms                                                          | 307 ms: 1.18x slower                                                            |
| python_startup             | 22.0 ms                                                         | 26.0 ms: 1.18x slower                                                           |
| dask                       | 355 ms                                                          | 439 ms: 1.24x slower                                                            |
| python_startup_no_site     | 18.8 ms                                                         | 24.0 ms: 1.28x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 241 ms: 2.13x slower                                                            |
| coverage                   | 58.0 ms                                                         | 497 ms: 8.57x slower                                                            |
| thrift                     | 801 us                                                          | 11.0 ms: 13.76x slower                                                          |
| Geometric mean             | (ref)                                                           | 1.12x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown