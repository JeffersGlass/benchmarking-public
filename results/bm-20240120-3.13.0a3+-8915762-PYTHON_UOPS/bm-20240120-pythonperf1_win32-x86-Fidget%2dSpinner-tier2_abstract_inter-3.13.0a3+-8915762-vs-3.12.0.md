
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: 8915762
- commit date: 2024-01-20
- overall geometric mean: 1.15x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 252 ms: 1.11x faster                                                                      |
| chameleon      | 7.75 ms                                                         | 5.67 ms: 1.37x faster                                                                     |
| docutils       | 1.98 sec                                                        | 1.83 sec: 1.08x faster                                                                    |
| tornado_http   | 105 ms                                                          | 101 ms: 1.04x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 249 ms: 1.20x faster                                                                      |
| async_tree_memoization_tg  | 350 ms                                                          | 296 ms: 1.18x faster                                                                      |
| async_tree_none_tg         | 278 ms                                                          | 235 ms: 1.18x faster                                                                      |
| async_tree_memoization     | 364 ms                                                          | 310 ms: 1.17x faster                                                                      |
| async_tree_io_tg           | 677 ms                                                          | 582 ms: 1.16x faster                                                                      |
| async_tree_io              | 693 ms                                                          | 600 ms: 1.15x faster                                                                      |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 505 ms: 1.12x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 493 ms: 1.11x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.16x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 85.9 ms: 1.48x faster                                                                     |
| float          | 76.7 ms                                                         | 56.2 ms: 1.36x faster                                                                     |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.27x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 107 ms: 1.21x faster                                                                      |
| regex_dna      | 127 ms                                                          | 117 ms: 1.09x faster                                                                      |
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                                     |
| regex_v8       | 15.0 ms                                                         | 16.0 ms: 1.06x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.08x faster                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 149 us: 1.41x faster                                                                      |
| pickle_pure_python   | 286 us                                                          | 209 us: 1.37x faster                                                                      |
| tomli_loads          | 2.20 sec                                                        | 1.62 sec: 1.35x faster                                                                    |
| xml_etree_process    | 53.2 ms                                                         | 41.9 ms: 1.27x faster                                                                     |
| xml_etree_generate   | 72.1 ms                                                         | 59.8 ms: 1.21x faster                                                                     |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.1 ms: 1.14x faster                                                                     |
| json_dumps           | 7.40 ms                                                         | 6.64 ms: 1.11x faster                                                                     |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                                      |
| unpickle_list        | 2.95 us                                                         | 2.83 us: 1.04x faster                                                                     |
| pickle_list          | 3.37 us                                                         | 3.25 us: 1.04x faster                                                                     |
| json_loads           | 20.4 us                                                         | 19.9 us: 1.02x faster                                                                     |
| unpickle             | 9.71 us                                                         | 9.55 us: 1.02x faster                                                                     |
| pickle_dict          | 19.9 us                                                         | 20.2 us: 1.01x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                              |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.7 ms: 1.01x slower                                                                     |
| python_startup_no_site | 19.1 ms                                                         | 20.6 ms: 1.08x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.74 ms: 1.29x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 60.4 ns: 1.67x faster                                                                     |
| generators                 | 38.5 ms                                                         | 24.0 ms: 1.60x faster                                                                     |
| scimark_sor                | 130 ms                                                          | 82.1 ms: 1.58x faster                                                                     |
| deepcopy_memo              | 38.4 us                                                         | 25.1 us: 1.53x faster                                                                     |
| scimark_lu                 | 93.2 ms                                                         | 62.0 ms: 1.50x faster                                                                     |
| unpack_sequence            | 62.5 ns                                                         | 41.6 ns: 1.50x faster                                                                     |
| nbody                      | 127 ms                                                          | 85.9 ms: 1.48x faster                                                                     |
| raytrace                   | 308 ms                                                          | 211 ms: 1.46x faster                                                                      |
| coroutines                 | 20.9 ms                                                         | 14.7 ms: 1.42x faster                                                                     |
| comprehensions             | 19.2 us                                                         | 13.5 us: 1.42x faster                                                                     |
| unpickle_pure_python       | 210 us                                                          | 149 us: 1.41x faster                                                                      |
| richards                   | 41.3 ms                                                         | 29.6 ms: 1.40x faster                                                                     |
| richards_super             | 46.5 ms                                                         | 33.3 ms: 1.39x faster                                                                     |
| typing_runtime_protocols   | 126 us                                                          | 92.3 us: 1.37x faster                                                                     |
| pickle_pure_python         | 286 us                                                          | 209 us: 1.37x faster                                                                      |
| chameleon                  | 7.75 ms                                                         | 5.67 ms: 1.37x faster                                                                     |
| sqlglot_parse              | 1.25 ms                                                         | 913 us: 1.37x faster                                                                      |
| float                      | 76.7 ms                                                         | 56.2 ms: 1.36x faster                                                                     |
| tomli_loads                | 2.20 sec                                                        | 1.62 sec: 1.35x faster                                                                    |
| deltablue                  | 3.58 ms                                                         | 2.67 ms: 1.34x faster                                                                     |
| scimark_monte_carlo        | 66.4 ms                                                         | 49.6 ms: 1.34x faster                                                                     |
| chaos                      | 69.4 ms                                                         | 52.5 ms: 1.32x faster                                                                     |
| sqlglot_transpile          | 1.53 ms                                                         | 1.17 ms: 1.31x faster                                                                     |
| scimark_fft                | 271 ms                                                          | 207 ms: 1.31x faster                                                                      |
| hexiom                     | 6.82 ms                                                         | 5.21 ms: 1.31x faster                                                                     |
| go                         | 137 ms                                                          | 105 ms: 1.30x faster                                                                      |
| spectral_norm              | 104 ms                                                          | 79.8 ms: 1.30x faster                                                                     |
| deepcopy_reduce            | 3.23 us                                                         | 2.49 us: 1.30x faster                                                                     |
| deepcopy                   | 360 us                                                          | 279 us: 1.29x faster                                                                      |
| mako                       | 9.96 ms                                                         | 7.74 ms: 1.29x faster                                                                     |
| pyflate                    | 424 ms                                                          | 333 ms: 1.27x faster                                                                      |
| xml_etree_process          | 53.2 ms                                                         | 41.9 ms: 1.27x faster                                                                     |
| crypto_pyaes               | 69.2 ms                                                         | 55.7 ms: 1.24x faster                                                                     |
| fannkuch                   | 354 ms                                                          | 288 ms: 1.23x faster                                                                      |
| regex_compile              | 129 ms                                                          | 107 ms: 1.21x faster                                                                      |
| pprint_pformat             | 1.50 sec                                                        | 1.24 sec: 1.21x faster                                                                    |
| logging_simple             | 9.75 us                                                         | 8.06 us: 1.21x faster                                                                     |
| xml_etree_generate         | 72.1 ms                                                         | 59.8 ms: 1.21x faster                                                                     |
| nqueens                    | 93.7 ms                                                         | 77.8 ms: 1.20x faster                                                                     |
| pprint_safe_repr           | 721 ms                                                          | 599 ms: 1.20x faster                                                                      |
| async_tree_none            | 298 ms                                                          | 249 ms: 1.20x faster                                                                      |
| logging_format             | 10.4 us                                                         | 8.71 us: 1.19x faster                                                                     |
| async_tree_memoization_tg  | 350 ms                                                          | 296 ms: 1.18x faster                                                                      |
| async_tree_none_tg         | 278 ms                                                          | 235 ms: 1.18x faster                                                                      |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.28 ms: 1.17x faster                                                                     |
| async_tree_memoization     | 364 ms                                                          | 310 ms: 1.17x faster                                                                      |
| pycparser                  | 978 ms                                                          | 837 ms: 1.17x faster                                                                      |
| async_tree_io_tg           | 677 ms                                                          | 582 ms: 1.16x faster                                                                      |
| async_generators           | 313 ms                                                          | 270 ms: 1.16x faster                                                                      |
| sqlglot_optimize           | 48.5 ms                                                         | 41.8 ms: 1.16x faster                                                                     |
| async_tree_io              | 693 ms                                                          | 600 ms: 1.15x faster                                                                      |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.1 ms: 1.14x faster                                                                     |
| sympy_integrate            | 17.5 ms                                                         | 15.4 ms: 1.14x faster                                                                     |
| sympy_sum                  | 123 ms                                                          | 109 ms: 1.12x faster                                                                      |
| sympy_str                  | 240 ms                                                          | 213 ms: 1.12x faster                                                                      |
| mdp                        | 1.91 sec                                                        | 1.71 sec: 1.12x faster                                                                    |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 505 ms: 1.12x faster                                                                      |
| json_dumps                 | 7.40 ms                                                         | 6.64 ms: 1.11x faster                                                                     |
| 2to3                       | 280 ms                                                          | 252 ms: 1.11x faster                                                                      |
| sqlite_synth               | 2.07 us                                                         | 1.86 us: 1.11x faster                                                                     |
| meteor_contest             | 86.9 ms                                                         | 78.1 ms: 1.11x faster                                                                     |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 493 ms: 1.11x faster                                                                      |
| regex_dna                  | 127 ms                                                          | 117 ms: 1.09x faster                                                                      |
| docutils                   | 1.98 sec                                                        | 1.83 sec: 1.08x faster                                                                    |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                                     |
| bench_thread_pool          | 1.10 ms                                                         | 1.03 ms: 1.08x faster                                                                     |
| sympy_expand               | 398 ms                                                          | 376 ms: 1.06x faster                                                                      |
| dask                       | 323 ms                                                          | 307 ms: 1.05x faster                                                                      |
| asyncio_tcp                | 662 ms                                                          | 634 ms: 1.05x faster                                                                      |
| tornado_http               | 105 ms                                                          | 101 ms: 1.04x faster                                                                      |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                                      |
| unpickle_list              | 2.95 us                                                         | 2.83 us: 1.04x faster                                                                     |
| pathlib                    | 91.4 ms                                                         | 88.1 ms: 1.04x faster                                                                     |
| pickle_list                | 3.37 us                                                         | 3.25 us: 1.04x faster                                                                     |
| gc_traversal               | 1.44 ms                                                         | 1.41 ms: 1.03x faster                                                                     |
| json_loads                 | 20.4 us                                                         | 19.9 us: 1.02x faster                                                                     |
| unpickle                   | 9.71 us                                                         | 9.55 us: 1.02x faster                                                                     |
| create_gc_cycles           | 652 us                                                          | 642 us: 1.02x faster                                                                      |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 17.4 sec: 1.01x faster                                                                    |
| json                       | 4.15 ms                                                         | 4.10 ms: 1.01x faster                                                                     |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                                      |
| bench_mp_pool              | 75.4 ms                                                         | 74.9 ms: 1.01x faster                                                                     |
| pickle_dict                | 19.9 us                                                         | 20.2 us: 1.01x slower                                                                     |
| python_startup             | 22.4 ms                                                         | 22.7 ms: 1.01x slower                                                                     |
| regex_v8                   | 15.0 ms                                                         | 16.0 ms: 1.06x slower                                                                     |
| python_startup_no_site     | 19.1 ms                                                         | 20.6 ms: 1.08x slower                                                                     |
| telco                      | 5.51 ms                                                         | 6.14 ms: 1.11x slower                                                                     |
| sqlglot_normalize          | 100 ms                                                          | 216 ms: 2.16x slower                                                                      |
| coverage                   | 48.4 ms                                                         | 487 ms: 10.07x slower                                                                     |
| Geometric mean             | (ref)                                                           | 1.15x faster                                                                              |

Benchmark hidden because not significant (1): pickle
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown