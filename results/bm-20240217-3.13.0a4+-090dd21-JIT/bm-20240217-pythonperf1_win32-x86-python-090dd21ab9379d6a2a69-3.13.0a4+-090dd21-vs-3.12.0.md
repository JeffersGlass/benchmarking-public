
# Results vs. 3.12.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.11x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 252 ms: 1.11x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.98 ms: 1.30x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                          |
| tornado_http   | 105 ms                                                          | 98.6 ms: 1.06x faster                                                           |
| Geometric mean | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 350 ms                                                          | 305 ms: 1.15x faster                                                            |
| async_tree_none            | 298 ms                                                          | 259 ms: 1.15x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 242 ms: 1.15x faster                                                            |
| async_tree_io              | 693 ms                                                          | 620 ms: 1.12x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 608 ms: 1.11x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 327 ms: 1.11x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 512 ms: 1.10x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 501 ms: 1.09x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.12x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 53.8 ms: 1.43x faster                                                           |
| nbody          | 127 ms                                                          | 94.2 ms: 1.35x faster                                                           |
| pidigits       | 199 ms                                                          | 201 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 108 ms: 1.20x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.87 ms: 1.09x faster                                                           |
| regex_dna      | 127 ms                                                          | 120 ms: 1.06x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 15.7 ms: 1.04x slower                                                           |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 158 us: 1.33x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.66 sec: 1.32x faster                                                          |
| pickle_pure_python   | 286 us                                                          | 219 us: 1.31x faster                                                            |
| xml_etree_process    | 53.2 ms                                                         | 42.6 ms: 1.25x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 60.8 ms: 1.19x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 65.7 ms: 1.18x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.88 ms: 1.08x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 108 ms: 1.05x faster                                                            |
| json_loads           | 20.4 us                                                         | 19.8 us: 1.03x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.28 us: 1.03x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| pickle               | 7.79 us                                                         | 8.09 us: 1.04x slower                                                           |
| unpickle             | 9.71 us                                                         | 10.3 us: 1.06x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.0 ms: 1.03x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.8 ms: 1.09x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.31 ms: 1.36x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 24.5 ms: 1.57x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 25.3 us: 1.52x faster                                                           |
| logging_silent             | 101 ns                                                          | 67.7 ns: 1.49x faster                                                           |
| scimark_sor                | 130 ms                                                          | 88.3 ms: 1.47x faster                                                           |
| spectral_norm              | 104 ms                                                          | 71.2 ms: 1.46x faster                                                           |
| float                      | 76.7 ms                                                         | 53.8 ms: 1.43x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 44.1 ns: 1.41x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.57 ms: 1.39x faster                                                           |
| comprehensions             | 19.2 us                                                         | 13.9 us: 1.38x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 15.1 ms: 1.38x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 68.4 ms: 1.36x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.31 ms: 1.36x faster                                                           |
| nbody                      | 127 ms                                                          | 94.2 ms: 1.35x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 158 us: 1.33x faster                                                            |
| richards_super             | 46.5 ms                                                         | 35.1 ms: 1.32x faster                                                           |
| tomli_loads                | 2.20 sec                                                        | 1.66 sec: 1.32x faster                                                          |
| richards                   | 41.3 ms                                                         | 31.5 ms: 1.31x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 219 us: 1.31x faster                                                            |
| sqlglot_parse              | 1.25 ms                                                         | 957 us: 1.30x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 97.1 us: 1.30x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 5.98 ms: 1.30x faster                                                           |
| raytrace                   | 308 ms                                                          | 238 ms: 1.30x faster                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.21 ms: 1.27x faster                                                           |
| deepcopy                   | 360 us                                                          | 285 us: 1.26x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.55 us: 1.26x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 42.6 ms: 1.25x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.11 ms: 1.24x faster                                                           |
| regex_compile              | 129 ms                                                          | 108 ms: 1.20x faster                                                            |
| xml_etree_generate         | 72.1 ms                                                         | 60.8 ms: 1.19x faster                                                           |
| xml_etree_iterparse        | 77.6 ms                                                         | 65.7 ms: 1.18x faster                                                           |
| chaos                      | 69.4 ms                                                         | 59.0 ms: 1.18x faster                                                           |
| logging_simple             | 9.75 us                                                         | 8.30 us: 1.18x faster                                                           |
| fannkuch                   | 354 ms                                                          | 303 ms: 1.17x faster                                                            |
| logging_format             | 10.4 us                                                         | 9.00 us: 1.16x faster                                                           |
| scimark_fft                | 271 ms                                                          | 235 ms: 1.15x faster                                                            |
| go                         | 137 ms                                                          | 119 ms: 1.15x faster                                                            |
| pyflate                    | 424 ms                                                          | 369 ms: 1.15x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 305 ms: 1.15x faster                                                            |
| async_tree_none            | 298 ms                                                          | 259 ms: 1.15x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 242 ms: 1.15x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 60.7 ms: 1.14x faster                                                           |
| sqlglot_optimize           | 48.5 ms                                                         | 43.2 ms: 1.12x faster                                                           |
| async_tree_io              | 693 ms                                                          | 620 ms: 1.12x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 110 ms: 1.12x faster                                                            |
| pycparser                  | 978 ms                                                          | 876 ms: 1.12x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.7 ms: 1.12x faster                                                           |
| async_tree_io_tg           | 677 ms                                                          | 608 ms: 1.11x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 327 ms: 1.11x faster                                                            |
| sympy_str                  | 240 ms                                                          | 216 ms: 1.11x faster                                                            |
| 2to3                       | 280 ms                                                          | 252 ms: 1.11x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 1.87 us: 1.11x faster                                                           |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 512 ms: 1.10x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 501 ms: 1.09x faster                                                            |
| regex_effbot               | 2.04 ms                                                         | 1.87 ms: 1.09x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 84.1 ms: 1.09x faster                                                           |
| async_generators           | 313 ms                                                          | 289 ms: 1.08x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 6.88 ms: 1.08x faster                                                           |
| bench_thread_pool          | 1.10 ms                                                         | 1.03 ms: 1.07x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 87.7 ms: 1.07x faster                                                           |
| tornado_http               | 105 ms                                                          | 98.6 ms: 1.06x faster                                                           |
| regex_dna                  | 127 ms                                                          | 120 ms: 1.06x faster                                                            |
| sympy_expand               | 398 ms                                                          | 376 ms: 1.06x faster                                                            |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.7 sec: 1.06x faster                                                          |
| hexiom                     | 6.82 ms                                                         | 6.47 ms: 1.05x faster                                                           |
| dask                       | 323 ms                                                          | 307 ms: 1.05x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.37 ms: 1.05x faster                                                           |
| asyncio_tcp                | 662 ms                                                          | 632 ms: 1.05x faster                                                            |
| xml_etree_parse            | 113 ms                                                          | 108 ms: 1.05x faster                                                            |
| meteor_contest             | 86.9 ms                                                         | 83.5 ms: 1.04x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.44 sec: 1.04x faster                                                          |
| mdp                        | 1.91 sec                                                        | 1.84 sec: 1.04x faster                                                          |
| json_loads                 | 20.4 us                                                         | 19.8 us: 1.03x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.28 us: 1.03x faster                                                           |
| pprint_safe_repr           | 721 ms                                                          | 702 ms: 1.03x faster                                                            |
| bench_mp_pool              | 75.4 ms                                                         | 74.7 ms: 1.01x faster                                                           |
| pidigits                   | 199 ms                                                          | 201 ms: 1.01x slower                                                            |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| python_startup             | 22.4 ms                                                         | 23.0 ms: 1.03x slower                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 68.7 ms: 1.03x slower                                                           |
| pickle                     | 7.79 us                                                         | 8.09 us: 1.04x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 15.7 ms: 1.04x slower                                                           |
| unpickle                   | 9.71 us                                                         | 10.3 us: 1.06x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.98 ms: 1.09x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.8 ms: 1.09x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 218 ms: 2.18x slower                                                            |
| coverage                   | 48.4 ms                                                         | 466 ms: 9.62x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (3): create_gc_cycles, json, unpickle_list
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown