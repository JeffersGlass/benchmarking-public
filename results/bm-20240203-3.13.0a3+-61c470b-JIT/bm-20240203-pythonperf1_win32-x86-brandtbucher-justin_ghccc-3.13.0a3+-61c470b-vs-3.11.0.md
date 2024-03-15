
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_ghccc
- machine: windows-x86
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.28x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 247 ms: 1.14x faster                                                          |
| chameleon      | 8.08 ms                                                         | 5.72 ms: 1.41x faster                                                         |
| docutils       | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                        |
| tornado_http   | 118 ms                                                          | 99.1 ms: 1.19x faster                                                         |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 246 ms: 1.39x faster                                                          |
| async_tree_memoization     | 408 ms                                                          | 314 ms: 1.30x faster                                                          |
| async_tree_memoization_tg  | 378 ms                                                          | 292 ms: 1.29x faster                                                          |
| async_tree_none_tg         | 301 ms                                                          | 236 ms: 1.27x faster                                                          |
| async_tree_io              | 754 ms                                                          | 599 ms: 1.26x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 596 ms: 1.25x faster                                                          |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 510 ms: 1.13x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 522 ms: 1.13x faster                                                          |
| Geometric mean             | (ref)                                                           | 1.25x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 61.4 ms: 2.05x faster                                                         |
| float          | 76.1 ms                                                         | 49.8 ms: 1.53x faster                                                         |
| Geometric mean | (ref)                                                           | 1.47x faster                                                                  |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 99.2 ms: 1.49x faster                                                         |
| regex_dna      | 122 ms                                                          | 121 ms: 1.01x faster                                                          |
| regex_effbot   | 1.82 ms                                                         | 1.93 ms: 1.06x slower                                                         |
| regex_v8       | 15.2 ms                                                         | 16.4 ms: 1.08x slower                                                         |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| tomli_loads          | 2.31 sec                                                        | 1.46 sec: 1.59x faster                                                        |
| unpickle_pure_python | 231 us                                                          | 147 us: 1.57x faster                                                          |
| pickle_pure_python   | 309 us                                                          | 209 us: 1.48x faster                                                          |
| json_dumps           | 9.80 ms                                                         | 6.66 ms: 1.47x faster                                                         |
| xml_etree_process    | 55.0 ms                                                         | 40.5 ms: 1.36x faster                                                         |
| xml_etree_generate   | 71.6 ms                                                         | 57.8 ms: 1.24x faster                                                         |
| xml_etree_iterparse  | 75.6 ms                                                         | 65.0 ms: 1.16x faster                                                         |
| unpickle_list        | 3.28 us                                                         | 3.04 us: 1.08x faster                                                         |
| xml_etree_parse      | 114 ms                                                          | 110 ms: 1.04x faster                                                          |
| pickle_dict          | 20.1 us                                                         | 19.8 us: 1.01x faster                                                         |
| pickle_list          | 3.27 us                                                         | 3.24 us: 1.01x faster                                                         |
| json_loads           | 20.0 us                                                         | 20.3 us: 1.01x slower                                                         |
| pickle               | 7.99 us                                                         | 8.11 us: 1.02x slower                                                         |
| unpickle             | 9.23 us                                                         | 10.2 us: 1.10x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.18x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 23.2 ms: 1.05x slower                                                         |
| python_startup_no_site | 18.8 ms                                                         | 21.1 ms: 1.12x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.09x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 6.37 ms: 1.61x faster                                                         |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 98.0 us: 4.88x faster                                                         |
| generators                 | 52.2 ms                                                         | 22.2 ms: 2.35x faster                                                         |
| nbody                      | 126 ms                                                          | 61.4 ms: 2.05x faster                                                         |
| logging_silent             | 119 ns                                                          | 61.2 ns: 1.95x faster                                                         |
| spectral_norm              | 122 ms                                                          | 63.2 ms: 1.92x faster                                                         |
| deltablue                  | 4.10 ms                                                         | 2.18 ms: 1.88x faster                                                         |
| comprehensions             | 22.1 us                                                         | 12.1 us: 1.83x faster                                                         |
| deepcopy_memo              | 40.0 us                                                         | 22.8 us: 1.76x faster                                                         |
| richards_super             | 58.7 ms                                                         | 33.4 ms: 1.75x faster                                                         |
| sqlglot_parse              | 1.49 ms                                                         | 884 us: 1.69x faster                                                          |
| scimark_lu                 | 102 ms                                                          | 60.7 ms: 1.69x faster                                                         |
| richards                   | 48.8 ms                                                         | 29.5 ms: 1.65x faster                                                         |
| scimark_sor                | 135 ms                                                          | 82.3 ms: 1.64x faster                                                         |
| chaos                      | 84.4 ms                                                         | 51.6 ms: 1.64x faster                                                         |
| coroutines                 | 23.7 ms                                                         | 14.6 ms: 1.62x faster                                                         |
| mako                       | 10.3 ms                                                         | 6.37 ms: 1.61x faster                                                         |
| sqlglot_transpile          | 1.78 ms                                                         | 1.12 ms: 1.59x faster                                                         |
| tomli_loads                | 2.31 sec                                                        | 1.46 sec: 1.59x faster                                                        |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 2.69 ms: 1.57x faster                                                         |
| unpickle_pure_python       | 231 us                                                          | 147 us: 1.57x faster                                                          |
| crypto_pyaes               | 79.4 ms                                                         | 51.1 ms: 1.56x faster                                                         |
| raytrace                   | 327 ms                                                          | 213 ms: 1.54x faster                                                          |
| float                      | 76.1 ms                                                         | 49.8 ms: 1.53x faster                                                         |
| unpack_sequence            | 65.2 ns                                                         | 42.7 ns: 1.53x faster                                                         |
| fannkuch                   | 399 ms                                                          | 263 ms: 1.52x faster                                                          |
| nqueens                    | 111 ms                                                          | 73.7 ms: 1.51x faster                                                         |
| regex_compile              | 148 ms                                                          | 99.2 ms: 1.49x faster                                                         |
| scimark_fft                | 291 ms                                                          | 197 ms: 1.48x faster                                                          |
| pickle_pure_python         | 309 us                                                          | 209 us: 1.48x faster                                                          |
| json_dumps                 | 9.80 ms                                                         | 6.66 ms: 1.47x faster                                                         |
| pyflate                    | 471 ms                                                          | 325 ms: 1.45x faster                                                          |
| deepcopy                   | 381 us                                                          | 266 us: 1.43x faster                                                          |
| logging_simple             | 10.8 us                                                         | 7.63 us: 1.42x faster                                                         |
| chameleon                  | 8.08 ms                                                         | 5.72 ms: 1.41x faster                                                         |
| sympy_sum                  | 149 ms                                                          | 106 ms: 1.41x faster                                                          |
| async_tree_none            | 343 ms                                                          | 246 ms: 1.39x faster                                                          |
| deepcopy_reduce            | 3.32 us                                                         | 2.40 us: 1.38x faster                                                         |
| pprint_safe_repr           | 819 ms                                                          | 593 ms: 1.38x faster                                                          |
| sympy_str                  | 283 ms                                                          | 205 ms: 1.38x faster                                                          |
| pprint_pformat             | 1.70 sec                                                        | 1.23 sec: 1.38x faster                                                        |
| logging_format             | 11.5 us                                                         | 8.38 us: 1.37x faster                                                         |
| xml_etree_process          | 55.0 ms                                                         | 40.5 ms: 1.36x faster                                                         |
| hexiom                     | 7.51 ms                                                         | 5.70 ms: 1.32x faster                                                         |
| sympy_integrate            | 19.9 ms                                                         | 15.2 ms: 1.31x faster                                                         |
| async_tree_memoization     | 408 ms                                                          | 314 ms: 1.30x faster                                                          |
| go                         | 147 ms                                                          | 113 ms: 1.30x faster                                                          |
| sympy_expand               | 462 ms                                                          | 357 ms: 1.29x faster                                                          |
| async_tree_memoization_tg  | 378 ms                                                          | 292 ms: 1.29x faster                                                          |
| sqlglot_optimize           | 51.8 ms                                                         | 40.2 ms: 1.29x faster                                                         |
| async_tree_none_tg         | 301 ms                                                          | 236 ms: 1.27x faster                                                          |
| pycparser                  | 1.04 sec                                                        | 822 ms: 1.27x faster                                                          |
| async_tree_io              | 754 ms                                                          | 599 ms: 1.26x faster                                                          |
| async_tree_io_tg           | 746 ms                                                          | 596 ms: 1.25x faster                                                          |
| xml_etree_generate         | 71.6 ms                                                         | 57.8 ms: 1.24x faster                                                         |
| asyncio_tcp                | 787 ms                                                          | 647 ms: 1.22x faster                                                          |
| scimark_monte_carlo        | 70.8 ms                                                         | 58.6 ms: 1.21x faster                                                         |
| tornado_http               | 118 ms                                                          | 99.1 ms: 1.19x faster                                                         |
| sqlite_synth               | 2.15 us                                                         | 1.82 us: 1.18x faster                                                         |
| mdp                        | 2.07 sec                                                        | 1.75 sec: 1.18x faster                                                        |
| xml_etree_iterparse        | 75.6 ms                                                         | 65.0 ms: 1.16x faster                                                         |
| docutils                   | 2.10 sec                                                        | 1.81 sec: 1.16x faster                                                        |
| dask                       | 355 ms                                                          | 306 ms: 1.16x faster                                                          |
| 2to3                       | 282 ms                                                          | 247 ms: 1.14x faster                                                          |
| meteor_contest             | 90.9 ms                                                         | 79.4 ms: 1.14x faster                                                         |
| json                       | 4.78 ms                                                         | 4.22 ms: 1.13x faster                                                         |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 510 ms: 1.13x faster                                                          |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 522 ms: 1.13x faster                                                          |
| bench_thread_pool          | 1.14 ms                                                         | 1.05 ms: 1.08x faster                                                         |
| unpickle_list              | 3.28 us                                                         | 3.04 us: 1.08x faster                                                         |
| xml_etree_parse            | 114 ms                                                          | 110 ms: 1.04x faster                                                          |
| pickle_dict                | 20.1 us                                                         | 19.8 us: 1.01x faster                                                         |
| regex_dna                  | 122 ms                                                          | 121 ms: 1.01x faster                                                          |
| pickle_list                | 3.27 us                                                         | 3.24 us: 1.01x faster                                                         |
| json_loads                 | 20.0 us                                                         | 20.3 us: 1.01x slower                                                         |
| pickle                     | 7.99 us                                                         | 8.11 us: 1.02x slower                                                         |
| gc_traversal               | 1.38 ms                                                         | 1.40 ms: 1.02x slower                                                         |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 17.6 sec: 1.03x slower                                                        |
| bench_mp_pool              | 70.9 ms                                                         | 74.4 ms: 1.05x slower                                                         |
| python_startup             | 22.0 ms                                                         | 23.2 ms: 1.05x slower                                                         |
| regex_effbot               | 1.82 ms                                                         | 1.93 ms: 1.06x slower                                                         |
| telco                      | 5.29 ms                                                         | 5.68 ms: 1.07x slower                                                         |
| regex_v8                   | 15.2 ms                                                         | 16.4 ms: 1.08x slower                                                         |
| create_gc_cycles           | 618 us                                                          | 668 us: 1.08x slower                                                          |
| async_generators           | 260 ms                                                          | 282 ms: 1.08x slower                                                          |
| unpickle                   | 9.23 us                                                         | 10.2 us: 1.10x slower                                                         |
| pathlib                    | 79.9 ms                                                         | 88.8 ms: 1.11x slower                                                         |
| python_startup_no_site     | 18.8 ms                                                         | 21.1 ms: 1.12x slower                                                         |
| sqlglot_normalize          | 113 ms                                                          | 203 ms: 1.80x slower                                                          |
| coverage                   | 58.0 ms                                                         | 473 ms: 8.15x slower                                                          |
| Geometric mean             | (ref)                                                           | 1.28x faster                                                                  |

Benchmark hidden because not significant (1): pidigits
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: unknown