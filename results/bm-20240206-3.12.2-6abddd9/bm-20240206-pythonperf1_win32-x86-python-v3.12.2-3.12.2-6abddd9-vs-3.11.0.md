
# Results vs. 3.11.0

- fork: python
- ref: v3.12.2
- machine: windows-x86
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.11x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 274 ms: 1.03x faster                                            |
| chameleon      | 8.08 ms                                                         | 7.50 ms: 1.08x faster                                           |
| docutils       | 2.10 sec                                                        | 1.93 sec: 1.09x faster                                          |
| tornado_http   | 118 ms                                                          | 104 ms: 1.14x faster                                            |
| Geometric mean | (ref)                                                           | 1.08x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 299 ms: 1.15x faster                                            |
| async_tree_memoization     | 408 ms                                                          | 358 ms: 1.14x faster                                            |
| async_tree_io_tg           | 746 ms                                                          | 661 ms: 1.13x faster                                            |
| async_tree_io              | 754 ms                                                          | 678 ms: 1.11x faster                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 341 ms: 1.11x faster                                            |
| async_tree_none_tg         | 301 ms                                                          | 273 ms: 1.10x faster                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 538 ms: 1.07x faster                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 555 ms: 1.06x faster                                            |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 73.6 ms: 1.03x faster                                           |
| pidigits       | 203 ms                                                          | 198 ms: 1.03x faster                                            |
| nbody          | 126 ms                                                          | 124 ms: 1.02x faster                                            |
| Geometric mean | (ref)                                                           | 1.03x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 126 ms: 1.17x faster                                            |
| regex_dna      | 122 ms                                                          | 120 ms: 1.01x faster                                            |
| regex_v8       | 15.2 ms                                                         | 15.4 ms: 1.01x slower                                           |
| regex_effbot   | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 9.80 ms                                                         | 7.47 ms: 1.31x faster                                           |
| unpickle_pure_python | 231 us                                                          | 205 us: 1.13x faster                                            |
| unpickle_list        | 3.28 us                                                         | 2.96 us: 1.11x faster                                           |
| pickle_pure_python   | 309 us                                                          | 286 us: 1.08x faster                                            |
| tomli_loads          | 2.31 sec                                                        | 2.17 sec: 1.06x faster                                          |
| xml_etree_parse      | 114 ms                                                          | 111 ms: 1.03x faster                                            |
| xml_etree_process    | 55.0 ms                                                         | 53.9 ms: 1.02x faster                                           |
| pickle               | 7.99 us                                                         | 7.85 us: 1.02x faster                                           |
| json_loads           | 20.0 us                                                         | 20.3 us: 1.01x slower                                           |
| xml_etree_generate   | 71.6 ms                                                         | 72.8 ms: 1.02x slower                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 77.1 ms: 1.02x slower                                           |
| unpickle             | 9.23 us                                                         | 9.42 us: 1.02x slower                                           |
| Geometric mean       | (ref)                                                           | 1.05x faster                                                    |

Benchmark hidden because not significant (2): pickle_list, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 18.8 ms                                                         | 18.1 ms: 1.04x faster                                           |
| python_startup         | 22.0 ms                                                         | 21.3 ms: 1.03x faster                                           |
| Geometric mean         | (ref)                                                           | 1.03x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 10.3 ms                                                         | 9.80 ms: 1.05x faster                                           |
| django_template | 37.4 ms                                                         | 36.1 ms: 1.04x faster                                           |
| Geometric mean  | (ref)                                                           | 1.04x faster                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 113 us: 4.24x faster                                            |
| generators                 | 52.2 ms                                                         | 38.1 ms: 1.37x faster                                           |
| json_dumps                 | 9.80 ms                                                         | 7.47 ms: 1.31x faster                                           |
| sqlalchemy_imperative      | 15.4 ms                                                         | 11.9 ms: 1.29x faster                                           |
| richards_super             | 58.7 ms                                                         | 46.9 ms: 1.25x faster                                           |
| sympy_sum                  | 149 ms                                                          | 120 ms: 1.24x faster                                            |
| chaos                      | 84.4 ms                                                         | 68.0 ms: 1.24x faster                                           |
| asyncio_tcp                | 787 ms                                                          | 645 ms: 1.22x faster                                            |
| coverage                   | 58.0 ms                                                         | 48.0 ms: 1.21x faster                                           |
| sqlglot_parse              | 1.49 ms                                                         | 1.24 ms: 1.20x faster                                           |
| sympy_str                  | 283 ms                                                          | 238 ms: 1.19x faster                                            |
| spectral_norm              | 122 ms                                                          | 102 ms: 1.19x faster                                            |
| logging_silent             | 119 ns                                                          | 101 ns: 1.18x faster                                            |
| mypy2                      | 626 ms                                                          | 529 ms: 1.18x faster                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.51 ms: 1.18x faster                                           |
| sympy_expand               | 462 ms                                                          | 393 ms: 1.18x faster                                            |
| nqueens                    | 111 ms                                                          | 94.8 ms: 1.17x faster                                           |
| regex_compile              | 148 ms                                                          | 126 ms: 1.17x faster                                            |
| richards                   | 48.8 ms                                                         | 41.8 ms: 1.17x faster                                           |
| deltablue                  | 4.10 ms                                                         | 3.52 ms: 1.17x faster                                           |
| crypto_pyaes               | 79.4 ms                                                         | 68.5 ms: 1.16x faster                                           |
| sympy_integrate            | 19.9 ms                                                         | 17.2 ms: 1.16x faster                                           |
| coroutines                 | 23.7 ms                                                         | 20.7 ms: 1.15x faster                                           |
| async_tree_none            | 343 ms                                                          | 299 ms: 1.15x faster                                            |
| aiohttp                    | 1.17 ms                                                         | 1.02 ms: 1.15x faster                                           |
| sqlalchemy_declarative     | 115 ms                                                          | 101 ms: 1.14x faster                                            |
| tornado_http               | 118 ms                                                          | 104 ms: 1.14x faster                                            |
| async_tree_memoization     | 408 ms                                                          | 358 ms: 1.14x faster                                            |
| logging_simple             | 10.8 us                                                         | 9.50 us: 1.14x faster                                           |
| pprint_pformat             | 1.70 sec                                                        | 1.50 sec: 1.13x faster                                          |
| logging_format             | 11.5 us                                                         | 10.1 us: 1.13x faster                                           |
| mdp                        | 2.07 sec                                                        | 1.83 sec: 1.13x faster                                          |
| pyflate                    | 471 ms                                                          | 417 ms: 1.13x faster                                            |
| unpickle_pure_python       | 231 us                                                          | 205 us: 1.13x faster                                            |
| async_tree_io_tg           | 746 ms                                                          | 661 ms: 1.13x faster                                            |
| dulwich_log                | 62.8 ms                                                         | 55.7 ms: 1.13x faster                                           |
| json                       | 4.78 ms                                                         | 4.24 ms: 1.13x faster                                           |
| comprehensions             | 22.1 us                                                         | 19.6 us: 1.13x faster                                           |
| pprint_safe_repr           | 819 ms                                                          | 728 ms: 1.13x faster                                            |
| sqlglot_normalize          | 113 ms                                                          | 102 ms: 1.11x faster                                            |
| async_tree_io              | 754 ms                                                          | 678 ms: 1.11x faster                                            |
| hexiom                     | 7.51 ms                                                         | 6.75 ms: 1.11x faster                                           |
| async_tree_memoization_tg  | 378 ms                                                          | 341 ms: 1.11x faster                                            |
| unpickle_list              | 3.28 us                                                         | 2.96 us: 1.11x faster                                           |
| dask                       | 355 ms                                                          | 321 ms: 1.11x faster                                            |
| async_tree_none_tg         | 301 ms                                                          | 273 ms: 1.10x faster                                            |
| go                         | 147 ms                                                          | 134 ms: 1.10x faster                                            |
| pycparser                  | 1.04 sec                                                        | 955 ms: 1.09x faster                                            |
| fannkuch                   | 399 ms                                                          | 367 ms: 1.09x faster                                            |
| raytrace                   | 327 ms                                                          | 301 ms: 1.09x faster                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 47.6 ms: 1.09x faster                                           |
| docutils                   | 2.10 sec                                                        | 1.93 sec: 1.09x faster                                          |
| scimark_lu                 | 102 ms                                                          | 94.0 ms: 1.09x faster                                           |
| scimark_fft                | 291 ms                                                          | 269 ms: 1.08x faster                                            |
| pickle_pure_python         | 309 us                                                          | 286 us: 1.08x faster                                            |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.93 ms: 1.08x faster                                           |
| chameleon                  | 8.08 ms                                                         | 7.50 ms: 1.08x faster                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 538 ms: 1.07x faster                                            |
| deepcopy                   | 381 us                                                          | 358 us: 1.07x faster                                            |
| tomli_loads                | 2.31 sec                                                        | 2.17 sec: 1.06x faster                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 555 ms: 1.06x faster                                            |
| deepcopy_memo              | 40.0 us                                                         | 37.8 us: 1.06x faster                                           |
| scimark_monte_carlo        | 70.8 ms                                                         | 67.3 ms: 1.05x faster                                           |
| unpack_sequence            | 65.2 ns                                                         | 62.1 ns: 1.05x faster                                           |
| meteor_contest             | 90.9 ms                                                         | 86.5 ms: 1.05x faster                                           |
| mako                       | 10.3 ms                                                         | 9.80 ms: 1.05x faster                                           |
| scimark_sor                | 135 ms                                                          | 130 ms: 1.04x faster                                            |
| bench_thread_pool          | 1.14 ms                                                         | 1.09 ms: 1.04x faster                                           |
| python_startup_no_site     | 18.8 ms                                                         | 18.1 ms: 1.04x faster                                           |
| django_template            | 37.4 ms                                                         | 36.1 ms: 1.04x faster                                           |
| float                      | 76.1 ms                                                         | 73.6 ms: 1.03x faster                                           |
| xml_etree_parse            | 114 ms                                                          | 111 ms: 1.03x faster                                            |
| python_startup             | 22.0 ms                                                         | 21.3 ms: 1.03x faster                                           |
| 2to3                       | 282 ms                                                          | 274 ms: 1.03x faster                                            |
| sqlite_synth               | 2.15 us                                                         | 2.09 us: 1.03x faster                                           |
| pidigits                   | 203 ms                                                          | 198 ms: 1.03x faster                                            |
| deepcopy_reduce            | 3.32 us                                                         | 3.24 us: 1.02x faster                                           |
| xml_etree_process          | 55.0 ms                                                         | 53.9 ms: 1.02x faster                                           |
| nbody                      | 126 ms                                                          | 124 ms: 1.02x faster                                            |
| pickle                     | 7.99 us                                                         | 7.85 us: 1.02x faster                                           |
| telco                      | 5.29 ms                                                         | 5.22 ms: 1.02x faster                                           |
| regex_dna                  | 122 ms                                                          | 120 ms: 1.01x faster                                            |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.9 sec: 1.01x faster                                          |
| bench_mp_pool              | 70.9 ms                                                         | 71.6 ms: 1.01x slower                                           |
| json_loads                 | 20.0 us                                                         | 20.3 us: 1.01x slower                                           |
| regex_v8                   | 15.2 ms                                                         | 15.4 ms: 1.01x slower                                           |
| xml_etree_generate         | 71.6 ms                                                         | 72.8 ms: 1.02x slower                                           |
| gc_traversal               | 1.38 ms                                                         | 1.40 ms: 1.02x slower                                           |
| xml_etree_iterparse        | 75.6 ms                                                         | 77.1 ms: 1.02x slower                                           |
| unpickle                   | 9.23 us                                                         | 9.42 us: 1.02x slower                                           |
| create_gc_cycles           | 618 us                                                          | 641 us: 1.04x slower                                            |
| regex_effbot               | 1.82 ms                                                         | 1.90 ms: 1.04x slower                                           |
| pathlib                    | 79.9 ms                                                         | 85.1 ms: 1.06x slower                                           |
| async_generators           | 260 ms                                                          | 307 ms: 1.18x slower                                            |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                    |

Benchmark hidden because not significant (2): pickle_list, pickle_dict
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown