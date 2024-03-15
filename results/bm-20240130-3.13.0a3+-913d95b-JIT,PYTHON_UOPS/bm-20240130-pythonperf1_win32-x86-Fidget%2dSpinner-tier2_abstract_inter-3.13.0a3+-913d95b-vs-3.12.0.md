
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 268 ms: 1.05x faster                                                                      |
| chameleon      | 7.75 ms                                                         | 6.17 ms: 1.26x faster                                                                     |
| docutils       | 1.98 sec                                                        | 1.86 sec: 1.07x faster                                                                    |
| tornado_http   | 105 ms                                                          | 103 ms: 1.02x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.09x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 264 ms: 1.13x faster                                                                      |
| async_tree_memoization_tg  | 350 ms                                                          | 314 ms: 1.12x faster                                                                      |
| async_tree_memoization     | 364 ms                                                          | 330 ms: 1.10x faster                                                                      |
| async_tree_none_tg         | 278 ms                                                          | 253 ms: 1.10x faster                                                                      |
| async_tree_io              | 693 ms                                                          | 634 ms: 1.09x faster                                                                      |
| async_tree_io_tg           | 677 ms                                                          | 625 ms: 1.08x faster                                                                      |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 527 ms: 1.07x faster                                                                      |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 513 ms: 1.06x faster                                                                      |
| Geometric mean             | (ref)                                                           | 1.09x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 90.8 ms: 1.40x faster                                                                     |
| float          | 76.7 ms                                                         | 55.7 ms: 1.38x faster                                                                     |
| pidigits       | 199 ms                                                          | 201 ms: 1.01x slower                                                                      |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 113 ms: 1.15x faster                                                                      |
| regex_effbot   | 2.04 ms                                                         | 1.91 ms: 1.07x faster                                                                     |
| regex_dna      | 127 ms                                                          | 122 ms: 1.04x faster                                                                      |
| regex_v8       | 15.0 ms                                                         | 16.2 ms: 1.08x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| tomli_loads          | 2.20 sec                                                        | 1.64 sec: 1.34x faster                                                                    |
| unpickle_pure_python | 210 us                                                          | 157 us: 1.33x faster                                                                      |
| pickle_pure_python   | 286 us                                                          | 227 us: 1.26x faster                                                                      |
| xml_etree_process    | 53.2 ms                                                         | 42.8 ms: 1.24x faster                                                                     |
| xml_etree_generate   | 72.1 ms                                                         | 62.3 ms: 1.16x faster                                                                     |
| xml_etree_iterparse  | 77.6 ms                                                         | 67.2 ms: 1.16x faster                                                                     |
| xml_etree_parse      | 113 ms                                                          | 104 ms: 1.09x faster                                                                      |
| unpickle_list        | 2.95 us                                                         | 2.79 us: 1.05x faster                                                                     |
| json_dumps           | 7.40 ms                                                         | 7.14 ms: 1.04x faster                                                                     |
| pickle_list          | 3.37 us                                                         | 3.31 us: 1.02x faster                                                                     |
| json_loads           | 20.4 us                                                         | 20.1 us: 1.01x faster                                                                     |
| pickle_dict          | 19.9 us                                                         | 20.5 us: 1.03x slower                                                                     |
| pickle               | 7.79 us                                                         | 8.07 us: 1.04x slower                                                                     |
| unpickle             | 9.71 us                                                         | 10.1 us: 1.04x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 23.6 ms: 1.05x slower                                                                     |
| python_startup_no_site | 19.1 ms                                                         | 21.1 ms: 1.11x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 8.01 ms: 1.24x faster                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 25.0 ms: 1.54x faster                                                                     |
| logging_silent             | 101 ns                                                          | 66.3 ns: 1.52x faster                                                                     |
| unpack_sequence            | 62.5 ns                                                         | 41.9 ns: 1.49x faster                                                                     |
| deepcopy_memo              | 38.4 us                                                         | 26.1 us: 1.47x faster                                                                     |
| nbody                      | 127 ms                                                          | 90.8 ms: 1.40x faster                                                                     |
| scimark_sor                | 130 ms                                                          | 93.2 ms: 1.39x faster                                                                     |
| coroutines                 | 20.9 ms                                                         | 15.2 ms: 1.38x faster                                                                     |
| float                      | 76.7 ms                                                         | 55.7 ms: 1.38x faster                                                                     |
| deltablue                  | 3.58 ms                                                         | 2.62 ms: 1.37x faster                                                                     |
| scimark_lu                 | 93.2 ms                                                         | 68.7 ms: 1.36x faster                                                                     |
| spectral_norm              | 104 ms                                                          | 77.4 ms: 1.34x faster                                                                     |
| tomli_loads                | 2.20 sec                                                        | 1.64 sec: 1.34x faster                                                                    |
| unpickle_pure_python       | 210 us                                                          | 157 us: 1.33x faster                                                                      |
| richards                   | 41.3 ms                                                         | 31.1 ms: 1.33x faster                                                                     |
| deepcopy_reduce            | 3.23 us                                                         | 2.45 us: 1.32x faster                                                                     |
| richards_super             | 46.5 ms                                                         | 35.3 ms: 1.32x faster                                                                     |
| sqlglot_parse              | 1.25 ms                                                         | 965 us: 1.29x faster                                                                      |
| typing_runtime_protocols   | 126 us                                                          | 97.9 us: 1.29x faster                                                                     |
| raytrace                   | 308 ms                                                          | 240 ms: 1.28x faster                                                                      |
| deepcopy                   | 360 us                                                          | 284 us: 1.27x faster                                                                      |
| pickle_pure_python         | 286 us                                                          | 227 us: 1.26x faster                                                                      |
| chameleon                  | 7.75 ms                                                         | 6.17 ms: 1.26x faster                                                                     |
| sqlglot_transpile          | 1.53 ms                                                         | 1.23 ms: 1.24x faster                                                                     |
| xml_etree_process          | 53.2 ms                                                         | 42.8 ms: 1.24x faster                                                                     |
| mako                       | 9.96 ms                                                         | 8.01 ms: 1.24x faster                                                                     |
| comprehensions             | 19.2 us                                                         | 15.9 us: 1.20x faster                                                                     |
| chaos                      | 69.4 ms                                                         | 58.0 ms: 1.20x faster                                                                     |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.23 ms: 1.19x faster                                                                     |
| logging_simple             | 9.75 us                                                         | 8.37 us: 1.16x faster                                                                     |
| xml_etree_generate         | 72.1 ms                                                         | 62.3 ms: 1.16x faster                                                                     |
| xml_etree_iterparse        | 77.6 ms                                                         | 67.2 ms: 1.16x faster                                                                     |
| logging_format             | 10.4 us                                                         | 9.01 us: 1.15x faster                                                                     |
| regex_compile              | 129 ms                                                          | 113 ms: 1.15x faster                                                                      |
| fannkuch                   | 354 ms                                                          | 310 ms: 1.14x faster                                                                      |
| async_tree_none            | 298 ms                                                          | 264 ms: 1.13x faster                                                                      |
| pycparser                  | 978 ms                                                          | 869 ms: 1.12x faster                                                                      |
| go                         | 137 ms                                                          | 122 ms: 1.12x faster                                                                      |
| async_tree_memoization_tg  | 350 ms                                                          | 314 ms: 1.12x faster                                                                      |
| sqlite_synth               | 2.07 us                                                         | 1.86 us: 1.12x faster                                                                     |
| pyflate                    | 424 ms                                                          | 383 ms: 1.11x faster                                                                      |
| async_tree_memoization     | 364 ms                                                          | 330 ms: 1.10x faster                                                                      |
| async_tree_none_tg         | 278 ms                                                          | 253 ms: 1.10x faster                                                                      |
| sqlglot_optimize           | 48.5 ms                                                         | 44.3 ms: 1.09x faster                                                                     |
| async_tree_io              | 693 ms                                                          | 634 ms: 1.09x faster                                                                      |
| xml_etree_parse            | 113 ms                                                          | 104 ms: 1.09x faster                                                                      |
| async_tree_io_tg           | 677 ms                                                          | 625 ms: 1.08x faster                                                                      |
| sympy_str                  | 240 ms                                                          | 221 ms: 1.08x faster                                                                      |
| crypto_pyaes               | 69.2 ms                                                         | 64.7 ms: 1.07x faster                                                                     |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 527 ms: 1.07x faster                                                                      |
| regex_effbot               | 2.04 ms                                                         | 1.91 ms: 1.07x faster                                                                     |
| docutils                   | 1.98 sec                                                        | 1.86 sec: 1.07x faster                                                                    |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 513 ms: 1.06x faster                                                                      |
| asyncio_tcp                | 662 ms                                                          | 622 ms: 1.06x faster                                                                      |
| sympy_sum                  | 123 ms                                                          | 116 ms: 1.06x faster                                                                      |
| scimark_fft                | 271 ms                                                          | 257 ms: 1.05x faster                                                                      |
| unpickle_list              | 2.95 us                                                         | 2.79 us: 1.05x faster                                                                     |
| sympy_expand               | 398 ms                                                          | 378 ms: 1.05x faster                                                                      |
| 2to3                       | 280 ms                                                          | 268 ms: 1.05x faster                                                                      |
| nqueens                    | 93.7 ms                                                         | 89.6 ms: 1.05x faster                                                                     |
| dask                       | 323 ms                                                          | 311 ms: 1.04x faster                                                                      |
| regex_dna                  | 127 ms                                                          | 122 ms: 1.04x faster                                                                      |
| json_dumps                 | 7.40 ms                                                         | 7.14 ms: 1.04x faster                                                                     |
| async_generators           | 313 ms                                                          | 303 ms: 1.03x faster                                                                      |
| bench_thread_pool          | 1.10 ms                                                         | 1.07 ms: 1.03x faster                                                                     |
| pprint_pformat             | 1.50 sec                                                        | 1.46 sec: 1.03x faster                                                                    |
| mdp                        | 1.91 sec                                                        | 1.87 sec: 1.02x faster                                                                    |
| pathlib                    | 91.4 ms                                                         | 89.2 ms: 1.02x faster                                                                     |
| tornado_http               | 105 ms                                                          | 103 ms: 1.02x faster                                                                      |
| sympy_integrate            | 17.5 ms                                                         | 17.2 ms: 1.02x faster                                                                     |
| gc_traversal               | 1.44 ms                                                         | 1.41 ms: 1.02x faster                                                                     |
| pickle_list                | 3.37 us                                                         | 3.31 us: 1.02x faster                                                                     |
| pprint_safe_repr           | 721 ms                                                          | 711 ms: 1.01x faster                                                                      |
| json_loads                 | 20.4 us                                                         | 20.1 us: 1.01x faster                                                                     |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 17.8 sec: 1.01x slower                                                                    |
| pidigits                   | 199 ms                                                          | 201 ms: 1.01x slower                                                                      |
| bench_mp_pool              | 75.4 ms                                                         | 76.3 ms: 1.01x slower                                                                     |
| meteor_contest             | 86.9 ms                                                         | 88.3 ms: 1.02x slower                                                                     |
| create_gc_cycles           | 652 us                                                          | 668 us: 1.03x slower                                                                      |
| pickle_dict                | 19.9 us                                                         | 20.5 us: 1.03x slower                                                                     |
| pickle                     | 7.79 us                                                         | 8.07 us: 1.04x slower                                                                     |
| unpickle                   | 9.71 us                                                         | 10.1 us: 1.04x slower                                                                     |
| hexiom                     | 6.82 ms                                                         | 7.09 ms: 1.04x slower                                                                     |
| python_startup             | 22.4 ms                                                         | 23.6 ms: 1.05x slower                                                                     |
| scimark_monte_carlo        | 66.4 ms                                                         | 70.3 ms: 1.06x slower                                                                     |
| regex_v8                   | 15.0 ms                                                         | 16.2 ms: 1.08x slower                                                                     |
| python_startup_no_site     | 19.1 ms                                                         | 21.1 ms: 1.11x slower                                                                     |
| json                       | 4.15 ms                                                         | 4.71 ms: 1.13x slower                                                                     |
| telco                      | 5.51 ms                                                         | 6.44 ms: 1.17x slower                                                                     |
| sqlglot_normalize          | 100 ms                                                          | 227 ms: 2.26x slower                                                                      |
| coverage                   | 48.4 ms                                                         | 483 ms: 9.97x slower                                                                      |
| Geometric mean             | (ref)                                                           | 1.08x faster                                                                              |
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown