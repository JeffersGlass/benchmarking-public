
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.14x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 252 ms: 1.11x faster                                                                      |
| chameleon      | 7.75 ms                                                         | 5.72 ms: 1.35x faster                                                                     |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.09x faster                                                                    |
| tornado_http   | 105 ms                                                          | 99.9 ms: 1.05x faster                                                                     |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none_tg         | 278 ms                                                          | 237 ms: 1.17x faster                                                                      |
| async_tree_memoization_tg  | 350 ms                                                          | 301 ms: 1.17x faster                                                                      |
| async_tree_none            | 298 ms                                                          | 256 ms: 1.16x faster                                                                      |
| async_tree_memoization     | 364 ms                                                          | 320 ms: 1.14x faster                                                                      |
| async_tree_io_tg           | 677 ms                                                          | 599 ms: 1.13x faster                                                                      |
| async_tree_io              | 693 ms                                                          | 614 ms: 1.13x faster                                                                      |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 501 ms: 1.13x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 499 ms: 1.09x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.14x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 82.3 ms: 1.54x faster                                                                     |
| float          | 76.7 ms                                                         | 56.6 ms: 1.35x faster                                                                     |
| Geometric mean | (ref)                                                           | 1.28x faster                                                                              |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 107 ms: 1.21x faster                                                                      |
| regex_effbot   | 2.04 ms                                                         | 1.91 ms: 1.07x faster                                                                     |
| regex_dna      | 127 ms                                                          | 120 ms: 1.05x faster                                                                      |
| regex_v8       | 15.0 ms                                                         | 16.3 ms: 1.08x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 150 us: 1.40x faster                                                                      |
| pickle_pure_python   | 286 us                                                          | 211 us: 1.35x faster                                                                      |
| tomli_loads          | 2.20 sec                                                        | 1.67 sec: 1.31x faster                                                                    |
| xml_etree_process    | 53.2 ms                                                         | 41.1 ms: 1.29x faster                                                                     |
| xml_etree_generate   | 72.1 ms                                                         | 60.3 ms: 1.20x faster                                                                     |
| xml_etree_iterparse  | 77.6 ms                                                         | 69.9 ms: 1.11x faster                                                                     |
| json_dumps           | 7.40 ms                                                         | 6.84 ms: 1.08x faster                                                                     |
| xml_etree_parse      | 113 ms                                                          | 112 ms: 1.01x faster                                                                      |
| unpickle             | 9.71 us                                                         | 9.62 us: 1.01x faster                                                                     |
| json_loads           | 20.4 us                                                         | 20.2 us: 1.01x faster                                                                     |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                                                     |
| pickle               | 7.79 us                                                         | 7.88 us: 1.01x slower                                                                     |
| unpickle_list        | 2.95 us                                                         | 3.01 us: 1.02x slower                                                                     |
| pickle_list          | 3.37 us                                                         | 3.52 us: 1.04x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.9 ms: 1.03x slower                                                                     |
| python_startup_no_site | 19.1 ms                                                         | 20.7 ms: 1.09x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.73 ms: 1.29x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 60.6 ns: 1.67x faster                                                                     |
| generators                 | 38.5 ms                                                         | 23.3 ms: 1.65x faster                                                                     |
| scimark_sor                | 130 ms                                                          | 81.5 ms: 1.59x faster                                                                     |
| deepcopy_memo              | 38.4 us                                                         | 24.3 us: 1.58x faster                                                                     |
| nbody                      | 127 ms                                                          | 82.3 ms: 1.54x faster                                                                     |
| raytrace                   | 308 ms                                                          | 203 ms: 1.52x faster                                                                      |
| scimark_lu                 | 93.2 ms                                                         | 62.7 ms: 1.49x faster                                                                     |
| coroutines                 | 20.9 ms                                                         | 14.4 ms: 1.45x faster                                                                     |
| comprehensions             | 19.2 us                                                         | 13.3 us: 1.45x faster                                                                     |
| unpickle_pure_python       | 210 us                                                          | 150 us: 1.40x faster                                                                      |
| deepcopy_reduce            | 3.23 us                                                         | 2.33 us: 1.39x faster                                                                     |
| richards                   | 41.3 ms                                                         | 30.3 ms: 1.37x faster                                                                     |
| unpack_sequence            | 62.5 ns                                                         | 46.1 ns: 1.36x faster                                                                     |
| chameleon                  | 7.75 ms                                                         | 5.72 ms: 1.35x faster                                                                     |
| float                      | 76.7 ms                                                         | 56.6 ms: 1.35x faster                                                                     |
| pickle_pure_python         | 286 us                                                          | 211 us: 1.35x faster                                                                      |
| typing_runtime_protocols   | 126 us                                                          | 93.4 us: 1.35x faster                                                                     |
| deepcopy                   | 360 us                                                          | 266 us: 1.35x faster                                                                      |
| hexiom                     | 6.82 ms                                                         | 5.08 ms: 1.34x faster                                                                     |
| richards_super             | 46.5 ms                                                         | 34.7 ms: 1.34x faster                                                                     |
| deltablue                  | 3.58 ms                                                         | 2.68 ms: 1.34x faster                                                                     |
| sqlglot_parse              | 1.25 ms                                                         | 935 us: 1.33x faster                                                                      |
| spectral_norm              | 104 ms                                                          | 78.2 ms: 1.33x faster                                                                     |
| tomli_loads                | 2.20 sec                                                        | 1.67 sec: 1.31x faster                                                                    |
| sqlglot_transpile          | 1.53 ms                                                         | 1.17 ms: 1.31x faster                                                                     |
| scimark_monte_carlo        | 66.4 ms                                                         | 50.9 ms: 1.30x faster                                                                     |
| xml_etree_process          | 53.2 ms                                                         | 41.1 ms: 1.29x faster                                                                     |
| chaos                      | 69.4 ms                                                         | 53.6 ms: 1.29x faster                                                                     |
| mako                       | 9.96 ms                                                         | 7.73 ms: 1.29x faster                                                                     |
| go                         | 137 ms                                                          | 107 ms: 1.28x faster                                                                      |
| scimark_fft                | 271 ms                                                          | 212 ms: 1.28x faster                                                                      |
| pyflate                    | 424 ms                                                          | 335 ms: 1.27x faster                                                                      |
| pprint_pformat             | 1.50 sec                                                        | 1.22 sec: 1.23x faster                                                                    |
| fannkuch                   | 354 ms                                                          | 289 ms: 1.22x faster                                                                      |
| nqueens                    | 93.7 ms                                                         | 77.0 ms: 1.22x faster                                                                     |
| regex_compile              | 129 ms                                                          | 107 ms: 1.21x faster                                                                      |
| pprint_safe_repr           | 721 ms                                                          | 600 ms: 1.20x faster                                                                      |
| logging_format             | 10.4 us                                                         | 8.66 us: 1.20x faster                                                                     |
| logging_simple             | 9.75 us                                                         | 8.12 us: 1.20x faster                                                                     |
| xml_etree_generate         | 72.1 ms                                                         | 60.3 ms: 1.20x faster                                                                     |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.26 ms: 1.18x faster                                                                     |
| async_tree_none_tg         | 278 ms                                                          | 237 ms: 1.17x faster                                                                      |
| async_tree_memoization_tg  | 350 ms                                                          | 301 ms: 1.17x faster                                                                      |
| mdp                        | 1.91 sec                                                        | 1.64 sec: 1.16x faster                                                                    |
| async_tree_none            | 298 ms                                                          | 256 ms: 1.16x faster                                                                      |
| sqlglot_optimize           | 48.5 ms                                                         | 41.8 ms: 1.16x faster                                                                     |
| crypto_pyaes               | 69.2 ms                                                         | 59.7 ms: 1.16x faster                                                                     |
| sympy_str                  | 240 ms                                                          | 209 ms: 1.14x faster                                                                      |
| pycparser                  | 978 ms                                                          | 857 ms: 1.14x faster                                                                      |
| async_tree_memoization     | 364 ms                                                          | 320 ms: 1.14x faster                                                                      |
| sympy_integrate            | 17.5 ms                                                         | 15.5 ms: 1.13x faster                                                                     |
| async_tree_io_tg           | 677 ms                                                          | 599 ms: 1.13x faster                                                                      |
| async_tree_io              | 693 ms                                                          | 614 ms: 1.13x faster                                                                      |
| sympy_sum                  | 123 ms                                                          | 109 ms: 1.13x faster                                                                      |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 501 ms: 1.13x faster                                                                      |
| sqlite_synth               | 2.07 us                                                         | 1.85 us: 1.12x faster                                                                     |
| 2to3                       | 280 ms                                                          | 252 ms: 1.11x faster                                                                      |
| xml_etree_iterparse        | 77.6 ms                                                         | 69.9 ms: 1.11x faster                                                                     |
| async_generators           | 313 ms                                                          | 283 ms: 1.11x faster                                                                      |
| meteor_contest             | 86.9 ms                                                         | 79.3 ms: 1.09x faster                                                                     |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 499 ms: 1.09x faster                                                                      |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.09x faster                                                                    |
| sympy_expand               | 398 ms                                                          | 366 ms: 1.09x faster                                                                      |
| json_dumps                 | 7.40 ms                                                         | 6.84 ms: 1.08x faster                                                                     |
| regex_effbot               | 2.04 ms                                                         | 1.91 ms: 1.07x faster                                                                     |
| asyncio_tcp                | 662 ms                                                          | 622 ms: 1.06x faster                                                                      |
| regex_dna                  | 127 ms                                                          | 120 ms: 1.05x faster                                                                      |
| tornado_http               | 105 ms                                                          | 99.9 ms: 1.05x faster                                                                     |
| dask                       | 323 ms                                                          | 312 ms: 1.04x faster                                                                      |
| pathlib                    | 91.4 ms                                                         | 89.2 ms: 1.02x faster                                                                     |
| json                       | 4.15 ms                                                         | 4.06 ms: 1.02x faster                                                                     |
| gc_traversal               | 1.44 ms                                                         | 1.42 ms: 1.01x faster                                                                     |
| xml_etree_parse            | 113 ms                                                          | 112 ms: 1.01x faster                                                                      |
| unpickle                   | 9.71 us                                                         | 9.62 us: 1.01x faster                                                                     |
| json_loads                 | 20.4 us                                                         | 20.2 us: 1.01x faster                                                                     |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                                                     |
| pickle                     | 7.79 us                                                         | 7.88 us: 1.01x slower                                                                     |
| unpickle_list              | 2.95 us                                                         | 3.01 us: 1.02x slower                                                                     |
| python_startup             | 22.4 ms                                                         | 22.9 ms: 1.03x slower                                                                     |
| pickle_list                | 3.37 us                                                         | 3.52 us: 1.04x slower                                                                     |
| telco                      | 5.51 ms                                                         | 5.92 ms: 1.07x slower                                                                     |
| regex_v8                   | 15.0 ms                                                         | 16.3 ms: 1.08x slower                                                                     |
| python_startup_no_site     | 19.1 ms                                                         | 20.7 ms: 1.09x slower                                                                     |
| sqlglot_normalize          | 100 ms                                                          | 214 ms: 2.13x slower                                                                      |
| coverage                   | 48.4 ms                                                         | 461 ms: 9.53x slower                                                                      |
| Geometric mean             | (ref)                                                           | 1.14x faster                                                                              |

Benchmark hidden because not significant (5): bench_thread_pool, pidigits, bench_mp_pool, create_gc_cycles, asyncio_tcp_ssl
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown