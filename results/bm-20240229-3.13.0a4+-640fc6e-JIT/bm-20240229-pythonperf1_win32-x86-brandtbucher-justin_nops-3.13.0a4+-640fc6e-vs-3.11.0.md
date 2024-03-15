# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_nops
- machine: windows-x86
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 259 ms: 1.09x faster                                                         |
| chameleon      | 8.08 ms                                                         | 5.58 ms: 1.45x faster                                                        |
| docutils       | 2.10 sec                                                        | 1.79 sec: 1.17x faster                                                       |
| html5lib       | 54.3 ms                                                         | 44.4 ms: 1.22x faster                                                        |
| tornado_http   | 118 ms                                                          | 96.1 ms: 1.23x faster                                                        |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 261 ms: 1.32x faster                                                         |
| async_tree_memoization     | 408 ms                                                          | 324 ms: 1.26x faster                                                         |
| async_tree_memoization_tg  | 378 ms                                                          | 306 ms: 1.23x faster                                                         |
| async_tree_io_tg           | 746 ms                                                          | 611 ms: 1.22x faster                                                         |
| async_tree_none_tg         | 301 ms                                                          | 249 ms: 1.21x faster                                                         |
| async_tree_io              | 754 ms                                                          | 630 ms: 1.20x faster                                                         |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 509 ms: 1.13x faster                                                         |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 525 ms: 1.12x faster                                                         |
| Geometric mean             | (ref)                                                           | 1.21x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 55.0 ms: 1.38x faster                                                        |
| nbody          | 126 ms                                                          | 92.6 ms: 1.36x faster                                                        |
| pidigits       | 203 ms                                                          | 198 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 107 ms: 1.38x faster                                                         |
| regex_dna      | 122 ms                                                          | 118 ms: 1.03x faster                                                         |
| regex_effbot   | 1.82 ms                                                         | 1.87 ms: 1.03x slower                                                        |
| regex_v8       | 15.2 ms                                                         | 15.9 ms: 1.05x slower                                                        |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 309 us                                                          | 208 us: 1.48x faster                                                         |
| json_dumps           | 9.80 ms                                                         | 7.05 ms: 1.39x faster                                                        |
| tomli_loads          | 2.31 sec                                                        | 1.68 sec: 1.38x faster                                                       |
| unpickle_pure_python | 231 us                                                          | 168 us: 1.38x faster                                                         |
| xml_etree_process    | 55.0 ms                                                         | 42.5 ms: 1.29x faster                                                        |
| xml_etree_generate   | 71.6 ms                                                         | 61.8 ms: 1.16x faster                                                        |
| unpickle_list        | 3.28 us                                                         | 2.91 us: 1.13x faster                                                        |
| xml_etree_iterparse  | 75.6 ms                                                         | 67.2 ms: 1.13x faster                                                        |
| xml_etree_parse      | 114 ms                                                          | 109 ms: 1.05x faster                                                         |
| pickle_list          | 3.27 us                                                         | 3.23 us: 1.01x faster                                                        |
| pickle               | 7.99 us                                                         | 7.91 us: 1.01x faster                                                        |
| json_loads           | 20.0 us                                                         | 19.9 us: 1.01x faster                                                        |
| pickle_dict          | 20.1 us                                                         | 20.4 us: 1.02x slower                                                        |
| unpickle             | 9.23 us                                                         | 10.1 us: 1.09x slower                                                        |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 26.9 ms: 1.22x slower                                                        |
| python_startup_no_site | 18.8 ms                                                         | 24.4 ms: 1.30x slower                                                        |
| Geometric mean         | (ref)                                                           | 1.26x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.3 ms                                                         | 7.19 ms: 1.43x faster                                                        |
| django_template | 37.4 ms                                                         | 30.2 ms: 1.24x faster                                                        |
| genshi_xml      | 61.2 ms                                                         | 49.5 ms: 1.24x faster                                                        |
| genshi_text     | 26.8 ms                                                         | 23.4 ms: 1.14x faster                                                        |
| Geometric mean  | (ref)                                                           | 1.26x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 94.0 us: 5.09x faster                                                        |
| generators                 | 52.2 ms                                                         | 22.2 ms: 2.35x faster                                                        |
| logging_silent             | 119 ns                                                          | 59.6 ns: 2.00x faster                                                        |
| pylint                     | 418 ms                                                          | 227 ms: 1.84x faster                                                         |
| deepcopy_memo              | 40.0 us                                                         | 23.8 us: 1.68x faster                                                        |
| coroutines                 | 23.7 ms                                                         | 14.2 ms: 1.67x faster                                                        |
| deltablue                  | 4.10 ms                                                         | 2.55 ms: 1.61x faster                                                        |
| spectral_norm              | 122 ms                                                          | 77.2 ms: 1.58x faster                                                        |
| comprehensions             | 22.1 us                                                         | 14.1 us: 1.57x faster                                                        |
| sqlglot_parse              | 1.49 ms                                                         | 976 us: 1.53x faster                                                         |
| unpack_sequence            | 65.2 ns                                                         | 43.7 ns: 1.49x faster                                                        |
| pickle_pure_python         | 309 us                                                          | 208 us: 1.48x faster                                                         |
| sqlglot_transpile          | 1.78 ms                                                         | 1.21 ms: 1.47x faster                                                        |
| richards_super             | 58.7 ms                                                         | 40.3 ms: 1.46x faster                                                        |
| chameleon                  | 8.08 ms                                                         | 5.58 ms: 1.45x faster                                                        |
| chaos                      | 84.4 ms                                                         | 58.8 ms: 1.43x faster                                                        |
| mako                       | 10.3 ms                                                         | 7.19 ms: 1.43x faster                                                        |
| deepcopy_reduce            | 3.32 us                                                         | 2.38 us: 1.39x faster                                                        |
| sympy_sum                  | 149 ms                                                          | 107 ms: 1.39x faster                                                         |
| json_dumps                 | 9.80 ms                                                         | 7.05 ms: 1.39x faster                                                        |
| float                      | 76.1 ms                                                         | 55.0 ms: 1.38x faster                                                        |
| tomli_loads                | 2.31 sec                                                        | 1.68 sec: 1.38x faster                                                       |
| deepcopy                   | 381 us                                                          | 277 us: 1.38x faster                                                         |
| unpickle_pure_python       | 231 us                                                          | 168 us: 1.38x faster                                                         |
| regex_compile              | 148 ms                                                          | 107 ms: 1.38x faster                                                         |
| richards                   | 48.8 ms                                                         | 35.8 ms: 1.36x faster                                                        |
| nbody                      | 126 ms                                                          | 92.6 ms: 1.36x faster                                                        |
| sympy_str                  | 283 ms                                                          | 209 ms: 1.36x faster                                                         |
| crypto_pyaes               | 79.4 ms                                                         | 58.6 ms: 1.36x faster                                                        |
| scimark_sor                | 135 ms                                                          | 100 ms: 1.35x faster                                                         |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.14 ms: 1.35x faster                                                        |
| logging_simple             | 10.8 us                                                         | 8.07 us: 1.34x faster                                                        |
| logging_format             | 11.5 us                                                         | 8.63 us: 1.33x faster                                                        |
| async_tree_none            | 343 ms                                                          | 261 ms: 1.32x faster                                                         |
| xml_etree_process          | 55.0 ms                                                         | 42.5 ms: 1.29x faster                                                        |
| sympy_integrate            | 19.9 ms                                                         | 15.4 ms: 1.29x faster                                                        |
| sympy_expand               | 462 ms                                                          | 364 ms: 1.27x faster                                                         |
| async_tree_memoization     | 408 ms                                                          | 324 ms: 1.26x faster                                                         |
| raytrace                   | 327 ms                                                          | 263 ms: 1.24x faster                                                         |
| scimark_lu                 | 102 ms                                                          | 82.3 ms: 1.24x faster                                                        |
| scimark_fft                | 291 ms                                                          | 235 ms: 1.24x faster                                                         |
| django_template            | 37.4 ms                                                         | 30.2 ms: 1.24x faster                                                        |
| genshi_xml                 | 61.2 ms                                                         | 49.5 ms: 1.24x faster                                                        |
| async_tree_memoization_tg  | 378 ms                                                          | 306 ms: 1.23x faster                                                         |
| tornado_http               | 118 ms                                                          | 96.1 ms: 1.23x faster                                                        |
| asyncio_tcp                | 787 ms                                                          | 639 ms: 1.23x faster                                                         |
| pyflate                    | 471 ms                                                          | 383 ms: 1.23x faster                                                         |
| go                         | 147 ms                                                          | 120 ms: 1.22x faster                                                         |
| html5lib                   | 54.3 ms                                                         | 44.4 ms: 1.22x faster                                                        |
| async_tree_io_tg           | 746 ms                                                          | 611 ms: 1.22x faster                                                         |
| pycparser                  | 1.04 sec                                                        | 857 ms: 1.22x faster                                                         |
| nqueens                    | 111 ms                                                          | 91.9 ms: 1.21x faster                                                        |
| hexiom                     | 7.51 ms                                                         | 6.20 ms: 1.21x faster                                                        |
| async_tree_none_tg         | 301 ms                                                          | 249 ms: 1.21x faster                                                         |
| async_tree_io              | 754 ms                                                          | 630 ms: 1.20x faster                                                         |
| mdp                        | 2.07 sec                                                        | 1.74 sec: 1.19x faster                                                       |
| fannkuch                   | 399 ms                                                          | 339 ms: 1.18x faster                                                         |
| docutils                   | 2.10 sec                                                        | 1.79 sec: 1.17x faster                                                       |
| xml_etree_generate         | 71.6 ms                                                         | 61.8 ms: 1.16x faster                                                        |
| genshi_text                | 26.8 ms                                                         | 23.4 ms: 1.14x faster                                                        |
| json                       | 4.78 ms                                                         | 4.19 ms: 1.14x faster                                                        |
| sqlglot_optimize           | 51.8 ms                                                         | 45.5 ms: 1.14x faster                                                        |
| pprint_pformat             | 1.70 sec                                                        | 1.49 sec: 1.14x faster                                                       |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 509 ms: 1.13x faster                                                         |
| unpickle_list              | 3.28 us                                                         | 2.91 us: 1.13x faster                                                        |
| xml_etree_iterparse        | 75.6 ms                                                         | 67.2 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 525 ms: 1.12x faster                                                         |
| pprint_safe_repr           | 819 ms                                                          | 733 ms: 1.12x faster                                                         |
| bench_thread_pool          | 1.14 ms                                                         | 1.03 ms: 1.11x faster                                                        |
| 2to3                       | 282 ms                                                          | 259 ms: 1.09x faster                                                         |
| sqlite_synth               | 2.15 us                                                         | 1.97 us: 1.09x faster                                                        |
| scimark_monte_carlo        | 70.8 ms                                                         | 65.1 ms: 1.09x faster                                                        |
| meteor_contest             | 90.9 ms                                                         | 84.5 ms: 1.08x faster                                                        |
| xml_etree_parse            | 114 ms                                                          | 109 ms: 1.05x faster                                                         |
| regex_dna                  | 122 ms                                                          | 118 ms: 1.03x faster                                                         |
| pidigits                   | 203 ms                                                          | 198 ms: 1.02x faster                                                         |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.02x faster                                                       |
| pickle_list                | 3.27 us                                                         | 3.23 us: 1.01x faster                                                        |
| pickle                     | 7.99 us                                                         | 7.91 us: 1.01x faster                                                        |
| json_loads                 | 20.0 us                                                         | 19.9 us: 1.01x faster                                                        |
| pickle_dict                | 20.1 us                                                         | 20.4 us: 1.02x slower                                                        |
| gc_traversal               | 1.38 ms                                                         | 1.41 ms: 1.02x slower                                                        |
| regex_effbot               | 1.82 ms                                                         | 1.87 ms: 1.03x slower                                                        |
| regex_v8                   | 15.2 ms                                                         | 15.9 ms: 1.05x slower                                                        |
| pathlib                    | 79.9 ms                                                         | 84.2 ms: 1.05x slower                                                        |
| create_gc_cycles           | 618 us                                                          | 663 us: 1.07x slower                                                         |
| unpickle                   | 9.23 us                                                         | 10.1 us: 1.09x slower                                                        |
| async_generators           | 260 ms                                                          | 283 ms: 1.09x slower                                                         |
| bench_mp_pool              | 70.9 ms                                                         | 77.5 ms: 1.09x slower                                                        |
| dask                       | 355 ms                                                          | 418 ms: 1.18x slower                                                         |
| telco                      | 5.29 ms                                                         | 6.34 ms: 1.20x slower                                                        |
| python_startup             | 22.0 ms                                                         | 26.9 ms: 1.22x slower                                                        |
| python_startup_no_site     | 18.8 ms                                                         | 24.4 ms: 1.30x slower                                                        |
| sqlglot_normalize          | 113 ms                                                          | 223 ms: 1.97x slower                                                         |
| coverage                   | 58.0 ms                                                         | 490 ms: 8.44x slower                                                         |
| thrift                     | 801 us                                                          | 10.7 ms: 13.36x slower                                                       |
| Geometric mean             | (ref)                                                           | 1.16x faster                                                                 |
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown