
# Results vs. 3.12.0

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-x86
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 241 ms: 1.16x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.74 ms: 1.35x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.73 sec: 1.15x faster                                                          |
| tornado_http   | 105 ms                                                          | 97.8 ms: 1.07x faster                                                           |
| Geometric mean | (ref)                                                           | 1.18x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 257 ms: 1.16x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 308 ms: 1.14x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 324 ms: 1.12x faster                                                            |
| async_tree_io              | 693 ms                                                          | 627 ms: 1.10x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 615 ms: 1.10x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 522 ms: 1.08x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 520 ms: 1.05x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 74.8 ms: 1.70x faster                                                           |
| float          | 76.7 ms                                                         | 54.5 ms: 1.41x faster                                                           |
| Geometric mean | (ref)                                                           | 1.34x faster                                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 97.1 ms: 1.33x faster                                                           |
| regex_effbot   | 2.04 ms                                                         | 1.94 ms: 1.05x faster                                                           |
| regex_dna      | 127 ms                                                          | 123 ms: 1.03x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.08x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 140 us: 1.50x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 198 us: 1.45x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.62 sec: 1.36x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 40.9 ms: 1.30x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 59.0 ms: 1.22x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.3 ms: 1.14x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.71 ms: 1.10x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.25 us: 1.04x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 112 ms: 1.01x faster                                                            |
| pickle_dict          | 19.9 us                                                         | 20.0 us: 1.01x slower                                                           |
| unpickle             | 9.71 us                                                         | 10.0 us: 1.03x slower                                                           |
| unpickle_list        | 2.95 us                                                         | 3.05 us: 1.03x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (2): pickle, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.9 ms: 1.07x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 21.5 ms: 1.13x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.10x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.12 ms: 1.40x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpack_sequence            | 62.5 ns                                                         | 35.7 ns: 1.75x faster                                                           |
| logging_silent             | 101 ns                                                          | 58.4 ns: 1.73x faster                                                           |
| generators                 | 38.5 ms                                                         | 22.6 ms: 1.70x faster                                                           |
| nbody                      | 127 ms                                                          | 74.8 ms: 1.70x faster                                                           |
| comprehensions             | 19.2 us                                                         | 11.3 us: 1.69x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 23.3 us: 1.65x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 4.17 ms: 1.63x faster                                                           |
| scimark_sor                | 130 ms                                                          | 82.6 ms: 1.57x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 59.9 ms: 1.56x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.34 ms: 1.53x faster                                                           |
| spectral_norm              | 104 ms                                                          | 68.1 ms: 1.52x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 140 us: 1.50x faster                                                            |
| raytrace                   | 308 ms                                                          | 212 ms: 1.45x faster                                                            |
| pickle_pure_python         | 286 us                                                          | 198 us: 1.45x faster                                                            |
| scimark_monte_carlo        | 66.4 ms                                                         | 46.0 ms: 1.44x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.23 us: 1.44x faster                                                           |
| chaos                      | 69.4 ms                                                         | 48.9 ms: 1.42x faster                                                           |
| typing_runtime_protocols   | 126 us                                                          | 89.6 us: 1.41x faster                                                           |
| float                      | 76.7 ms                                                         | 54.5 ms: 1.41x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.9 ms: 1.40x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.12 ms: 1.40x faster                                                           |
| scimark_fft                | 271 ms                                                          | 197 ms: 1.37x faster                                                            |
| deepcopy                   | 360 us                                                          | 263 us: 1.37x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.62 sec: 1.36x faster                                                          |
| sqlglot_parse              | 1.25 ms                                                         | 923 us: 1.35x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.74 ms: 1.35x faster                                                           |
| richards                   | 41.3 ms                                                         | 30.8 ms: 1.34x faster                                                           |
| go                         | 137 ms                                                          | 103 ms: 1.34x faster                                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 2.90 ms: 1.33x faster                                                           |
| pyflate                    | 424 ms                                                          | 319 ms: 1.33x faster                                                            |
| regex_compile              | 129 ms                                                          | 97.1 ms: 1.33x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 70.7 ms: 1.32x faster                                                           |
| richards_super             | 46.5 ms                                                         | 35.1 ms: 1.32x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.16 ms: 1.32x faster                                                           |
| fannkuch                   | 354 ms                                                          | 269 ms: 1.32x faster                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.15 sec: 1.31x faster                                                          |
| xml_etree_process          | 53.2 ms                                                         | 40.9 ms: 1.30x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 53.9 ms: 1.28x faster                                                           |
| pprint_safe_repr           | 721 ms                                                          | 569 ms: 1.27x faster                                                            |
| logging_simple             | 9.75 us                                                         | 7.88 us: 1.24x faster                                                           |
| pycparser                  | 978 ms                                                          | 791 ms: 1.24x faster                                                            |
| logging_format             | 10.4 us                                                         | 8.43 us: 1.23x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 59.0 ms: 1.22x faster                                                           |
| sympy_integrate            | 17.5 ms                                                         | 14.3 ms: 1.22x faster                                                           |
| sympy_str                  | 240 ms                                                          | 197 ms: 1.21x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 39.9 ms: 1.21x faster                                                           |
| sympy_sum                  | 123 ms                                                          | 102 ms: 1.21x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.61 sec: 1.19x faster                                                          |
| 2to3                       | 280 ms                                                          | 241 ms: 1.16x faster                                                            |
| async_generators           | 313 ms                                                          | 269 ms: 1.16x faster                                                            |
| async_tree_none            | 298 ms                                                          | 257 ms: 1.16x faster                                                            |
| sympy_expand               | 398 ms                                                          | 344 ms: 1.16x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                                            |
| meteor_contest             | 86.9 ms                                                         | 75.7 ms: 1.15x faster                                                           |
| docutils                   | 1.98 sec                                                        | 1.73 sec: 1.15x faster                                                          |
| sqlite_synth               | 2.07 us                                                         | 1.82 us: 1.14x faster                                                           |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.3 ms: 1.14x faster                                                           |
| async_tree_memoization_tg  | 350 ms                                                          | 308 ms: 1.14x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 324 ms: 1.12x faster                                                            |
| async_tree_io              | 693 ms                                                          | 627 ms: 1.10x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 6.71 ms: 1.10x faster                                                           |
| async_tree_io_tg           | 677 ms                                                          | 615 ms: 1.10x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 522 ms: 1.08x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.03 ms: 1.08x faster                                                           |
| tornado_http               | 105 ms                                                          | 97.8 ms: 1.07x faster                                                           |
| dask                       | 323 ms                                                          | 304 ms: 1.06x faster                                                            |
| regex_effbot               | 2.04 ms                                                         | 1.94 ms: 1.05x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 520 ms: 1.05x faster                                                            |
| pickle_list                | 3.37 us                                                         | 3.25 us: 1.04x faster                                                           |
| regex_dna                  | 127 ms                                                          | 123 ms: 1.03x faster                                                            |
| pathlib                    | 91.4 ms                                                         | 88.8 ms: 1.03x faster                                                           |
| json                       | 4.15 ms                                                         | 4.08 ms: 1.02x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.42 ms: 1.02x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 112 ms: 1.01x faster                                                            |
| pickle_dict                | 19.9 us                                                         | 20.0 us: 1.01x slower                                                           |
| unpickle                   | 9.71 us                                                         | 10.0 us: 1.03x slower                                                           |
| unpickle_list              | 2.95 us                                                         | 3.05 us: 1.03x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.06x slower                                                           |
| python_startup             | 22.4 ms                                                         | 23.9 ms: 1.07x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.97 ms: 1.08x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 21.5 ms: 1.13x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 205 ms: 2.05x slower                                                            |
| coverage                   | 48.4 ms                                                         | 484 ms: 9.99x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.18x faster                                                                    |

Benchmark hidden because not significant (7): pidigits, pickle, bench_mp_pool, json_loads, asyncio_tcp_ssl, create_gc_cycles, asyncio_tcp
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown