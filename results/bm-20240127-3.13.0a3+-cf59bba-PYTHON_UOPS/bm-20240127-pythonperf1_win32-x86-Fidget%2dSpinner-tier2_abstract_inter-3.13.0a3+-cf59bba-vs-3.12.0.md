
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 250 ms: 1.12x faster                                                                      |
| chameleon      | 7.75 ms                                                         | 5.86 ms: 1.32x faster                                                                     |
| docutils       | 1.98 sec                                                        | 1.83 sec: 1.09x faster                                                                    |
| tornado_http   | 105 ms                                                          | 101 ms: 1.04x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.14x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none_tg         | 278 ms                                                          | 240 ms: 1.15x faster                                                                      |
| async_tree_none            | 298 ms                                                          | 261 ms: 1.14x faster                                                                      |
| async_tree_memoization_tg  | 350 ms                                                          | 311 ms: 1.13x faster                                                                      |
| async_tree_io_tg           | 677 ms                                                          | 605 ms: 1.12x faster                                                                      |
| async_tree_memoization     | 364 ms                                                          | 325 ms: 1.12x faster                                                                      |
| async_tree_io              | 693 ms                                                          | 628 ms: 1.10x faster                                                                      |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 522 ms: 1.08x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 514 ms: 1.06x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 85.2 ms: 1.49x faster                                                                     |
| float          | 76.7 ms                                                         | 58.5 ms: 1.31x faster                                                                     |
| pidigits       | 199 ms                                                          | 202 ms: 1.01x slower                                                                      |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 108 ms: 1.19x faster                                                                      |
| regex_effbot   | 2.04 ms                                                         | 1.91 ms: 1.07x faster                                                                     |
| regex_v8       | 15.0 ms                                                         | 16.2 ms: 1.08x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                              |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 149 us: 1.40x faster                                                                      |
| pickle_pure_python   | 286 us                                                          | 209 us: 1.37x faster                                                                      |
| tomli_loads          | 2.20 sec                                                        | 1.64 sec: 1.34x faster                                                                    |
| xml_etree_process    | 53.2 ms                                                         | 41.3 ms: 1.29x faster                                                                     |
| xml_etree_generate   | 72.1 ms                                                         | 60.6 ms: 1.19x faster                                                                     |
| xml_etree_iterparse  | 77.6 ms                                                         | 69.2 ms: 1.12x faster                                                                     |
| json_dumps           | 7.40 ms                                                         | 6.62 ms: 1.12x faster                                                                     |
| xml_etree_parse      | 113 ms                                                          | 110 ms: 1.03x faster                                                                      |
| json_loads           | 20.4 us                                                         | 19.9 us: 1.02x faster                                                                     |
| unpickle_list        | 2.95 us                                                         | 2.87 us: 1.02x faster                                                                     |
| pickle               | 7.79 us                                                         | 7.64 us: 1.02x faster                                                                     |
| pickle_dict          | 19.9 us                                                         | 20.2 us: 1.01x slower                                                                     |
| unpickle             | 9.71 us                                                         | 9.88 us: 1.02x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.12x faster                                                                              |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.5 ms: 1.05x slower                                                                     |
| python_startup_no_site | 19.1 ms                                                         | 21.1 ms: 1.11x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.86 ms: 1.27x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| logging_silent             | 101 ns                                                          | 59.5 ns: 1.70x faster                                                                     |
| generators                 | 38.5 ms                                                         | 23.2 ms: 1.66x faster                                                                     |
| unpack_sequence            | 62.5 ns                                                         | 39.5 ns: 1.58x faster                                                                     |
| scimark_sor                | 130 ms                                                          | 83.7 ms: 1.55x faster                                                                     |
| deepcopy_memo              | 38.4 us                                                         | 25.4 us: 1.51x faster                                                                     |
| scimark_lu                 | 93.2 ms                                                         | 62.1 ms: 1.50x faster                                                                     |
| nbody                      | 127 ms                                                          | 85.2 ms: 1.49x faster                                                                     |
| comprehensions             | 19.2 us                                                         | 13.2 us: 1.45x faster                                                                     |
| coroutines                 | 20.9 ms                                                         | 14.6 ms: 1.43x faster                                                                     |
| raytrace                   | 308 ms                                                          | 216 ms: 1.43x faster                                                                      |
| richards                   | 41.3 ms                                                         | 29.3 ms: 1.41x faster                                                                     |
| unpickle_pure_python       | 210 us                                                          | 149 us: 1.40x faster                                                                      |
| richards_super             | 46.5 ms                                                         | 33.5 ms: 1.39x faster                                                                     |
| pickle_pure_python         | 286 us                                                          | 209 us: 1.37x faster                                                                      |
| sqlglot_parse              | 1.25 ms                                                         | 920 us: 1.36x faster                                                                      |
| deltablue                  | 3.58 ms                                                         | 2.65 ms: 1.35x faster                                                                     |
| tomli_loads                | 2.20 sec                                                        | 1.64 sec: 1.34x faster                                                                    |
| typing_runtime_protocols   | 126 us                                                          | 94.8 us: 1.33x faster                                                                     |
| chaos                      | 69.4 ms                                                         | 52.1 ms: 1.33x faster                                                                     |
| chameleon                  | 7.75 ms                                                         | 5.86 ms: 1.32x faster                                                                     |
| hexiom                     | 6.82 ms                                                         | 5.18 ms: 1.32x faster                                                                     |
| deepcopy_reduce            | 3.23 us                                                         | 2.45 us: 1.32x faster                                                                     |
| float                      | 76.7 ms                                                         | 58.5 ms: 1.31x faster                                                                     |
| sqlglot_transpile          | 1.53 ms                                                         | 1.17 ms: 1.30x faster                                                                     |
| scimark_monte_carlo        | 66.4 ms                                                         | 51.3 ms: 1.29x faster                                                                     |
| xml_etree_process          | 53.2 ms                                                         | 41.3 ms: 1.29x faster                                                                     |
| deepcopy                   | 360 us                                                          | 280 us: 1.28x faster                                                                      |
| go                         | 137 ms                                                          | 107 ms: 1.28x faster                                                                      |
| spectral_norm              | 104 ms                                                          | 81.6 ms: 1.27x faster                                                                     |
| mako                       | 9.96 ms                                                         | 7.86 ms: 1.27x faster                                                                     |
| pyflate                    | 424 ms                                                          | 337 ms: 1.26x faster                                                                      |
| scimark_fft                | 271 ms                                                          | 217 ms: 1.25x faster                                                                      |
| nqueens                    | 93.7 ms                                                         | 77.0 ms: 1.22x faster                                                                     |
| fannkuch                   | 354 ms                                                          | 296 ms: 1.20x faster                                                                      |
| regex_compile              | 129 ms                                                          | 108 ms: 1.19x faster                                                                      |
| pprint_pformat             | 1.50 sec                                                        | 1.26 sec: 1.19x faster                                                                    |
| xml_etree_generate         | 72.1 ms                                                         | 60.6 ms: 1.19x faster                                                                     |
| crypto_pyaes               | 69.2 ms                                                         | 58.3 ms: 1.19x faster                                                                     |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.30 ms: 1.17x faster                                                                     |
| logging_simple             | 9.75 us                                                         | 8.37 us: 1.16x faster                                                                     |
| pprint_safe_repr           | 721 ms                                                          | 621 ms: 1.16x faster                                                                      |
| sqlglot_optimize           | 48.5 ms                                                         | 41.8 ms: 1.16x faster                                                                     |
| logging_format             | 10.4 us                                                         | 8.99 us: 1.16x faster                                                                     |
| async_generators           | 313 ms                                                          | 271 ms: 1.15x faster                                                                      |
| async_tree_none_tg         | 278 ms                                                          | 240 ms: 1.15x faster                                                                      |
| mdp                        | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                                                    |
| pycparser                  | 978 ms                                                          | 854 ms: 1.14x faster                                                                      |
| async_tree_none            | 298 ms                                                          | 261 ms: 1.14x faster                                                                      |
| sqlite_synth               | 2.07 us                                                         | 1.84 us: 1.13x faster                                                                     |
| sympy_integrate            | 17.5 ms                                                         | 15.6 ms: 1.13x faster                                                                     |
| async_tree_memoization_tg  | 350 ms                                                          | 311 ms: 1.13x faster                                                                      |
| xml_etree_iterparse        | 77.6 ms                                                         | 69.2 ms: 1.12x faster                                                                     |
| async_tree_io_tg           | 677 ms                                                          | 605 ms: 1.12x faster                                                                      |
| meteor_contest             | 86.9 ms                                                         | 77.6 ms: 1.12x faster                                                                     |
| sympy_str                  | 240 ms                                                          | 214 ms: 1.12x faster                                                                      |
| json_dumps                 | 7.40 ms                                                         | 6.62 ms: 1.12x faster                                                                     |
| async_tree_memoization     | 364 ms                                                          | 325 ms: 1.12x faster                                                                      |
| 2to3                       | 280 ms                                                          | 250 ms: 1.12x faster                                                                      |
| sympy_sum                  | 123 ms                                                          | 111 ms: 1.11x faster                                                                      |
| async_tree_io              | 693 ms                                                          | 628 ms: 1.10x faster                                                                      |
| docutils                   | 1.98 sec                                                        | 1.83 sec: 1.09x faster                                                                    |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 522 ms: 1.08x faster                                                                      |
| sympy_expand               | 398 ms                                                          | 372 ms: 1.07x faster                                                                      |
| regex_effbot               | 2.04 ms                                                         | 1.91 ms: 1.07x faster                                                                     |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 514 ms: 1.06x faster                                                                      |
| tornado_http               | 105 ms                                                          | 101 ms: 1.04x faster                                                                      |
| dask                       | 323 ms                                                          | 312 ms: 1.03x faster                                                                      |
| bench_thread_pool          | 1.10 ms                                                         | 1.07 ms: 1.03x faster                                                                     |
| pathlib                    | 91.4 ms                                                         | 88.7 ms: 1.03x faster                                                                     |
| gc_traversal               | 1.44 ms                                                         | 1.40 ms: 1.03x faster                                                                     |
| xml_etree_parse            | 113 ms                                                          | 110 ms: 1.03x faster                                                                      |
| json_loads                 | 20.4 us                                                         | 19.9 us: 1.02x faster                                                                     |
| unpickle_list              | 2.95 us                                                         | 2.87 us: 1.02x faster                                                                     |
| pickle                     | 7.79 us                                                         | 7.64 us: 1.02x faster                                                                     |
| pidigits                   | 199 ms                                                          | 202 ms: 1.01x slower                                                                      |
| pickle_dict                | 19.9 us                                                         | 20.2 us: 1.01x slower                                                                     |
| unpickle                   | 9.71 us                                                         | 9.88 us: 1.02x slower                                                                     |
| python_startup             | 22.4 ms                                                         | 23.5 ms: 1.05x slower                                                                     |
| regex_v8                   | 15.0 ms                                                         | 16.2 ms: 1.08x slower                                                                     |
| telco                      | 5.51 ms                                                         | 6.07 ms: 1.10x slower                                                                     |
| python_startup_no_site     | 19.1 ms                                                         | 21.1 ms: 1.11x slower                                                                     |
| sqlglot_normalize          | 100 ms                                                          | 213 ms: 2.12x slower                                                                      |
| coverage                   | 48.4 ms                                                         | 485 ms: 10.02x slower                                                                     |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                              |

Benchmark hidden because not significant (7): create_gc_cycles, regex_dna, json, asyncio_tcp_ssl, bench_mp_pool, asyncio_tcp, pickle_list
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown