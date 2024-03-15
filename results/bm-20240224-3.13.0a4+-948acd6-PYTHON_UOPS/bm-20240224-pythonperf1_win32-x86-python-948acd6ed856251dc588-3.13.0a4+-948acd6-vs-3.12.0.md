
# Results vs. 3.12.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 246 ms: 1.14x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.94 ms: 1.30x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.84 sec: 1.08x faster                                                          |
| tornado_http   | 105 ms                                                          | 97.4 ms: 1.08x faster                                                           |
| Geometric mean | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 248 ms: 1.20x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 234 ms: 1.19x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 297 ms: 1.18x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 311 ms: 1.17x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 584 ms: 1.16x faster                                                            |
| async_tree_io              | 693 ms                                                          | 600 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 504 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 491 ms: 1.11x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.16x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 80.8 ms: 1.57x faster                                                           |
| float          | 76.7 ms                                                         | 61.6 ms: 1.24x faster                                                           |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.25x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| regex_dna      | 127 ms                                                          | 119 ms: 1.07x faster                                                            |
| regex_compile  | 129 ms                                                          | 121 ms: 1.07x faster                                                            |
| regex_v8       | 15.0 ms                                                         | 16.4 ms: 1.09x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_pure_python   | 286 us                                                          | 216 us: 1.32x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.66 sec: 1.32x faster                                                          |
| xml_etree_process    | 53.2 ms                                                         | 42.4 ms: 1.26x faster                                                           |
| unpickle_pure_python | 210 us                                                          | 171 us: 1.23x faster                                                            |
| xml_etree_generate   | 72.1 ms                                                         | 59.8 ms: 1.21x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.1 ms: 1.14x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.87 ms: 1.08x faster                                                           |
| unpickle_list        | 2.95 us                                                         | 2.81 us: 1.05x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| pickle_list          | 3.37 us                                                         | 3.27 us: 1.03x faster                                                           |
| json_loads           | 20.4 us                                                         | 19.8 us: 1.03x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 20.2 us: 1.02x slower                                                           |
| unpickle             | 9.71 us                                                         | 9.86 us: 1.02x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.1 ms: 1.01x faster                                                           |
| python_startup_no_site | 19.1 ms                                                         | 19.9 ms: 1.04x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.02x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.65 ms: 1.30x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 23.2 ms: 1.66x faster                                                           |
| logging_silent             | 101 ns                                                          | 61.6 ns: 1.64x faster                                                           |
| nbody                      | 127 ms                                                          | 80.8 ms: 1.57x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 25.0 us: 1.54x faster                                                           |
| deltablue                  | 3.58 ms                                                         | 2.43 ms: 1.47x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.9 ms: 1.40x faster                                                           |
| richards_super             | 46.5 ms                                                         | 33.2 ms: 1.40x faster                                                           |
| richards                   | 41.3 ms                                                         | 29.6 ms: 1.40x faster                                                           |
| scimark_sor                | 130 ms                                                          | 93.9 ms: 1.38x faster                                                           |
| raytrace                   | 308 ms                                                          | 229 ms: 1.35x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 94.3 us: 1.34x faster                                                           |
| comprehensions             | 19.2 us                                                         | 14.4 us: 1.33x faster                                                           |
| chaos                      | 69.4 ms                                                         | 52.2 ms: 1.33x faster                                                           |
| spectral_norm              | 104 ms                                                          | 78.4 ms: 1.32x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 216 us: 1.32x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.66 sec: 1.32x faster                                                          |
| sqlglot_parse              | 1.25 ms                                                         | 948 us: 1.32x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.94 ms: 1.30x faster                                                           |
| mako                       | 9.96 ms                                                         | 7.65 ms: 1.30x faster                                                           |
| deepcopy_reduce            | 3.23 us                                                         | 2.50 us: 1.29x faster                                                           |
| scimark_fft                | 271 ms                                                          | 212 ms: 1.28x faster                                                            |
| fannkuch                   | 354 ms                                                          | 277 ms: 1.28x faster                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.20 ms: 1.28x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 52.5 ms: 1.27x faster                                                           |
| deepcopy                   | 360 us                                                          | 285 us: 1.26x faster                                                            |
| xml_etree_process          | 53.2 ms                                                         | 42.4 ms: 1.26x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 55.4 ms: 1.25x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.10 ms: 1.24x faster                                                           |
| float                      | 76.7 ms                                                         | 61.6 ms: 1.24x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 50.7 ns: 1.23x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 171 us: 1.23x faster                                                            |
| pyflate                    | 424 ms                                                          | 348 ms: 1.22x faster                                                            |
| logging_simple             | 9.75 us                                                         | 8.02 us: 1.22x faster                                                           |
| logging_format             | 10.4 us                                                         | 8.59 us: 1.21x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 59.8 ms: 1.21x faster                                                           |
| pprint_pformat             | 1.50 sec                                                        | 1.25 sec: 1.20x faster                                                          |
| async_tree_none            | 298 ms                                                          | 248 ms: 1.20x faster                                                            |
| go                         | 137 ms                                                          | 116 ms: 1.19x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 234 ms: 1.19x faster                                                            |
| pprint_safe_repr           | 721 ms                                                          | 608 ms: 1.18x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 297 ms: 1.18x faster                                                            |
| hexiom                     | 6.82 ms                                                         | 5.80 ms: 1.18x faster                                                           |
| scimark_lu                 | 93.2 ms                                                         | 79.3 ms: 1.18x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 80.1 ms: 1.17x faster                                                           |
| async_tree_memoization     | 364 ms                                                          | 311 ms: 1.17x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 584 ms: 1.16x faster                                                            |
| async_tree_io              | 693 ms                                                          | 600 ms: 1.15x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.66 sec: 1.15x faster                                                          |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.1 ms: 1.14x faster                                                           |
| 2to3                       | 280 ms                                                          | 246 ms: 1.14x faster                                                            |
| async_generators           | 313 ms                                                          | 280 ms: 1.12x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 504 ms: 1.12x faster                                                            |
| sqlglot_optimize           | 48.5 ms                                                         | 43.3 ms: 1.12x faster                                                           |
| pycparser                  | 978 ms                                                          | 879 ms: 1.11x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 491 ms: 1.11x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.8 ms: 1.11x faster                                                           |
| sympy_sum                  | 123 ms                                                          | 111 ms: 1.11x faster                                                            |
| sympy_str                  | 240 ms                                                          | 218 ms: 1.10x faster                                                            |
| tornado_http               | 105 ms                                                          | 97.4 ms: 1.08x faster                                                           |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                                           |
| json_dumps                 | 7.40 ms                                                         | 6.87 ms: 1.08x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 80.7 ms: 1.08x faster                                                           |
| docutils                   | 1.98 sec                                                        | 1.84 sec: 1.08x faster                                                          |
| bench_mp_pool              | 75.4 ms                                                         | 70.1 ms: 1.08x faster                                                           |
| regex_dna                  | 127 ms                                                          | 119 ms: 1.07x faster                                                            |
| regex_compile              | 129 ms                                                          | 121 ms: 1.07x faster                                                            |
| pathlib                    | 91.4 ms                                                         | 85.8 ms: 1.07x faster                                                           |
| asyncio_tcp                | 662 ms                                                          | 624 ms: 1.06x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.04 ms: 1.06x faster                                                           |
| unpickle_list              | 2.95 us                                                         | 2.81 us: 1.05x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.9 sec: 1.05x faster                                                          |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| sympy_expand               | 398 ms                                                          | 383 ms: 1.04x faster                                                            |
| sqlite_synth               | 2.07 us                                                         | 2.00 us: 1.04x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.27 us: 1.03x faster                                                           |
| json_loads                 | 20.4 us                                                         | 19.8 us: 1.03x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.41 ms: 1.02x faster                                                           |
| python_startup             | 22.4 ms                                                         | 22.1 ms: 1.01x faster                                                           |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                            |
| pickle_dict                | 19.9 us                                                         | 20.2 us: 1.02x slower                                                           |
| unpickle                   | 9.71 us                                                         | 9.86 us: 1.02x slower                                                           |
| json                       | 4.15 ms                                                         | 4.25 ms: 1.02x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 19.9 ms: 1.04x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 16.4 ms: 1.09x slower                                                           |
| telco                      | 5.51 ms                                                         | 6.08 ms: 1.10x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 225 ms: 2.24x slower                                                            |
| coverage                   | 48.4 ms                                                         | 470 ms: 9.69x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (2): pickle, create_gc_cycles
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown