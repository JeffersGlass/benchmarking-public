
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_continue
- machine: windows-x86
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 247 ms: 1.13x faster                                                             |
| chameleon      | 7.75 ms                                                         | 5.91 ms: 1.31x faster                                                            |
| docutils       | 1.98 sec                                                        | 1.77 sec: 1.12x faster                                                           |
| tornado_http   | 105 ms                                                          | 96.4 ms: 1.09x faster                                                            |
| Geometric mean | (ref)                                                           | 1.16x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 250 ms: 1.19x faster                                                             |
| async_tree_none_tg         | 278 ms                                                          | 239 ms: 1.16x faster                                                             |
| async_tree_memoization_tg  | 350 ms                                                          | 302 ms: 1.16x faster                                                             |
| async_tree_memoization     | 364 ms                                                          | 313 ms: 1.16x faster                                                             |
| async_tree_io              | 693 ms                                                          | 601 ms: 1.15x faster                                                             |
| async_tree_io_tg           | 677 ms                                                          | 590 ms: 1.15x faster                                                             |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 510 ms: 1.10x faster                                                             |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 501 ms: 1.09x faster                                                             |
| Geometric mean             | (ref)                                                           | 1.15x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 53.8 ms: 1.42x faster                                                            |
| nbody          | 127 ms                                                          | 93.5 ms: 1.36x faster                                                            |
| pidigits       | 199 ms                                                          | 201 ms: 1.01x slower                                                             |
| Geometric mean | (ref)                                                           | 1.24x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 103 ms: 1.25x faster                                                             |
| regex_effbot   | 2.04 ms                                                         | 1.91 ms: 1.07x faster                                                            |
| regex_dna      | 127 ms                                                          | 123 ms: 1.03x faster                                                             |
| regex_v8       | 15.0 ms                                                         | 16.1 ms: 1.07x slower                                                            |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 2.20 sec                                                        | 1.60 sec: 1.37x faster                                                           |
| pickle_pure_python   | 286 us                                                          | 210 us: 1.36x faster                                                             |
| unpickle_pure_python | 210 us                                                          | 155 us: 1.36x faster                                                             |
| xml_etree_process    | 53.2 ms                                                         | 41.5 ms: 1.28x faster                                                            |
| xml_etree_generate   | 72.1 ms                                                         | 58.4 ms: 1.24x faster                                                            |
| xml_etree_iterparse  | 77.6 ms                                                         | 67.8 ms: 1.14x faster                                                            |
| json_dumps           | 7.40 ms                                                         | 6.84 ms: 1.08x faster                                                            |
| unpickle_list        | 2.95 us                                                         | 2.82 us: 1.05x faster                                                            |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                             |
| json_loads           | 20.4 us                                                         | 20.1 us: 1.01x faster                                                            |
| pickle_dict          | 19.9 us                                                         | 19.7 us: 1.01x faster                                                            |
| pickle               | 7.79 us                                                         | 8.00 us: 1.03x slower                                                            |
| unpickle             | 9.71 us                                                         | 10.1 us: 1.04x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.12x faster                                                                     |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 19.1 ms                                                         | 20.2 ms: 1.06x slower                                                            |
| Geometric mean         | (ref)                                                           | 1.03x slower                                                                     |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.60 ms: 1.31x faster                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 22.5 ms: 1.71x faster                                                            |
| logging_silent             | 101 ns                                                          | 61.0 ns: 1.66x faster                                                            |
| deepcopy_memo              | 38.4 us                                                         | 23.6 us: 1.63x faster                                                            |
| scimark_sor                | 130 ms                                                          | 83.5 ms: 1.55x faster                                                            |
| scimark_lu                 | 93.2 ms                                                         | 60.5 ms: 1.54x faster                                                            |
| unpack_sequence            | 62.5 ns                                                         | 41.3 ns: 1.51x faster                                                            |
| deltablue                  | 3.58 ms                                                         | 2.37 ms: 1.51x faster                                                            |
| richards                   | 41.3 ms                                                         | 28.5 ms: 1.45x faster                                                            |
| coroutines                 | 20.9 ms                                                         | 14.4 ms: 1.45x faster                                                            |
| float                      | 76.7 ms                                                         | 53.8 ms: 1.42x faster                                                            |
| richards_super             | 46.5 ms                                                         | 33.5 ms: 1.39x faster                                                            |
| raytrace                   | 308 ms                                                          | 224 ms: 1.38x faster                                                             |
| spectral_norm              | 104 ms                                                          | 75.5 ms: 1.38x faster                                                            |
| tomli_loads                | 2.20 sec                                                        | 1.60 sec: 1.37x faster                                                           |
| pickle_pure_python         | 286 us                                                          | 210 us: 1.36x faster                                                             |
| nbody                      | 127 ms                                                          | 93.5 ms: 1.36x faster                                                            |
| unpickle_pure_python       | 210 us                                                          | 155 us: 1.36x faster                                                             |
| sqlglot_parse              | 1.25 ms                                                         | 920 us: 1.36x faster                                                             |
| typing_runtime_protocols   | 126 us                                                          | 94.9 us: 1.33x faster                                                            |
| deepcopy_reduce            | 3.23 us                                                         | 2.43 us: 1.33x faster                                                            |
| sqlglot_transpile          | 1.53 ms                                                         | 1.16 ms: 1.32x faster                                                            |
| chameleon                  | 7.75 ms                                                         | 5.91 ms: 1.31x faster                                                            |
| mako                       | 9.96 ms                                                         | 7.60 ms: 1.31x faster                                                            |
| deepcopy                   | 360 us                                                          | 277 us: 1.30x faster                                                             |
| comprehensions             | 19.2 us                                                         | 15.0 us: 1.28x faster                                                            |
| xml_etree_process          | 53.2 ms                                                         | 41.5 ms: 1.28x faster                                                            |
| regex_compile              | 129 ms                                                          | 103 ms: 1.25x faster                                                             |
| xml_etree_generate         | 72.1 ms                                                         | 58.4 ms: 1.24x faster                                                            |
| logging_simple             | 9.75 us                                                         | 8.01 us: 1.22x faster                                                            |
| logging_format             | 10.4 us                                                         | 8.60 us: 1.21x faster                                                            |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.22 ms: 1.20x faster                                                            |
| pycparser                  | 978 ms                                                          | 821 ms: 1.19x faster                                                             |
| async_tree_none            | 298 ms                                                          | 250 ms: 1.19x faster                                                             |
| go                         | 137 ms                                                          | 116 ms: 1.19x faster                                                             |
| chaos                      | 69.4 ms                                                         | 58.5 ms: 1.19x faster                                                            |
| async_tree_none_tg         | 278 ms                                                          | 239 ms: 1.16x faster                                                             |
| async_tree_memoization_tg  | 350 ms                                                          | 302 ms: 1.16x faster                                                             |
| async_tree_memoization     | 364 ms                                                          | 313 ms: 1.16x faster                                                             |
| async_tree_io              | 693 ms                                                          | 601 ms: 1.15x faster                                                             |
| sqlglot_optimize           | 48.5 ms                                                         | 42.1 ms: 1.15x faster                                                            |
| async_tree_io_tg           | 677 ms                                                          | 590 ms: 1.15x faster                                                             |
| xml_etree_iterparse        | 77.6 ms                                                         | 67.8 ms: 1.14x faster                                                            |
| pyflate                    | 424 ms                                                          | 372 ms: 1.14x faster                                                             |
| 2to3                       | 280 ms                                                          | 247 ms: 1.13x faster                                                             |
| async_generators           | 313 ms                                                          | 277 ms: 1.13x faster                                                             |
| crypto_pyaes               | 69.2 ms                                                         | 61.4 ms: 1.13x faster                                                            |
| docutils                   | 1.98 sec                                                        | 1.77 sec: 1.12x faster                                                           |
| sympy_str                  | 240 ms                                                          | 213 ms: 1.12x faster                                                             |
| sympy_integrate            | 17.5 ms                                                         | 15.6 ms: 1.12x faster                                                            |
| fannkuch                   | 354 ms                                                          | 315 ms: 1.12x faster                                                             |
| sympy_sum                  | 123 ms                                                          | 110 ms: 1.12x faster                                                             |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 510 ms: 1.10x faster                                                             |
| sqlite_synth               | 2.07 us                                                         | 1.89 us: 1.09x faster                                                            |
| bench_thread_pool          | 1.10 ms                                                         | 1.01 ms: 1.09x faster                                                            |
| dask                       | 323 ms                                                          | 296 ms: 1.09x faster                                                             |
| tornado_http               | 105 ms                                                          | 96.4 ms: 1.09x faster                                                            |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 501 ms: 1.09x faster                                                             |
| sympy_expand               | 398 ms                                                          | 366 ms: 1.09x faster                                                             |
| pathlib                    | 91.4 ms                                                         | 84.1 ms: 1.09x faster                                                            |
| hexiom                     | 6.82 ms                                                         | 6.30 ms: 1.08x faster                                                            |
| pprint_pformat             | 1.50 sec                                                        | 1.39 sec: 1.08x faster                                                           |
| json_dumps                 | 7.40 ms                                                         | 6.84 ms: 1.08x faster                                                            |
| scimark_fft                | 271 ms                                                          | 251 ms: 1.08x faster                                                             |
| pprint_safe_repr           | 721 ms                                                          | 670 ms: 1.08x faster                                                             |
| regex_effbot               | 2.04 ms                                                         | 1.91 ms: 1.07x faster                                                            |
| bench_mp_pool              | 75.4 ms                                                         | 70.7 ms: 1.07x faster                                                            |
| meteor_contest             | 86.9 ms                                                         | 82.0 ms: 1.06x faster                                                            |
| asyncio_tcp                | 662 ms                                                          | 627 ms: 1.06x faster                                                             |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.9 sec: 1.05x faster                                                           |
| unpickle_list              | 2.95 us                                                         | 2.82 us: 1.05x faster                                                            |
| gc_traversal               | 1.44 ms                                                         | 1.38 ms: 1.04x faster                                                            |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                             |
| regex_dna                  | 127 ms                                                          | 123 ms: 1.03x faster                                                             |
| mdp                        | 1.91 sec                                                        | 1.86 sec: 1.03x faster                                                           |
| nqueens                    | 93.7 ms                                                         | 91.6 ms: 1.02x faster                                                            |
| json_loads                 | 20.4 us                                                         | 20.1 us: 1.01x faster                                                            |
| pickle_dict                | 19.9 us                                                         | 19.7 us: 1.01x faster                                                            |
| pidigits                   | 199 ms                                                          | 201 ms: 1.01x slower                                                             |
| json                       | 4.15 ms                                                         | 4.19 ms: 1.01x slower                                                            |
| pickle                     | 7.79 us                                                         | 8.00 us: 1.03x slower                                                            |
| scimark_monte_carlo        | 66.4 ms                                                         | 68.3 ms: 1.03x slower                                                            |
| unpickle                   | 9.71 us                                                         | 10.1 us: 1.04x slower                                                            |
| python_startup_no_site     | 19.1 ms                                                         | 20.2 ms: 1.06x slower                                                            |
| regex_v8                   | 15.0 ms                                                         | 16.1 ms: 1.07x slower                                                            |
| telco                      | 5.51 ms                                                         | 6.56 ms: 1.19x slower                                                            |
| sqlglot_normalize          | 100 ms                                                          | 215 ms: 2.15x slower                                                             |
| coverage                   | 48.4 ms                                                         | 467 ms: 9.64x slower                                                             |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                                     |

Benchmark hidden because not significant (3): create_gc_cycles, python_startup, pickle_list
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown