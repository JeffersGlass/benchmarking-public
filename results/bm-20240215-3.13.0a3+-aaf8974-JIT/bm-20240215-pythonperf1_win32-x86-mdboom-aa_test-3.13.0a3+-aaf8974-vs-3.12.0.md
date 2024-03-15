
# Results vs. 3.12.0

- fork: mdboom
- ref: aa_test
- machine: windows-x86
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.11x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 252 ms: 1.11x faster                                               |
| chameleon      | 7.75 ms                                                         | 5.83 ms: 1.33x faster                                              |
| docutils       | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                             |
| tornado_http   | 105 ms                                                          | 98.6 ms: 1.06x faster                                              |
| Geometric mean | (ref)                                                           | 1.15x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 255 ms: 1.17x faster                                               |
| async_tree_memoization_tg  | 350 ms                                                          | 301 ms: 1.16x faster                                               |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                               |
| async_tree_memoization     | 364 ms                                                          | 317 ms: 1.15x faster                                               |
| async_tree_io_tg           | 677 ms                                                          | 597 ms: 1.13x faster                                               |
| async_tree_io              | 693 ms                                                          | 615 ms: 1.13x faster                                               |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 517 ms: 1.09x faster                                               |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 503 ms: 1.09x faster                                               |
| Geometric mean             | (ref)                                                           | 1.13x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 127 ms                                                          | 88.6 ms: 1.43x faster                                              |
| float          | 76.7 ms                                                         | 54.0 ms: 1.42x faster                                              |
| Geometric mean | (ref)                                                           | 1.27x faster                                                       |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 108 ms: 1.19x faster                                               |
| regex_effbot   | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                              |
| regex_dna      | 127 ms                                                          | 122 ms: 1.04x faster                                               |
| regex_v8       | 15.0 ms                                                         | 15.8 ms: 1.05x slower                                              |
| Geometric mean | (ref)                                                           | 1.06x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| unpickle_pure_python | 210 us                                                          | 158 us: 1.33x faster                                               |
| tomli_loads          | 2.20 sec                                                        | 1.67 sec: 1.31x faster                                             |
| pickle_pure_python   | 286 us                                                          | 222 us: 1.29x faster                                               |
| xml_etree_process    | 53.2 ms                                                         | 42.6 ms: 1.25x faster                                              |
| xml_etree_generate   | 72.1 ms                                                         | 61.1 ms: 1.18x faster                                              |
| xml_etree_iterparse  | 77.6 ms                                                         | 66.6 ms: 1.17x faster                                              |
| json_dumps           | 7.40 ms                                                         | 6.96 ms: 1.06x faster                                              |
| pickle_list          | 3.37 us                                                         | 3.18 us: 1.06x faster                                              |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                               |
| json_loads           | 20.4 us                                                         | 20.0 us: 1.02x faster                                              |
| pickle               | 7.79 us                                                         | 8.07 us: 1.04x slower                                              |
| unpickle             | 9.71 us                                                         | 10.1 us: 1.04x slower                                              |
| unpickle_list        | 2.95 us                                                         | 3.13 us: 1.06x slower                                              |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                       |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 22.9 ms: 1.02x slower                                              |
| python_startup_no_site | 19.1 ms                                                         | 20.8 ms: 1.09x slower                                              |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 9.96 ms                                                         | 7.44 ms: 1.34x faster                                              |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 24.5 ms: 1.57x faster                                              |
| deepcopy_memo              | 38.4 us                                                         | 25.7 us: 1.50x faster                                              |
| logging_silent             | 101 ns                                                          | 67.8 ns: 1.49x faster                                              |
| scimark_sor                | 130 ms                                                          | 88.3 ms: 1.47x faster                                              |
| nbody                      | 127 ms                                                          | 88.6 ms: 1.43x faster                                              |
| float                      | 76.7 ms                                                         | 54.0 ms: 1.42x faster                                              |
| coroutines                 | 20.9 ms                                                         | 14.8 ms: 1.41x faster                                              |
| deltablue                  | 3.58 ms                                                         | 2.55 ms: 1.40x faster                                              |
| spectral_norm              | 104 ms                                                          | 74.1 ms: 1.40x faster                                              |
| scimark_lu                 | 93.2 ms                                                         | 68.2 ms: 1.37x faster                                              |
| comprehensions             | 19.2 us                                                         | 14.1 us: 1.36x faster                                              |
| unpack_sequence            | 62.5 ns                                                         | 46.5 ns: 1.34x faster                                              |
| richards                   | 41.3 ms                                                         | 30.9 ms: 1.34x faster                                              |
| mako                       | 9.96 ms                                                         | 7.44 ms: 1.34x faster                                              |
| unpickle_pure_python       | 210 us                                                          | 158 us: 1.33x faster                                               |
| deepcopy_reduce            | 3.23 us                                                         | 2.43 us: 1.33x faster                                              |
| chameleon                  | 7.75 ms                                                         | 5.83 ms: 1.33x faster                                              |
| tomli_loads                | 2.20 sec                                                        | 1.67 sec: 1.31x faster                                             |
| richards_super             | 46.5 ms                                                         | 35.5 ms: 1.31x faster                                              |
| sqlglot_parse              | 1.25 ms                                                         | 961 us: 1.30x faster                                               |
| raytrace                   | 308 ms                                                          | 238 ms: 1.29x faster                                               |
| pickle_pure_python         | 286 us                                                          | 222 us: 1.29x faster                                               |
| typing_runtime_protocols   | 126 us                                                          | 98.6 us: 1.28x faster                                              |
| sqlglot_transpile          | 1.53 ms                                                         | 1.21 ms: 1.26x faster                                              |
| deepcopy                   | 360 us                                                          | 286 us: 1.26x faster                                               |
| xml_etree_process          | 53.2 ms                                                         | 42.6 ms: 1.25x faster                                              |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.11 ms: 1.24x faster                                              |
| regex_compile              | 129 ms                                                          | 108 ms: 1.19x faster                                               |
| xml_etree_generate         | 72.1 ms                                                         | 61.1 ms: 1.18x faster                                              |
| xml_etree_iterparse        | 77.6 ms                                                         | 66.6 ms: 1.17x faster                                              |
| async_tree_none            | 298 ms                                                          | 255 ms: 1.17x faster                                               |
| async_tree_memoization_tg  | 350 ms                                                          | 301 ms: 1.16x faster                                               |
| logging_simple             | 9.75 us                                                         | 8.42 us: 1.16x faster                                              |
| chaos                      | 69.4 ms                                                         | 60.2 ms: 1.15x faster                                              |
| async_tree_none_tg         | 278 ms                                                          | 241 ms: 1.15x faster                                               |
| go                         | 137 ms                                                          | 120 ms: 1.15x faster                                               |
| logging_format             | 10.4 us                                                         | 9.07 us: 1.15x faster                                              |
| async_tree_memoization     | 364 ms                                                          | 317 ms: 1.15x faster                                               |
| async_tree_io_tg           | 677 ms                                                          | 597 ms: 1.13x faster                                               |
| crypto_pyaes               | 69.2 ms                                                         | 61.4 ms: 1.13x faster                                              |
| async_tree_io              | 693 ms                                                          | 615 ms: 1.13x faster                                               |
| scimark_fft                | 271 ms                                                          | 241 ms: 1.13x faster                                               |
| fannkuch                   | 354 ms                                                          | 315 ms: 1.12x faster                                               |
| pycparser                  | 978 ms                                                          | 872 ms: 1.12x faster                                               |
| pyflate                    | 424 ms                                                          | 379 ms: 1.12x faster                                               |
| sympy_integrate            | 17.5 ms                                                         | 15.7 ms: 1.12x faster                                              |
| sqlglot_optimize           | 48.5 ms                                                         | 43.5 ms: 1.11x faster                                              |
| sympy_sum                  | 123 ms                                                          | 110 ms: 1.11x faster                                               |
| 2to3                       | 280 ms                                                          | 252 ms: 1.11x faster                                               |
| sympy_str                  | 240 ms                                                          | 216 ms: 1.11x faster                                               |
| sqlite_synth               | 2.07 us                                                         | 1.87 us: 1.11x faster                                              |
| docutils                   | 1.98 sec                                                        | 1.81 sec: 1.10x faster                                             |
| pathlib                    | 91.4 ms                                                         | 83.6 ms: 1.09x faster                                              |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 517 ms: 1.09x faster                                               |
| bench_thread_pool          | 1.10 ms                                                         | 1.01 ms: 1.09x faster                                              |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 503 ms: 1.09x faster                                               |
| regex_effbot               | 2.04 ms                                                         | 1.89 ms: 1.08x faster                                              |
| async_generators           | 313 ms                                                          | 291 ms: 1.08x faster                                               |
| asyncio_tcp                | 662 ms                                                          | 615 ms: 1.08x faster                                               |
| nqueens                    | 93.7 ms                                                         | 87.8 ms: 1.07x faster                                              |
| tornado_http               | 105 ms                                                          | 98.6 ms: 1.06x faster                                              |
| json_dumps                 | 7.40 ms                                                         | 6.96 ms: 1.06x faster                                              |
| dask                       | 323 ms                                                          | 305 ms: 1.06x faster                                               |
| pickle_list                | 3.37 us                                                         | 3.18 us: 1.06x faster                                              |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.7 sec: 1.06x faster                                             |
| sympy_expand               | 398 ms                                                          | 379 ms: 1.05x faster                                               |
| pprint_pformat             | 1.50 sec                                                        | 1.43 sec: 1.04x faster                                             |
| regex_dna                  | 127 ms                                                          | 122 ms: 1.04x faster                                               |
| gc_traversal               | 1.44 ms                                                         | 1.38 ms: 1.04x faster                                              |
| hexiom                     | 6.82 ms                                                         | 6.54 ms: 1.04x faster                                              |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                               |
| mdp                        | 1.91 sec                                                        | 1.84 sec: 1.04x faster                                             |
| pprint_safe_repr           | 721 ms                                                          | 700 ms: 1.03x faster                                               |
| meteor_contest             | 86.9 ms                                                         | 84.6 ms: 1.03x faster                                              |
| json_loads                 | 20.4 us                                                         | 20.0 us: 1.02x faster                                              |
| bench_mp_pool              | 75.4 ms                                                         | 74.7 ms: 1.01x faster                                              |
| json                       | 4.15 ms                                                         | 4.19 ms: 1.01x slower                                              |
| python_startup             | 22.4 ms                                                         | 22.9 ms: 1.02x slower                                              |
| pickle                     | 7.79 us                                                         | 8.07 us: 1.04x slower                                              |
| unpickle                   | 9.71 us                                                         | 10.1 us: 1.04x slower                                              |
| scimark_monte_carlo        | 66.4 ms                                                         | 69.3 ms: 1.04x slower                                              |
| regex_v8                   | 15.0 ms                                                         | 15.8 ms: 1.05x slower                                              |
| unpickle_list              | 2.95 us                                                         | 3.13 us: 1.06x slower                                              |
| python_startup_no_site     | 19.1 ms                                                         | 20.8 ms: 1.09x slower                                              |
| telco                      | 5.51 ms                                                         | 6.35 ms: 1.15x slower                                              |
| sqlglot_normalize          | 100 ms                                                          | 221 ms: 2.21x slower                                               |
| coverage                   | 48.4 ms                                                         | 474 ms: 9.79x slower                                               |
| Geometric mean             | (ref)                                                           | 1.11x faster                                                       |

Benchmark hidden because not significant (3): pidigits, create_gc_cycles, pickle_dict
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown