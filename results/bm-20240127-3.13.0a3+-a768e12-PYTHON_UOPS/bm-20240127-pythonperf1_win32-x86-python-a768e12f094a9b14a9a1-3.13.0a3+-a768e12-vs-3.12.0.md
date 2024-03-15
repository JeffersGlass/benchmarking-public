
# Results vs. 3.12.0

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-x86
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.14x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 247 ms: 1.13x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.87 ms: 1.32x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.80 sec: 1.10x faster                                                          |
| tornado_http   | 105 ms                                                          | 97.9 ms: 1.07x faster                                                           |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 255 ms: 1.17x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 305 ms: 1.15x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 319 ms: 1.14x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 596 ms: 1.14x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 489 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 506 ms: 1.11x faster                                                            |
| async_tree_io              | 693 ms                                                          | 623 ms: 1.11x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 84.7 ms: 1.50x faster                                                           |
| float          | 76.7 ms                                                         | 58.8 ms: 1.30x faster                                                           |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 106 ms: 1.22x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.92 ms: 1.06x faster                                                           |
| regex_dna      | 127 ms                                                          | 123 ms: 1.03x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.5 ms: 1.09x slower                                                           |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 152 us: 1.38x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.63 sec: 1.34x faster                                                          |
| pickle_pure_python   | 286 us                                                          | 214 us: 1.33x faster                                                            |
| xml_etree_process    | 53.2 ms                                                         | 41.7 ms: 1.28x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 61.2 ms: 1.18x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.5 ms: 1.13x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.89 ms: 1.07x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| pickle_list          | 3.37 us                                                         | 3.28 us: 1.03x faster                                                           |
| json_loads           | 20.4 us                                                         | 20.1 us: 1.01x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| unpickle             | 9.71 us                                                         | 9.83 us: 1.01x slower                                                           |
| pickle               | 7.79 us                                                         | 7.97 us: 1.02x slower                                                           |
| unpickle_list        | 2.95 us                                                         | 3.15 us: 1.07x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.4 ms: 1.05x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.6 ms: 1.08x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.70 ms: 1.29x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 60.4 ns: 1.67x faster                                                           |
| generators                 | 38.5 ms                                                         | 23.1 ms: 1.67x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 24.8 us: 1.55x faster                                                           |
| scimark_sor                | 130 ms                                                          | 84.9 ms: 1.53x faster                                                           |
| nbody                      | 127 ms                                                          | 84.7 ms: 1.50x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 42.0 ns: 1.49x faster                                                           |
| comprehensions             | 19.2 us                                                         | 13.0 us: 1.47x faster                                                           |
| raytrace                   | 308 ms                                                          | 211 ms: 1.46x faster                                                            |
| scimark_lu                 | 93.2 ms                                                         | 64.0 ms: 1.46x faster                                                           |
| richards_super             | 46.5 ms                                                         | 32.5 ms: 1.43x faster                                                           |
| richards                   | 41.3 ms                                                         | 29.4 ms: 1.41x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.9 ms: 1.40x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 904 us: 1.38x faster                                                            |
| unpickle_pure_python       | 210 us                                                          | 152 us: 1.38x faster                                                            |
| deltablue                  | 3.58 ms                                                         | 2.66 ms: 1.35x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.63 sec: 1.34x faster                                                          |
| deepcopy                   | 360 us                                                          | 269 us: 1.34x faster                                                            |
| pickle_pure_python         | 286 us                                                          | 214 us: 1.33x faster                                                            |
| chaos                      | 69.4 ms                                                         | 52.3 ms: 1.33x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.16 ms: 1.32x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 5.87 ms: 1.32x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 50.3 ms: 1.32x faster                                                           |
| typing_runtime_protocols   | 126 us                                                          | 96.1 us: 1.31x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 5.21 ms: 1.31x faster                                                           |
| float                      | 76.7 ms                                                         | 58.8 ms: 1.30x faster                                                           |
| spectral_norm              | 104 ms                                                          | 79.7 ms: 1.30x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.70 ms: 1.29x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.51 us: 1.29x faster                                                           |
| go                         | 137 ms                                                          | 107 ms: 1.28x faster                                                            |
| xml_etree_process          | 53.2 ms                                                         | 41.7 ms: 1.28x faster                                                           |
| pyflate                    | 424 ms                                                          | 337 ms: 1.26x faster                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.22 sec: 1.23x faster                                                          |
| regex_compile              | 129 ms                                                          | 106 ms: 1.22x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 57.1 ms: 1.21x faster                                                           |
| scimark_fft                | 271 ms                                                          | 225 ms: 1.21x faster                                                            |
| pprint_safe_repr           | 721 ms                                                          | 604 ms: 1.19x faster                                                            |
| logging_format             | 10.4 us                                                         | 8.75 us: 1.19x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.25 ms: 1.19x faster                                                           |
| logging_simple             | 9.75 us                                                         | 8.24 us: 1.18x faster                                                           |
| fannkuch                   | 354 ms                                                          | 299 ms: 1.18x faster                                                            |
| xml_etree_generate         | 72.1 ms                                                         | 61.2 ms: 1.18x faster                                                           |
| async_tree_none            | 298 ms                                                          | 255 ms: 1.17x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 41.7 ms: 1.16x faster                                                           |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 305 ms: 1.15x faster                                                            |
| nqueens                    | 93.7 ms                                                         | 81.8 ms: 1.15x faster                                                           |
| async_tree_memoization     | 364 ms                                                          | 319 ms: 1.14x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.68 sec: 1.14x faster                                                          |
| pycparser                  | 978 ms                                                          | 858 ms: 1.14x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 596 ms: 1.14x faster                                                            |
| 2to3                       | 280 ms                                                          | 247 ms: 1.13x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.5 ms: 1.13x faster                                                           |
| sympy_sum                  | 123 ms                                                          | 108 ms: 1.13x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.6 ms: 1.13x faster                                                           |
| sympy_str                  | 240 ms                                                          | 213 ms: 1.13x faster                                                            |
| async_generators           | 313 ms                                                          | 279 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 489 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 506 ms: 1.11x faster                                                            |
| async_tree_io              | 693 ms                                                          | 623 ms: 1.11x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.80 sec: 1.10x faster                                                          |
| sqlite_synth               | 2.07 us                                                         | 1.88 us: 1.10x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 80.0 ms: 1.09x faster                                                           |
| sympy_expand               | 398 ms                                                          | 367 ms: 1.08x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 6.89 ms: 1.07x faster                                                           |
| tornado_http               | 105 ms                                                          | 97.9 ms: 1.07x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.92 ms: 1.06x faster                                                           |
| dask                       | 323 ms                                                          | 308 ms: 1.05x faster                                                            |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.39 ms: 1.03x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 73.1 ms: 1.03x faster                                                           |
| regex_dna                  | 127 ms                                                          | 123 ms: 1.03x faster                                                            |
| pickle_list                | 3.37 us                                                         | 3.28 us: 1.03x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 89.2 ms: 1.03x faster                                                           |
| json_loads                 | 20.4 us                                                         | 20.1 us: 1.01x faster                                                           |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| unpickle                   | 9.71 us                                                         | 9.83 us: 1.01x slower                                                           |
| json                       | 4.15 ms                                                         | 4.22 ms: 1.02x slower                                                           |
| pickle                     | 7.79 us                                                         | 7.97 us: 1.02x slower                                                           |
| python_startup             | 22.4 ms                                                         | 23.4 ms: 1.05x slower                                                           |
| unpickle_list              | 2.95 us                                                         | 3.15 us: 1.07x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.92 ms: 1.07x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.6 ms: 1.08x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.5 ms: 1.09x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 212 ms: 2.11x slower                                                            |
| coverage                   | 48.4 ms                                                         | 489 ms: 10.09x slower                                                           |
| Geometric mean             | (ref)                                                           | 1.14x faster                                                                    |

Benchmark hidden because not significant (4): bench_thread_pool, asyncio_tcp, asyncio_tcp_ssl, create_gc_cycles
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown