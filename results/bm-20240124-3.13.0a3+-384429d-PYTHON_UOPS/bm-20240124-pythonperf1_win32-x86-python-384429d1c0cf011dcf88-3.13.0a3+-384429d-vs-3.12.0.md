
# Results vs. 3.12.0

- fork: python
- ref: 384429d1c0cf011dcf88
- machine: windows-x86
- commit hash: 384429d
- commit date: 2024-01-24
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 246 ms: 1.14x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.79 ms: 1.34x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.84 sec: 1.08x faster                                                          |
| tornado_http   | 105 ms                                                          | 99.1 ms: 1.06x faster                                                           |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                                            |
| async_tree_none            | 298 ms                                                          | 261 ms: 1.14x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 310 ms: 1.13x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 603 ms: 1.12x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 328 ms: 1.11x faster                                                            |
| async_tree_io              | 693 ms                                                          | 628 ms: 1.10x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 511 ms: 1.10x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 504 ms: 1.08x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.12x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 88.5 ms: 1.44x faster                                                           |
| float          | 76.7 ms                                                         | 59.3 ms: 1.29x faster                                                           |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 107 ms: 1.21x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| regex_dna      | 127 ms                                                          | 119 ms: 1.07x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 150 us: 1.40x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 208 us: 1.37x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.68 sec: 1.31x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 42.2 ms: 1.26x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 61.7 ms: 1.17x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.51 ms: 1.14x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 71.1 ms: 1.09x faster                                                           |
| json_loads           | 20.4 us                                                         | 19.7 us: 1.03x faster                                                           |
| unpickle             | 9.71 us                                                         | 9.57 us: 1.01x faster                                                           |
| pickle               | 7.79 us                                                         | 7.74 us: 1.01x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 19.8 us: 1.01x faster                                                           |
| unpickle_list        | 2.95 us                                                         | 3.07 us: 1.04x slower                                                           |
| pickle_list          | 3.37 us                                                         | 3.74 us: 1.11x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.2 ms: 1.04x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.7 ms: 1.08x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 8.03 ms: 1.24x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 61.8 ns: 1.63x faster                                                           |
| generators                 | 38.5 ms                                                         | 23.6 ms: 1.63x faster                                                           |
| scimark_sor                | 130 ms                                                          | 81.0 ms: 1.60x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 24.0 us: 1.60x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 62.3 ms: 1.50x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 42.6 ns: 1.47x faster                                                           |
| raytrace                   | 308 ms                                                          | 210 ms: 1.47x faster                                                            |
| coroutines                 | 20.9 ms                                                         | 14.5 ms: 1.44x faster                                                           |
| nbody                      | 127 ms                                                          | 88.5 ms: 1.44x faster                                                           |
| richards                   | 41.3 ms                                                         | 28.9 ms: 1.43x faster                                                           |
| richards_super             | 46.5 ms                                                         | 33.0 ms: 1.41x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 150 us: 1.40x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.34 us: 1.38x faster                                                           |
| comprehensions             | 19.2 us                                                         | 14.0 us: 1.37x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 208 us: 1.37x faster                                                            |
| sqlglot_parse              | 1.25 ms                                                         | 910 us: 1.37x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 93.5 us: 1.35x faster                                                           |
| deepcopy                   | 360 us                                                          | 268 us: 1.34x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.79 ms: 1.34x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.15 ms: 1.33x faster                                                           |
| chaos                      | 69.4 ms                                                         | 53.0 ms: 1.31x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.68 sec: 1.31x faster                                                          |
| go                         | 137 ms                                                          | 106 ms: 1.29x faster                                                            |
| float                      | 76.7 ms                                                         | 59.3 ms: 1.29x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.80 ms: 1.28x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 42.2 ms: 1.26x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 5.41 ms: 1.26x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 52.7 ms: 1.26x faster                                                           |
| mako                       | 9.96 ms                                                         | 8.03 ms: 1.24x faster                                                           |
| pyflate                    | 424 ms                                                          | 342 ms: 1.24x faster                                                            |
| spectral_norm              | 104 ms                                                          | 84.6 ms: 1.23x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.22 sec: 1.23x faster                                                          |
| regex_compile              | 129 ms                                                          | 107 ms: 1.21x faster                                                            |
| logging_simple             | 9.75 us                                                         | 8.08 us: 1.21x faster                                                           |
| scimark_fft                | 271 ms                                                          | 225 ms: 1.21x faster                                                            |
| pprint_safe_repr           | 721 ms                                                          | 598 ms: 1.20x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 57.7 ms: 1.20x faster                                                           |
| logging_format             | 10.4 us                                                         | 8.77 us: 1.19x faster                                                           |
| sqlglot_optimize           | 48.5 ms                                                         | 41.1 ms: 1.18x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 79.8 ms: 1.17x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 61.7 ms: 1.17x faster                                                           |
| mdp                        | 1.91 sec                                                        | 1.64 sec: 1.17x faster                                                          |
| pycparser                  | 978 ms                                                          | 839 ms: 1.17x faster                                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.35 ms: 1.15x faster                                                           |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                                            |
| async_generators           | 313 ms                                                          | 273 ms: 1.15x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.4 ms: 1.14x faster                                                           |
| async_tree_none            | 298 ms                                                          | 261 ms: 1.14x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 6.51 ms: 1.14x faster                                                           |
| 2to3                       | 280 ms                                                          | 246 ms: 1.14x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 108 ms: 1.13x faster                                                            |
| sympy_str                  | 240 ms                                                          | 211 ms: 1.13x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 310 ms: 1.13x faster                                                            |
| fannkuch                   | 354 ms                                                          | 314 ms: 1.13x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 603 ms: 1.12x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 1.85 us: 1.12x faster                                                           |
| async_tree_memoization     | 364 ms                                                          | 328 ms: 1.11x faster                                                            |
| async_tree_io              | 693 ms                                                          | 628 ms: 1.10x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 511 ms: 1.10x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 71.1 ms: 1.09x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 80.1 ms: 1.08x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 504 ms: 1.08x faster                                                            |
| sympy_expand               | 398 ms                                                          | 367 ms: 1.08x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.84 sec: 1.08x faster                                                          |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| regex_dna                  | 127 ms                                                          | 119 ms: 1.07x faster                                                            |
| tornado_http               | 105 ms                                                          | 99.1 ms: 1.06x faster                                                           |
| json                       | 4.15 ms                                                         | 3.98 ms: 1.04x faster                                                           |
| dask                       | 323 ms                                                          | 311 ms: 1.04x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.06 ms: 1.04x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 73.0 ms: 1.03x faster                                                           |
| json_loads                 | 20.4 us                                                         | 19.7 us: 1.03x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 89.2 ms: 1.02x faster                                                           |
| unpickle                   | 9.71 us                                                         | 9.57 us: 1.01x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.42 ms: 1.01x faster                                                           |
| pickle                     | 7.79 us                                                         | 7.74 us: 1.01x faster                                                           |
| pickle_dict                | 19.9 us                                                         | 19.8 us: 1.01x faster                                                           |
| python_startup             | 22.4 ms                                                         | 23.2 ms: 1.04x slower                                                           |
| unpickle_list              | 2.95 us                                                         | 3.07 us: 1.04x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.07x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.7 ms: 1.08x slower                                                           |
| pickle_list                | 3.37 us                                                         | 3.74 us: 1.11x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.23 ms: 1.13x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 211 ms: 2.11x slower                                                            |
| coverage                   | 48.4 ms                                                         | 477 ms: 9.84x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (5): asyncio_tcp_ssl, xml_etree_parse, pidigits, create_gc_cycles, asyncio_tcp
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown