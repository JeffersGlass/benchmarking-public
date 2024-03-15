
# Results vs. 3.12.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 232 ms: 1.21x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.76 ms: 1.35x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.71 sec: 1.16x faster                                                          |
| tornado_http   | 105 ms                                                          | 93.8 ms: 1.12x faster                                                           |
| Geometric mean | (ref)                                                           | 1.20x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 244 ms: 1.22x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 290 ms: 1.21x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 303 ms: 1.20x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 232 ms: 1.20x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 571 ms: 1.19x faster                                                            |
| async_tree_io              | 693 ms                                                          | 587 ms: 1.18x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 499 ms: 1.13x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 493 ms: 1.11x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.18x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 78.1 ms: 1.63x faster                                                           |
| float          | 76.7 ms                                                         | 54.4 ms: 1.41x faster                                                           |
| pidigits       | 199 ms                                                          | 197 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.32x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 96.1 ms: 1.34x faster                                                           |
| regex_effbot   | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                           |
| regex_dna      | 127 ms                                                          | 119 ms: 1.07x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 15.7 ms: 1.05x slower                                                           |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 141 us: 1.49x faster                                                            |
| pickle_pure_python   | 286 us                                                          | 206 us: 1.39x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.59 sec: 1.38x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 40.9 ms: 1.30x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 59.3 ms: 1.22x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 64.6 ms: 1.20x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.69 ms: 1.11x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.23 us: 1.04x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| json_loads           | 20.4 us                                                         | 19.8 us: 1.03x faster                                                           |
| unpickle_list        | 2.95 us                                                         | 2.88 us: 1.02x faster                                                           |
| unpickle             | 9.71 us                                                         | 9.91 us: 1.02x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.15x faster                                                                    |

