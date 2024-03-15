
# Results vs. 3.11.0

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: windows-x86
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 246 ms: 1.15x faster                                                            |
| chameleon      | 8.08 ms                                                         | 6.02 ms: 1.34x faster                                                           |
| docutils       | 2.10 sec                                                        | 1.78 sec: 1.18x faster                                                          |
| tornado_http   | 118 ms                                                          | 95.7 ms: 1.24x faster                                                           |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 343 ms                                                          | 250 ms: 1.37x faster                                                            |
| async_tree_memoization     | 408 ms                                                          | 311 ms: 1.31x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 585 ms: 1.28x faster                                                            |
| async_tree_none_tg         | 301 ms                                                          | 237 ms: 1.27x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 298 ms: 1.27x faster                                                            |
| async_tree_io              | 754 ms                                                          | 597 ms: 1.26x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 510 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 501 ms: 1.15x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.26x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.1 ms                                                         | 53.8 ms: 1.41x faster                                                           |
| nbody          | 126 ms                                                          | 90.6 ms: 1.39x faster                                                           |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 105 ms: 1.41x faster                                                            |
| regex_dna      | 122 ms                                                          | 117 ms: 1.04x faster                                                            |
| regex_effbot   | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| regex_v8       | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.08x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 150 us: 1.54x faster                                                            |
| pickle_pure_python   | 309 us                                                          | 205 us: 1.51x faster                                                            |
| json_dumps           | 9.80 ms                                                         | 6.71 ms: 1.46x faster                                                           |
| tomli_loads          | 2.31 sec                                                        | 1.59 sec: 1.45x faster                                                          |
| xml_etree_process    | 55.0 ms                                                         | 41.4 ms: 1.33x faster                                                           |
| xml_etree_generate   | 71.6 ms                                                         | 60.4 ms: 1.19x faster                                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 65.5 ms: 1.15x faster                                                           |
| xml_etree_parse      | 114 ms                                                          | 104 ms: 1.10x faster                                                            |
| unpickle_list        | 3.28 us                                                         | 3.10 us: 1.06x faster                                                           |
| pickle_dict          | 20.1 us                                                         | 19.8 us: 1.02x faster                                                           |
| pickle               | 7.99 us                                                         | 8.13 us: 1.02x slower                                                           |
| unpickle             | 9.23 us                                                         | 10.2 us: 1.10x slower                                                           |
| pickle_list          | 3.27 us                                                         | 3.66 us: 1.12x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.16x faster                                                                    |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.0 ms                                                         | 22.3 ms: 1.01x slower                                                           |
| python_startup_no_site | 18.8 ms                                                         | 20.1 ms: 1.07x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.04x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 10.3 ms                                                         | 7.64 ms: 1.35x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 478 us                                                          | 93.8 us: 5.10x faster                                                           |
| generators                 | 52.2 ms                                                         | 22.4 ms: 2.33x faster                                                           |
| logging_silent             | 119 ns                                                          | 60.5 ns: 1.97x faster                                                           |
| richards_super             | 58.7 ms                                                         | 32.3 ms: 1.82x faster                                                           |
| deepcopy_memo              | 40.0 us                                                         | 22.7 us: 1.76x faster                                                           |
| deltablue                  | 4.10 ms                                                         | 2.38 ms: 1.72x faster                                                           |
| richards                   | 48.8 ms                                                         | 28.4 ms: 1.72x faster                                                           |
| scimark_lu                 | 102 ms                                                          | 60.1 ms: 1.70x faster                                                           |
| scimark_sor                | 135 ms                                                          | 79.9 ms: 1.69x faster                                                           |
| coroutines                 | 23.7 ms                                                         | 14.4 ms: 1.65x faster                                                           |
| sqlglot_parse              | 1.49 ms                                                         | 932 us: 1.60x faster                                                            |
| unpack_sequence            | 65.2 ns                                                         | 41.2 ns: 1.58x faster                                                           |
| spectral_norm              | 122 ms                                                          | 78.4 ms: 1.55x faster                                                           |
| unpickle_pure_python       | 231 us                                                          | 150 us: 1.54x faster                                                            |
| sqlglot_transpile          | 1.78 ms                                                         | 1.18 ms: 1.52x faster                                                           |
| pickle_pure_python         | 309 us                                                          | 205 us: 1.51x faster                                                            |
| comprehensions             | 22.1 us                                                         | 14.7 us: 1.50x faster                                                           |
| json_dumps                 | 9.80 ms                                                         | 6.71 ms: 1.46x faster                                                           |
| tomli_loads                | 2.31 sec                                                        | 1.59 sec: 1.45x faster                                                          |
| raytrace                   | 327 ms                                                          | 228 ms: 1.43x faster                                                            |
| float                      | 76.1 ms                                                         | 53.8 ms: 1.41x faster                                                           |
| regex_compile              | 148 ms                                                          | 105 ms: 1.41x faster                                                            |
| deepcopy_reduce            | 3.32 us                                                         | 2.37 us: 1.40x faster                                                           |
| nbody                      | 126 ms                                                          | 90.6 ms: 1.39x faster                                                           |
| deepcopy                   | 381 us                                                          | 276 us: 1.38x faster                                                            |
| async_tree_none            | 343 ms                                                          | 250 ms: 1.37x faster                                                            |
| chaos                      | 84.4 ms                                                         | 61.8 ms: 1.37x faster                                                           |
| fannkuch                   | 399 ms                                                          | 293 ms: 1.36x faster                                                            |
| logging_simple             | 10.8 us                                                         | 7.97 us: 1.36x faster                                                           |
| sympy_sum                  | 149 ms                                                          | 110 ms: 1.35x faster                                                            |
| mako                       | 10.3 ms                                                         | 7.64 ms: 1.35x faster                                                           |
| chameleon                  | 8.08 ms                                                         | 6.02 ms: 1.34x faster                                                           |
| logging_format             | 11.5 us                                                         | 8.57 us: 1.34x faster                                                           |
| xml_etree_process          | 55.0 ms                                                         | 41.4 ms: 1.33x faster                                                           |
| scimark_sparse_mat_mult    | 4.23 ms                                                         | 3.19 ms: 1.33x faster                                                           |
| sympy_str                  | 283 ms                                                          | 214 ms: 1.32x faster                                                            |
| crypto_pyaes               | 79.4 ms                                                         | 60.4 ms: 1.31x faster                                                           |
| async_tree_memoization     | 408 ms                                                          | 311 ms: 1.31x faster                                                            |
| nqueens                    | 111 ms                                                          | 86.1 ms: 1.29x faster                                                           |
| asyncio_tcp                | 787 ms                                                          | 609 ms: 1.29x faster                                                            |
| async_tree_io_tg           | 746 ms                                                          | 585 ms: 1.28x faster                                                            |
| sympy_integrate            | 19.9 ms                                                         | 15.6 ms: 1.27x faster                                                           |
| async_tree_none_tg         | 301 ms                                                          | 237 ms: 1.27x faster                                                            |
| async_tree_memoization_tg  | 378 ms                                                          | 298 ms: 1.27x faster                                                            |
| go                         | 147 ms                                                          | 116 ms: 1.26x faster                                                            |
| async_tree_io              | 754 ms                                                          | 597 ms: 1.26x faster                                                            |
| sympy_expand               | 462 ms                                                          | 372 ms: 1.24x faster                                                            |
| pycparser                  | 1.04 sec                                                        | 843 ms: 1.24x faster                                                            |
| tornado_http               | 118 ms                                                          | 95.7 ms: 1.24x faster                                                           |
| pyflate                    | 471 ms                                                          | 383 ms: 1.23x faster                                                            |
| pprint_pformat             | 1.70 sec                                                        | 1.39 sec: 1.22x faster                                                          |
| pprint_safe_repr           | 819 ms                                                          | 674 ms: 1.22x faster                                                            |
| sqlglot_optimize           | 51.8 ms                                                         | 42.8 ms: 1.21x faster                                                           |
| hexiom                     | 7.51 ms                                                         | 6.30 ms: 1.19x faster                                                           |
| dask                       | 355 ms                                                          | 298 ms: 1.19x faster                                                            |
| xml_etree_generate         | 71.6 ms                                                         | 60.4 ms: 1.19x faster                                                           |
| docutils                   | 2.10 sec                                                        | 1.78 sec: 1.18x faster                                                          |
| json                       | 4.78 ms                                                         | 4.08 ms: 1.17x faster                                                           |
| sqlite_synth               | 2.15 us                                                         | 1.84 us: 1.17x faster                                                           |
| scimark_fft                | 291 ms                                                          | 251 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed    | 590 ms                                                          | 510 ms: 1.16x faster                                                            |
| xml_etree_iterparse        | 75.6 ms                                                         | 65.5 ms: 1.15x faster                                                           |
| async_tree_cpu_io_mixed_tg | 577 ms                                                          | 501 ms: 1.15x faster                                                            |
| 2to3                       | 282 ms                                                          | 246 ms: 1.15x faster                                                            |
| bench_thread_pool          | 1.14 ms                                                         | 1.02 ms: 1.12x faster                                                           |
| xml_etree_parse            | 114 ms                                                          | 104 ms: 1.10x faster                                                            |
| meteor_contest             | 90.9 ms                                                         | 82.6 ms: 1.10x faster                                                           |
| mdp                        | 2.07 sec                                                        | 1.89 sec: 1.10x faster                                                          |
| unpickle_list              | 3.28 us                                                         | 3.10 us: 1.06x faster                                                           |
| regex_dna                  | 122 ms                                                          | 117 ms: 1.04x faster                                                            |
| scimark_monte_carlo        | 70.8 ms                                                         | 68.8 ms: 1.03x faster                                                           |
| asyncio_tcp_ssl            | 17.1 sec                                                        | 16.8 sec: 1.02x faster                                                          |
| pickle_dict                | 20.1 us                                                         | 19.8 us: 1.02x faster                                                           |
| python_startup             | 22.0 ms                                                         | 22.3 ms: 1.01x slower                                                           |
| bench_mp_pool              | 70.9 ms                                                         | 72.0 ms: 1.02x slower                                                           |
| pickle                     | 7.99 us                                                         | 8.13 us: 1.02x slower                                                           |
| regex_effbot               | 1.82 ms                                                         | 1.89 ms: 1.04x slower                                                           |
| create_gc_cycles           | 618 us                                                          | 640 us: 1.04x slower                                                            |
| pathlib                    | 79.9 ms                                                         | 83.9 ms: 1.05x slower                                                           |
| regex_v8                   | 15.2 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| async_generators           | 260 ms                                                          | 277 ms: 1.07x slower                                                            |
| python_startup_no_site     | 18.8 ms                                                         | 20.1 ms: 1.07x slower                                                           |
| unpickle                   | 9.23 us                                                         | 10.2 us: 1.10x slower                                                           |
| pickle_list                | 3.27 us                                                         | 3.66 us: 1.12x slower                                                           |
| telco                      | 5.29 ms                                                         | 6.11 ms: 1.15x slower                                                           |
| sqlglot_normalize          | 113 ms                                                          | 219 ms: 1.94x slower                                                            |
| coverage                   | 58.0 ms                                                         | 465 ms: 8.01x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.23x faster                                                                    |

Benchmark hidden because not significant (3): pidigits, json_loads, gc_traversal
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: unknown