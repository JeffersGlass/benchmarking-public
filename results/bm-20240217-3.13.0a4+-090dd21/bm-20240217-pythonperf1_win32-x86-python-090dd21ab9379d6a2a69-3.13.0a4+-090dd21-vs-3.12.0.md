
# Results vs. 3.12.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 229 ms: 1.22x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.63 ms: 1.38x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.69 sec: 1.17x faster                                                          |
| tornado_http   | 105 ms                                                          | 93.9 ms: 1.12x faster                                                           |
| Geometric mean | (ref)                                                           | 1.22x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 241 ms: 1.23x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 228 ms: 1.22x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 288 ms: 1.22x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 300 ms: 1.21x faster                                                            |
| async_tree_io              | 693 ms                                                          | 582 ms: 1.19x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 570 ms: 1.19x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 486 ms: 1.16x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 477 ms: 1.15x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.20x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 76.1 ms: 1.67x faster                                                           |
| float          | 76.7 ms                                                         | 54.9 ms: 1.40x faster                                                           |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.33x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 94.6 ms: 1.36x faster                                                           |
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| regex_dna      | 127 ms                                                          | 120 ms: 1.06x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 15.9 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 143 us: 1.47x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 205 us: 1.40x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.62 sec: 1.35x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 40.2 ms: 1.32x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 57.6 ms: 1.25x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 64.8 ms: 1.20x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.45 ms: 1.15x faster                                                           |
| unpickle_list        | 2.95 us                                                         | 2.78 us: 1.06x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 108 ms: 1.05x faster                                                            |
| pickle_list          | 3.37 us                                                         | 3.22 us: 1.05x faster                                                           |
| json_loads           | 20.4 us                                                         | 19.6 us: 1.04x faster                                                           |
| pickle               | 7.79 us                                                         | 7.98 us: 1.02x slower                                                           |
| unpickle             | 9.71 us                                                         | 9.96 us: 1.03x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                    |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 19.1 ms                                                         | 20.2 ms: 1.06x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.03x slower                                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 6.94 ms: 1.43x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 21.7 ms: 1.77x faster                                                           |
| logging_silent             | 101 ns                                                          | 58.5 ns: 1.73x faster                                                           |
| comprehensions             | 19.2 us                                                         | 11.5 us: 1.67x faster                                                           |
| nbody                      | 127 ms                                                          | 76.1 ms: 1.67x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 23.1 us: 1.66x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.20 ms: 1.63x faster                                                           |
| raytrace                   | 308 ms                                                          | 191 ms: 1.61x faster                                                            |
| unpack_sequence            | 62.5 ns                                                         | 39.0 ns: 1.60x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 4.28 ms: 1.59x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 58.7 ms: 1.59x faster                                                           |
| spectral_norm              | 104 ms                                                          | 65.4 ms: 1.59x faster                                                           |
| scimark_sor                | 130 ms                                                          | 83.8 ms: 1.55x faster                                                           |
| chaos                      | 69.4 ms                                                         | 47.2 ms: 1.47x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 143 us: 1.47x faster                                                            |
| coroutines                 | 20.9 ms                                                         | 14.4 ms: 1.45x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 45.8 ms: 1.45x faster                                                           |
| richards                   | 41.3 ms                                                         | 28.6 ms: 1.45x faster                                                           |
| go                         | 137 ms                                                          | 95.3 ms: 1.44x faster                                                           |
| mako                       | 9.96 ms                                                         | 6.94 ms: 1.43x faster                                                           |
| typing_runtime_protocols   | 126 us                                                          | 88.7 us: 1.42x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 876 us: 1.42x faster                                                            |
| pickle_pure_python         | 286 us                                                          | 205 us: 1.40x faster                                                            |
| float                      | 76.7 ms                                                         | 54.9 ms: 1.40x faster                                                           |
| richards_super             | 46.5 ms                                                         | 33.4 ms: 1.39x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.11 ms: 1.38x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 5.63 ms: 1.38x faster                                                           |
| scimark_fft                | 271 ms                                                          | 197 ms: 1.37x faster                                                            |
| pyflate                    | 424 ms                                                          | 309 ms: 1.37x faster                                                            |
| deepcopy                   | 360 us                                                          | 263 us: 1.37x faster                                                            |
| regex_compile              | 129 ms                                                          | 94.6 ms: 1.36x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.37 us: 1.36x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.62 sec: 1.35x faster                                                          |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 2.87 ms: 1.34x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 52.2 ms: 1.33x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 40.2 ms: 1.32x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 71.7 ms: 1.31x faster                                                           |
| logging_simple             | 9.75 us                                                         | 7.48 us: 1.30x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.15 sec: 1.30x faster                                                          |
| logging_format             | 10.4 us                                                         | 8.10 us: 1.29x faster                                                           |
| fannkuch                   | 354 ms                                                          | 276 ms: 1.28x faster                                                            |
| pprint_safe_repr           | 721 ms                                                          | 565 ms: 1.28x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 38.1 ms: 1.27x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 57.6 ms: 1.25x faster                                                           |
| sympy_integrate            | 17.5 ms                                                         | 14.2 ms: 1.24x faster                                                           |
| async_tree_none            | 298 ms                                                          | 241 ms: 1.23x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 100 ms: 1.23x faster                                                            |
| sympy_str                  | 240 ms                                                          | 196 ms: 1.22x faster                                                            |
| 2to3                       | 280 ms                                                          | 229 ms: 1.22x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 228 ms: 1.22x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 288 ms: 1.22x faster                                                            |
| pycparser                  | 978 ms                                                          | 805 ms: 1.21x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 300 ms: 1.21x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 64.8 ms: 1.20x faster                                                           |
| async_tree_io              | 693 ms                                                          | 582 ms: 1.19x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 570 ms: 1.19x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.69 sec: 1.17x faster                                                          |
| async_generators           | 313 ms                                                          | 267 ms: 1.17x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 486 ms: 1.16x faster                                                            |
| sympy_expand               | 398 ms                                                          | 343 ms: 1.16x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.65 sec: 1.16x faster                                                          |
| meteor_contest             | 86.9 ms                                                         | 75.6 ms: 1.15x faster                                                           |
| json_dumps                 | 7.40 ms                                                         | 6.45 ms: 1.15x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 477 ms: 1.15x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 982 us: 1.12x faster                                                            |
| tornado_http               | 105 ms                                                          | 93.9 ms: 1.12x faster                                                           |
| dask                       | 323 ms                                                          | 291 ms: 1.11x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 1.87 us: 1.11x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 84.0 ms: 1.09x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| regex_dna                  | 127 ms                                                          | 120 ms: 1.06x faster                                                            |
| unpickle_list              | 2.95 us                                                         | 2.78 us: 1.06x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 71.5 ms: 1.06x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                          |
| xml_etree_parse            | 113 ms                                                          | 108 ms: 1.05x faster                                                            |
| pickle_list                | 3.37 us                                                         | 3.22 us: 1.05x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.38 ms: 1.04x faster                                                           |
| json_loads                 | 20.4 us                                                         | 19.6 us: 1.04x faster                                                           |
| asyncio_tcp                | 662 ms                                                          | 639 ms: 1.04x faster                                                            |
| create_gc_cycles           | 652 us                                                          | 641 us: 1.02x faster                                                            |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| pickle                     | 7.79 us                                                         | 7.98 us: 1.02x slower                                                           |
| unpickle                   | 9.71 us                                                         | 9.96 us: 1.03x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 15.9 ms: 1.06x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.84 ms: 1.06x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.2 ms: 1.06x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 194 ms: 1.93x slower                                                            |
| coverage                   | 48.4 ms                                                         | 463 ms: 9.57x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.21x faster                                                                    |

Benchmark hidden because not significant (3): json, pickle_dict, python_startup
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: unknown