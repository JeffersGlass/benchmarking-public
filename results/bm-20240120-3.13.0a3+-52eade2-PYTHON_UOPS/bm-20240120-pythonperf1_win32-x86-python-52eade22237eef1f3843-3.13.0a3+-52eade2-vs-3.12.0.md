
# Results vs. 3.12.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-x86
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.16x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 241 ms: 1.16x faster                                                            |
| chameleon      | 7.75 ms                                                         | 5.80 ms: 1.33x faster                                                           |
| docutils       | 1.98 sec                                                        | 1.80 sec: 1.10x faster                                                          |
| tornado_http   | 105 ms                                                          | 101 ms: 1.04x faster                                                            |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 252 ms: 1.18x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 300 ms: 1.17x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 238 ms: 1.16x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 588 ms: 1.15x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 316 ms: 1.15x faster                                                            |
| async_tree_io              | 693 ms                                                          | 605 ms: 1.15x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 510 ms: 1.10x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 503 ms: 1.08x faster                                                            |
| Geometric mean             | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 85.3 ms: 1.49x faster                                                           |
| float          | 76.7 ms                                                         | 57.4 ms: 1.34x faster                                                           |
| pidigits       | 199 ms                                                          | 197 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                           | 1.26x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 103 ms: 1.25x faster                                                            |
| regex_dna      | 127 ms                                                          | 116 ms: 1.09x faster                                                            |
| regex_effbot   | 2.04 ms                                                         | 1.87 ms: 1.09x faster                                                           |
| regex_v8       | 15.0 ms                                                         | 15.9 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                           | 1.09x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 153 us: 1.37x faster                                                            |
| tomli_loads          | 2.20 sec                                                        | 1.61 sec: 1.37x faster                                                          |
| pickle_pure_python   | 286 us                                                          | 212 us: 1.35x faster                                                            |
| xml_etree_process    | 53.2 ms                                                         | 41.0 ms: 1.30x faster                                                           |
| xml_etree_generate   | 72.1 ms                                                         | 59.2 ms: 1.22x faster                                                           |
| xml_etree_iterparse  | 77.6 ms                                                         | 68.4 ms: 1.14x faster                                                           |
| json_dumps           | 7.40 ms                                                         | 6.75 ms: 1.10x faster                                                           |
| pickle_list          | 3.37 us                                                         | 3.22 us: 1.05x faster                                                           |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| json_loads           | 20.4 us                                                         | 19.7 us: 1.03x faster                                                           |
| pickle               | 7.79 us                                                         | 7.67 us: 1.02x faster                                                           |
| pickle_dict          | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (2): unpickle, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.9 ms: 1.03x slower                                                           |
| python_startup_no_site | 19.1 ms                                                         | 20.6 ms: 1.08x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.57 ms: 1.32x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 22.4 ms: 1.72x faster                                                           |
| logging_silent             | 101 ns                                                          | 60.6 ns: 1.67x faster                                                           |
| deepcopy_memo              | 38.4 us                                                         | 24.5 us: 1.57x faster                                                           |
| unpack_sequence            | 62.5 ns                                                         | 40.4 ns: 1.54x faster                                                           |
| scimark_sor                | 130 ms                                                          | 84.1 ms: 1.54x faster                                                           |
| raytrace                   | 308 ms                                                          | 201 ms: 1.53x faster                                                            |
| scimark_lu                 | 93.2 ms                                                         | 62.2 ms: 1.50x faster                                                           |
| nbody                      | 127 ms                                                          | 85.3 ms: 1.49x faster                                                           |
| coroutines                 | 20.9 ms                                                         | 14.2 ms: 1.47x faster                                                           |
| comprehensions             | 19.2 us                                                         | 13.2 us: 1.45x faster                                                           |
| richards                   | 41.3 ms                                                         | 28.5 ms: 1.45x faster                                                           |
| richards_super             | 46.5 ms                                                         | 32.8 ms: 1.41x faster                                                           |
| sqlglot_parse              | 1.25 ms                                                         | 887 us: 1.41x faster                                                            |
| typing_runtime_protocols   | 126 us                                                          | 91.6 us: 1.38x faster                                                           |
| unpickle_pure_python       | 210 us                                                          | 153 us: 1.37x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.61 sec: 1.37x faster                                                          |
| deltablue                  | 3.58 ms                                                         | 2.63 ms: 1.36x faster                                                           |
| sqlglot_transpile          | 1.53 ms                                                         | 1.13 ms: 1.36x faster                                                           |
| chaos                      | 69.4 ms                                                         | 51.4 ms: 1.35x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 212 us: 1.35x faster                                                            |
| hexiom                     | 6.82 ms                                                         | 5.07 ms: 1.35x faster                                                           |
| float                      | 76.7 ms                                                         | 57.4 ms: 1.34x faster                                                           |
| chameleon                  | 7.75 ms                                                         | 5.80 ms: 1.33x faster                                                           |
| deepcopy                   | 360 us                                                          | 271 us: 1.33x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.43 us: 1.33x faster                                                           |
| scimark_monte_carlo        | 66.4 ms                                                         | 50.1 ms: 1.33x faster                                                           |
| go                         | 137 ms                                                          | 104 ms: 1.32x faster                                                            |
| mako                       | 9.96 ms                                                         | 7.57 ms: 1.32x faster                                                           |
| xml_etree_process          | 53.2 ms                                                         | 41.0 ms: 1.30x faster                                                           |
| crypto_pyaes               | 69.2 ms                                                         | 53.8 ms: 1.29x faster                                                           |
| pyflate                    | 424 ms                                                          | 338 ms: 1.25x faster                                                            |
| logging_simple             | 9.75 us                                                         | 7.79 us: 1.25x faster                                                           |
| regex_compile              | 129 ms                                                          | 103 ms: 1.25x faster                                                            |
| logging_format             | 10.4 us                                                         | 8.34 us: 1.25x faster                                                           |
| scimark_fft                | 271 ms                                                          | 220 ms: 1.23x faster                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.22 sec: 1.23x faster                                                          |
| sqlglot_optimize           | 48.5 ms                                                         | 39.6 ms: 1.22x faster                                                           |
| xml_etree_generate         | 72.1 ms                                                         | 59.2 ms: 1.22x faster                                                           |
| spectral_norm              | 104 ms                                                          | 85.7 ms: 1.21x faster                                                           |
| pprint_safe_repr           | 721 ms                                                          | 596 ms: 1.21x faster                                                            |
| nqueens                    | 93.7 ms                                                         | 77.8 ms: 1.20x faster                                                           |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.21 ms: 1.20x faster                                                           |
| pycparser                  | 978 ms                                                          | 816 ms: 1.20x faster                                                            |
| async_tree_none            | 298 ms                                                          | 252 ms: 1.18x faster                                                            |
| mdp                        | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                          |
| async_generators           | 313 ms                                                          | 268 ms: 1.17x faster                                                            |
| async_tree_memoization_tg  | 350 ms                                                          | 300 ms: 1.17x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 238 ms: 1.16x faster                                                            |
| sympy_integrate            | 17.5 ms                                                         | 15.1 ms: 1.16x faster                                                           |
| 2to3                       | 280 ms                                                          | 241 ms: 1.16x faster                                                            |
| fannkuch                   | 354 ms                                                          | 305 ms: 1.16x faster                                                            |
| sympy_sum                  | 123 ms                                                          | 106 ms: 1.16x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 588 ms: 1.15x faster                                                            |
| sympy_str                  | 240 ms                                                          | 208 ms: 1.15x faster                                                            |
| async_tree_memoization     | 364 ms                                                          | 316 ms: 1.15x faster                                                            |
| async_tree_io              | 693 ms                                                          | 605 ms: 1.15x faster                                                            |
| xml_etree_iterparse        | 77.6 ms                                                         | 68.4 ms: 1.14x faster                                                           |
| sqlite_synth               | 2.07 us                                                         | 1.84 us: 1.13x faster                                                           |
| meteor_contest             | 86.9 ms                                                         | 77.3 ms: 1.12x faster                                                           |
| sympy_expand               | 398 ms                                                          | 359 ms: 1.11x faster                                                            |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 510 ms: 1.10x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.80 sec: 1.10x faster                                                          |
| json_dumps                 | 7.40 ms                                                         | 6.75 ms: 1.10x faster                                                           |
| regex_dna                  | 127 ms                                                          | 116 ms: 1.09x faster                                                            |
| asyncio_tcp                | 662 ms                                                          | 608 ms: 1.09x faster                                                            |
| regex_effbot               | 2.04 ms                                                         | 1.87 ms: 1.09x faster                                                           |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 503 ms: 1.08x faster                                                            |
| dask                       | 323 ms                                                          | 302 ms: 1.07x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.04 ms: 1.06x faster                                                           |
| pickle_list                | 3.37 us                                                         | 3.22 us: 1.05x faster                                                           |
| tornado_http               | 105 ms                                                          | 101 ms: 1.04x faster                                                            |
| pathlib                    | 91.4 ms                                                         | 87.6 ms: 1.04x faster                                                           |
| gc_traversal               | 1.44 ms                                                         | 1.38 ms: 1.04x faster                                                           |
| bench_mp_pool              | 75.4 ms                                                         | 72.5 ms: 1.04x faster                                                           |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                            |
| json_loads                 | 20.4 us                                                         | 19.7 us: 1.03x faster                                                           |
| json                       | 4.15 ms                                                         | 4.06 ms: 1.02x faster                                                           |
| pickle                     | 7.79 us                                                         | 7.67 us: 1.02x faster                                                           |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 17.4 sec: 1.02x faster                                                          |
| pidigits                   | 199 ms                                                          | 197 ms: 1.01x faster                                                            |
| pickle_dict                | 19.9 us                                                         | 20.1 us: 1.01x slower                                                           |
| python_startup             | 22.4 ms                                                         | 22.9 ms: 1.03x slower                                                           |
| telco                      | 5.51 ms                                                         | 5.82 ms: 1.06x slower                                                           |
| regex_v8                   | 15.0 ms                                                         | 15.9 ms: 1.06x slower                                                           |
| python_startup_no_site     | 19.1 ms                                                         | 20.6 ms: 1.08x slower                                                           |
| sqlglot_normalize          | 100 ms                                                          | 202 ms: 2.02x slower                                                            |
| coverage                   | 48.4 ms                                                         | 474 ms: 9.79x slower                                                            |
| Geometric mean             | (ref)                                                           | 1.16x faster                                                                    |

Benchmark hidden because not significant (3): unpickle, unpickle_list, create_gc_cycles
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: unknown