Benchmark hidden because not significant (2): pickle_dict, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.7 ms: 1.01x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.4 ms: 1.07x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.04x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 6.86 ms: 1.45x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 57.3 ns: 1.76x faster                                                           |
| generators                 | 38.5 ms                                                         | 22.5 ms: 1.71x faster                                                           |
| comprehensions             | 19.2 us                                                         | 11.4 us: 1.69x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.15 ms: 1.67x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 37.5 ns: 1.67x faster                                                           |
| raytrace                   | 308 ms                                                          | 189 ms: 1.63x faster                                                            |
| deepcopy_memo              | 38.4 us                                                         | 23.6 us: 1.63x faster                                                           |
| nbody                      | 127 ms                                                          | 78.1 ms: 1.63x faster                                                           |
| spectral_norm              | 104 ms                                                          | 64.4 ms: 1.61x faster                                                           |
| hexiom                     | 6.82 ms                                                         | 4.25 ms: 1.60x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 59.2 ms: 1.57x faster                                                           |
| scimark_sor                | 130 ms                                                          | 84.1 ms: 1.54x faster                                                           |
| chaos                      | 69.4 ms                                                         | 46.3 ms: 1.50x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 141 us: 1.49x faster                                                            |
| scimark_monte_carlo        | 66.4 ms                                                         | 45.1 ms: 1.47x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 853 us: 1.46x faster                                                            |
| coroutines                 | 20.9 ms                                                         | 14.4 ms: 1.45x faster                                                           |
| mako                       | 9.96 ms                                                         | 6.86 ms: 1.45x faster                                                           |
| richards                   | 41.3 ms                                                         | 28.9 ms: 1.43x faster                                                           |
| typing_runtime_protocols   | 126 us                                                          | 88.6 us: 1.43x faster                                                           |
| go                         | 137 ms                                                          | 96.7 ms: 1.42x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.08 ms: 1.41x faster                                                           |
| richards_super             | 46.5 ms                                                         | 32.9 ms: 1.41x faster                                                           |
| float                      | 76.7 ms                                                         | 54.4 ms: 1.41x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 206 us: 1.39x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.59 sec: 1.38x faster                                                          |
| pyflate                    | 424 ms                                                          | 309 ms: 1.37x faster                                                            |
| nqueens                    | 93.7 ms                                                         | 69.5 ms: 1.35x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 5.76 ms: 1.35x faster                                                           |
| regex_compile              | 129 ms                                                          | 96.1 ms: 1.34x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.40 us: 1.34x faster                                                           |
| deepcopy                   | 360 us                                                          | 271 us: 1.33x faster                                                            |
| scimark_fft                | 271 ms                                                          | 206 ms: 1.32x faster                                                            |
| fannkuch                   | 354 ms                                                          | 269 ms: 1.32x faster                                                            |
| crypto_pyaes               | 69.2 ms                                                         | 52.9 ms: 1.31x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 40.9 ms: 1.30x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 2.98 ms: 1.30x faster                                                           |
| sqlglot_optimize           | 48.5 ms                                                         | 38.2 ms: 1.27x faster                                                           |
| logging_simple             | 9.75 us                                                         | 7.79 us: 1.25x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.20 sec: 1.25x faster                                                          |
| logging_format             | 10.4 us                                                         | 8.36 us: 1.25x faster                                                           |
| pycparser                  | 978 ms                                                          | 794 ms: 1.23x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 14.3 ms: 1.23x faster                                                           |
| sympy_sum                  | 123 ms                                                          | 100 ms: 1.23x faster                                                            |
| async_tree_none            | 298 ms                                                          | 244 ms: 1.22x faster                                                            |
| pprint_safe_repr           | 721 ms                                                          | 591 ms: 1.22x faster                                                            |
| xml_etree_generate         | 72.1 ms                                                         | 59.3 ms: 1.22x faster                                                           |
| sympy_str                  | 240 ms                                                          | 197 ms: 1.22x faster                                                            |
| 2to3                       | 280 ms                                                          | 232 ms: 1.21x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 290 ms: 1.21x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 64.6 ms: 1.20x faster                                                           |
| async_tree_memoization     | 364 ms                                                          | 303 ms: 1.20x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 232 ms: 1.20x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.60 sec: 1.19x faster                                                          |
| async_tree_io_tg           | 677 ms                                                          | 571 ms: 1.19x faster                                                            |
| async_tree_io              | 693 ms                                                          | 587 ms: 1.18x faster                                                            |
| sympy_expand               | 398 ms                                                          | 343 ms: 1.16x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.71 sec: 1.16x faster                                                          |
| meteor_contest             | 86.9 ms                                                         | 75.8 ms: 1.15x faster                                                           |
| async_generators           | 313 ms                                                          | 277 ms: 1.13x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 499 ms: 1.13x faster                                                            |
| tornado_http               | 105 ms                                                          | 93.8 ms: 1.12x faster                                                           |
| bench_thread_pool          | 1.10 ms                                                         | 991 us: 1.11x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 493 ms: 1.11x faster                                                            |
| json_dumps                 | 7.40 ms                                                         | 6.69 ms: 1.11x faster                                                           |
| pathlib                    | 91.4 ms                                                         | 85.1 ms: 1.07x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.90 ms: 1.07x faster                                                           |
| regex_dna                  | 127 ms                                                          | 119 ms: 1.07x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 1.96 us: 1.06x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                          |
| bench_mp_pool              | 75.4 ms                                                         | 71.8 ms: 1.05x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.23 us: 1.04x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.39 ms: 1.04x faster                                                           |
| json                       | 4.15 ms                                                         | 4.03 ms: 1.03x faster                                                           |
| json_loads                 | 20.4 us                                                         | 19.8 us: 1.03x faster                                                           |
| unpickle_list              | 2.95 us                                                         | 2.88 us: 1.02x faster                                                           |
| pidigits                   | 199 ms                                                          | 197 ms: 1.01x faster                                                            |
| python_startup             | 22.4 ms                                                         | 22.7 ms: 1.01x slower                                                           |
| unpickle                   | 9.71 us                                                         | 9.91 us: 1.02x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 15.7 ms: 1.05x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.84 ms: 1.06x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.4 ms: 1.07x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 196 ms: 1.95x slower                                                            |
| coverage                   | 48.4 ms                                                         | 474 ms: 9.79x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.20x faster                                                                    |

Benchmark hidden because not significant (4): asyncio_tcp, pickle_dict, create_gc_cycles, pickle
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: unknown