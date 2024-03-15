
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 250 ms: 1.12x faster                                                                      |
| chameleon      | 7.75 ms                                                         | 5.82 ms: 1.33x faster                                                                     |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                                    |
| tornado_http   | 105 ms                                                          | 98.8 ms: 1.06x faster                                                                     |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 255 ms: 1.17x faster                                                                      |
| async_tree_memoization     | 364 ms                                                          | 316 ms: 1.15x faster                                                                      |
| async_tree_memoization_tg  | 350 ms                                                          | 306 ms: 1.14x faster                                                                      |
| async_tree_io_tg           | 677 ms                                                          | 595 ms: 1.14x faster                                                                      |
| async_tree_none_tg         | 278 ms                                                          | 244 ms: 1.14x faster                                                                      |
| async_tree_io              | 693 ms                                                          | 620 ms: 1.12x faster                                                                      |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 521 ms: 1.08x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 505 ms: 1.08x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 87.0 ms: 1.46x faster                                                                     |
| float          | 76.7 ms                                                         | 61.2 ms: 1.25x faster                                                                     |
| pidigits       | 199 ms                                                          | 204 ms: 1.02x slower                                                                      |
| Geometric mean | (ref)                                                           | 1.21x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 108 ms: 1.20x faster                                                                      |
| regex_effbot   | 2.04 ms                                                         | 1.92 ms: 1.06x faster                                                                     |
| regex_dna      | 127 ms                                                          | 123 ms: 1.03x faster                                                                      |
| regex_v8       | 15.0 ms                                                         | 16.2 ms: 1.07x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 153 us: 1.37x faster                                                                      |
| pickle_pure_python   | 286 us                                                          | 209 us: 1.37x faster                                                                      |
| tomli_loads          | 2.20 sec                                                        | 1.65 sec: 1.33x faster                                                                    |
| xml_etree_process    | 53.2 ms                                                         | 42.2 ms: 1.26x faster                                                                     |
| xml_etree_generate   | 72.1 ms                                                         | 61.2 ms: 1.18x faster                                                                     |
| xml_etree_iterparse  | 77.6 ms                                                         | 70.5 ms: 1.10x faster                                                                     |
| json_dumps           | 7.40 ms                                                         | 6.87 ms: 1.08x faster                                                                     |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                                      |
| json_loads           | 20.4 us                                                         | 20.0 us: 1.02x faster                                                                     |
| pickle_dict          | 19.9 us                                                         | 20.2 us: 1.01x slower                                                                     |
| unpickle             | 9.71 us                                                         | 9.90 us: 1.02x slower                                                                     |
| unpickle_list        | 2.95 us                                                         | 3.05 us: 1.04x slower                                                                     |
| pickle_list          | 3.37 us                                                         | 3.69 us: 1.10x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                                              |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.8 ms: 1.06x slower                                                                     |
| python_startup_no_site | 19.1 ms                                                         | 21.5 ms: 1.13x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.10x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 8.34 ms: 1.19x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 60.2 ns: 1.68x faster                                                                     |
| generators                 | 38.5 ms                                                         | 23.2 ms: 1.66x faster                                                                     |
| scimark_sor                | 130 ms                                                          | 82.3 ms: 1.58x faster                                                                     |
| deepcopy_memo              | 38.4 us                                                         | 24.6 us: 1.56x faster                                                                     |
| unpack_sequence            | 62.5 ns                                                         | 41.4 ns: 1.51x faster                                                                     |
| scimark_lu                 | 93.2 ms                                                         | 62.6 ms: 1.49x faster                                                                     |
| raytrace                   | 308 ms                                                          | 209 ms: 1.47x faster                                                                      |
| coroutines                 | 20.9 ms                                                         | 14.2 ms: 1.47x faster                                                                     |
| nbody                      | 127 ms                                                          | 87.0 ms: 1.46x faster                                                                     |
| sqlglot_parse              | 1.25 ms                                                         | 883 us: 1.41x faster                                                                      |
| richards_super             | 46.5 ms                                                         | 33.1 ms: 1.41x faster                                                                     |
| richards                   | 41.3 ms                                                         | 29.4 ms: 1.40x faster                                                                     |
| comprehensions             | 19.2 us                                                         | 14.0 us: 1.37x faster                                                                     |
| unpickle_pure_python       | 210 us                                                          | 153 us: 1.37x faster                                                                      |
| pickle_pure_python         | 286 us                                                          | 209 us: 1.37x faster                                                                      |
| sqlglot_transpile          | 1.53 ms                                                         | 1.13 ms: 1.36x faster                                                                     |
| deepcopy_reduce            | 3.23 us                                                         | 2.39 us: 1.35x faster                                                                     |
| chameleon                  | 7.75 ms                                                         | 5.82 ms: 1.33x faster                                                                     |
| chaos                      | 69.4 ms                                                         | 52.1 ms: 1.33x faster                                                                     |
| tomli_loads                | 2.20 sec                                                        | 1.65 sec: 1.33x faster                                                                    |
| typing_runtime_protocols   | 126 us                                                          | 95.4 us: 1.32x faster                                                                     |
| deepcopy                   | 360 us                                                          | 275 us: 1.31x faster                                                                      |
| go                         | 137 ms                                                          | 106 ms: 1.30x faster                                                                      |
| scimark_monte_carlo        | 66.4 ms                                                         | 52.2 ms: 1.27x faster                                                                     |
| xml_etree_process          | 53.2 ms                                                         | 42.2 ms: 1.26x faster                                                                     |
| float                      | 76.7 ms                                                         | 61.2 ms: 1.25x faster                                                                     |
| scimark_fft                | 271 ms                                                          | 217 ms: 1.25x faster                                                                      |
| hexiom                     | 6.82 ms                                                         | 5.47 ms: 1.25x faster                                                                     |
| pyflate                    | 424 ms                                                          | 341 ms: 1.24x faster                                                                      |
| deltablue                  | 3.58 ms                                                         | 2.89 ms: 1.24x faster                                                                     |
| fannkuch                   | 354 ms                                                          | 288 ms: 1.23x faster                                                                      |
| spectral_norm              | 104 ms                                                          | 85.0 ms: 1.22x faster                                                                     |
| crypto_pyaes               | 69.2 ms                                                         | 56.7 ms: 1.22x faster                                                                     |
| nqueens                    | 93.7 ms                                                         | 77.5 ms: 1.21x faster                                                                     |
| regex_compile              | 129 ms                                                          | 108 ms: 1.20x faster                                                                      |
| mako                       | 9.96 ms                                                         | 8.34 ms: 1.19x faster                                                                     |
| logging_format             | 10.4 us                                                         | 8.72 us: 1.19x faster                                                                     |
| pprint_pformat             | 1.50 sec                                                        | 1.26 sec: 1.19x faster                                                                    |
| xml_etree_generate         | 72.1 ms                                                         | 61.2 ms: 1.18x faster                                                                     |
| logging_simple             | 9.75 us                                                         | 8.28 us: 1.18x faster                                                                     |
| pycparser                  | 978 ms                                                          | 832 ms: 1.18x faster                                                                      |
| async_tree_none            | 298 ms                                                          | 255 ms: 1.17x faster                                                                      |
| sqlglot_optimize           | 48.5 ms                                                         | 41.7 ms: 1.16x faster                                                                     |
| mdp                        | 1.91 sec                                                        | 1.65 sec: 1.16x faster                                                                    |
| pprint_safe_repr           | 721 ms                                                          | 622 ms: 1.16x faster                                                                      |
| async_tree_memoization     | 364 ms                                                          | 316 ms: 1.15x faster                                                                      |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.37 ms: 1.15x faster                                                                     |
| async_tree_memoization_tg  | 350 ms                                                          | 306 ms: 1.14x faster                                                                      |
| async_generators           | 313 ms                                                          | 275 ms: 1.14x faster                                                                      |
| async_tree_io_tg           | 677 ms                                                          | 595 ms: 1.14x faster                                                                      |
| sympy_integrate            | 17.5 ms                                                         | 15.4 ms: 1.14x faster                                                                     |
| async_tree_none_tg         | 278 ms                                                          | 244 ms: 1.14x faster                                                                      |
| 2to3                       | 280 ms                                                          | 250 ms: 1.12x faster                                                                      |
| sympy_str                  | 240 ms                                                          | 214 ms: 1.12x faster                                                                      |
| async_tree_io              | 693 ms                                                          | 620 ms: 1.12x faster                                                                      |
| sympy_sum                  | 123 ms                                                          | 110 ms: 1.12x faster                                                                      |
| xml_etree_iterparse        | 77.6 ms                                                         | 70.5 ms: 1.10x faster                                                                     |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                                                    |
| sqlite_synth               | 2.07 us                                                         | 1.90 us: 1.09x faster                                                                     |
| meteor_contest             | 86.9 ms                                                         | 80.0 ms: 1.09x faster                                                                     |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 521 ms: 1.08x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 505 ms: 1.08x faster                                                                      |
| sympy_expand               | 398 ms                                                          | 369 ms: 1.08x faster                                                                      |
| json_dumps                 | 7.40 ms                                                         | 6.87 ms: 1.08x faster                                                                     |
| tornado_http               | 105 ms                                                          | 98.8 ms: 1.06x faster                                                                     |
| regex_effbot               | 2.04 ms                                                         | 1.92 ms: 1.06x faster                                                                     |
| dask                       | 323 ms                                                          | 308 ms: 1.05x faster                                                                      |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                                      |
| regex_dna                  | 127 ms                                                          | 123 ms: 1.03x faster                                                                      |
| gc_traversal               | 1.44 ms                                                         | 1.40 ms: 1.03x faster                                                                     |
| bench_thread_pool          | 1.10 ms                                                         | 1.08 ms: 1.02x faster                                                                     |
| pathlib                    | 91.4 ms                                                         | 89.5 ms: 1.02x faster                                                                     |
| json_loads                 | 20.4 us                                                         | 20.0 us: 1.02x faster                                                                     |
| json                       | 4.15 ms                                                         | 4.10 ms: 1.01x faster                                                                     |
| bench_mp_pool              | 75.4 ms                                                         | 74.6 ms: 1.01x faster                                                                     |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 17.5 sec: 1.01x faster                                                                    |
| pickle_dict                | 19.9 us                                                         | 20.2 us: 1.01x slower                                                                     |
| unpickle                   | 9.71 us                                                         | 9.90 us: 1.02x slower                                                                     |
| pidigits                   | 199 ms                                                          | 204 ms: 1.02x slower                                                                      |
| create_gc_cycles           | 652 us                                                          | 671 us: 1.03x slower                                                                      |
| unpickle_list              | 2.95 us                                                         | 3.05 us: 1.04x slower                                                                     |
| telco                      | 5.51 ms                                                         | 5.75 ms: 1.04x slower                                                                     |
| python_startup             | 22.4 ms                                                         | 23.8 ms: 1.06x slower                                                                     |
| regex_v8                   | 15.0 ms                                                         | 16.2 ms: 1.07x slower                                                                     |
| pickle_list                | 3.37 us                                                         | 3.69 us: 1.10x slower                                                                     |
| python_startup_no_site     | 19.1 ms                                                         | 21.5 ms: 1.13x slower                                                                     |
| sqlglot_normalize          | 100 ms                                                          | 213 ms: 2.12x slower                                                                      |
| coverage                   | 48.4 ms                                                         | 505 ms: 10.43x slower                                                                     |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                              |

Benchmark hidden because not significant (2): pickle, asyncio_tcp
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown