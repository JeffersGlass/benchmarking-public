
# Results vs. 3.12.0

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 300 ms: 1.05x slower                                            |
| tornado_http   | 121 ms                                                       | 124 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                        | 1.02x slower                                                    |

Benchmark hidden because not significant (2): chameleon, docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 438 ms: 1.03x faster                                            |
| async_tree_memoization     | 544 ms                                                       | 548 ms: 1.01x slower                                            |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 706 ms: 1.01x slower                                            |
| async_tree_memoization_tg  | 540 ms                                                       | 552 ms: 1.02x slower                                            |
| async_tree_none_tg         | 431 ms                                                       | 441 ms: 1.02x slower                                            |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                          |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                          |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                    |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                            |
| float          | 76.6 ms                                                      | 81.2 ms: 1.06x slower                                           |
| nbody          | 88.0 ms                                                      | 107 ms: 1.22x slower                                            |
| Geometric mean | (ref)                                                        | 1.08x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 144 ms                                                       | 145 ms: 1.00x slower                                            |
| regex_dna      | 239 ms                                                       | 244 ms: 1.02x slower                                            |
| regex_v8       | 23.6 ms                                                      | 25.2 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                        | 1.02x slower                                                    |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 306 us: 1.04x faster                                            |
| xml_etree_generate   | 86.1 ms                                                      | 84.9 ms: 1.01x faster                                           |
| pickle_list          | 4.43 us                                                      | 4.38 us: 1.01x faster                                           |
| pickle_dict          | 32.5 us                                                      | 32.7 us: 1.00x slower                                           |
| pickle               | 10.5 us                                                      | 10.6 us: 1.01x slower                                           |
| unpickle             | 14.8 us                                                      | 15.0 us: 1.01x slower                                           |
| unpickle_list        | 4.66 us                                                      | 4.72 us: 1.01x slower                                           |
| xml_etree_iterparse  | 103 ms                                                       | 106 ms: 1.03x slower                                            |
| json_loads           | 24.4 us                                                      | 25.1 us: 1.03x slower                                           |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                           |
| xml_etree_parse      | 144 ms                                                       | 150 ms: 1.04x slower                                            |
| tomli_loads          | 2.16 sec                                                     | 2.29 sec: 1.06x slower                                          |
| unpickle_pure_python | 210 us                                                       | 227 us: 1.09x slower                                            |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                    |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                           |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                           |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 11.7 ms: 1.17x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpack_sequence            | 53.2 ns                                                      | 41.2 ns: 1.29x faster                                           |
| typing_runtime_protocols   | 152 us                                                       | 119 us: 1.28x faster                                            |
| comprehensions             | 21.9 us                                                      | 19.4 us: 1.13x faster                                           |
| generators                 | 37.4 ms                                                      | 33.5 ms: 1.12x faster                                           |
| async_generators           | 390 ms                                                       | 363 ms: 1.08x faster                                            |
| raytrace                   | 298 ms                                                       | 280 ms: 1.06x faster                                            |
| create_gc_cycles           | 1.59 ms                                                      | 1.52 ms: 1.05x faster                                           |
| logging_format             | 7.48 us                                                      | 7.18 us: 1.04x faster                                           |
| pickle_pure_python         | 318 us                                                       | 306 us: 1.04x faster                                            |
| async_tree_none            | 452 ms                                                       | 438 ms: 1.03x faster                                            |
| logging_simple             | 6.71 us                                                      | 6.55 us: 1.02x faster                                           |
| sympy_sum                  | 162 ms                                                       | 158 ms: 1.02x faster                                            |
| coroutines                 | 23.0 ms                                                      | 22.5 ms: 1.02x faster                                           |
| xml_etree_generate         | 86.1 ms                                                      | 84.9 ms: 1.01x faster                                           |
| gc_traversal               | 3.48 ms                                                      | 3.43 ms: 1.01x faster                                           |
| asyncio_tcp                | 378 ms                                                       | 373 ms: 1.01x faster                                            |
| pickle_list                | 4.43 us                                                      | 4.38 us: 1.01x faster                                           |
| sqlite_synth               | 2.77 us                                                      | 2.74 us: 1.01x faster                                           |
| sympy_str                  | 302 ms                                                       | 299 ms: 1.01x faster                                            |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                            |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                          |
| crypto_pyaes               | 80.3 ms                                                      | 79.9 ms: 1.01x faster                                           |
| sympy_integrate            | 23.9 ms                                                      | 23.8 ms: 1.01x faster                                           |
| deepcopy_memo              | 36.8 us                                                      | 36.6 us: 1.01x faster                                           |
| mdp                        | 2.57 sec                                                     | 2.56 sec: 1.00x faster                                          |
| pathlib                    | 18.9 ms                                                      | 18.9 ms: 1.00x slower                                           |
| pickle_dict                | 32.5 us                                                      | 32.7 us: 1.00x slower                                           |
| regex_compile              | 144 ms                                                       | 145 ms: 1.00x slower                                            |
| deepcopy                   | 368 us                                                       | 370 us: 1.00x slower                                            |
| async_tree_memoization     | 544 ms                                                       | 548 ms: 1.01x slower                                            |
| pickle                     | 10.5 us                                                      | 10.6 us: 1.01x slower                                           |
| unpickle                   | 14.8 us                                                      | 15.0 us: 1.01x slower                                           |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 706 ms: 1.01x slower                                            |
| unpickle_list              | 4.66 us                                                      | 4.72 us: 1.01x slower                                           |
| meteor_contest             | 128 ms                                                       | 130 ms: 1.01x slower                                            |
| sqlglot_normalize          | 116 ms                                                       | 118 ms: 1.02x slower                                            |
| regex_dna                  | 239 ms                                                       | 244 ms: 1.02x slower                                            |
| sqlglot_parse              | 1.38 ms                                                      | 1.41 ms: 1.02x slower                                           |
| async_tree_memoization_tg  | 540 ms                                                       | 552 ms: 1.02x slower                                            |
| logging_silent             | 94.4 ns                                                      | 96.7 ns: 1.02x slower                                           |
| async_tree_none_tg         | 431 ms                                                       | 441 ms: 1.02x slower                                            |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                          |
| tornado_http               | 121 ms                                                       | 124 ms: 1.03x slower                                            |
| sqlglot_transpile          | 1.78 ms                                                      | 1.82 ms: 1.03x slower                                           |
| xml_etree_iterparse        | 103 ms                                                       | 106 ms: 1.03x slower                                            |
| json_loads                 | 24.4 us                                                      | 25.1 us: 1.03x slower                                           |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                          |
| json                       | 5.12 ms                                                      | 5.29 ms: 1.03x slower                                           |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                           |
| bench_thread_pool          | 950 us                                                       | 986 us: 1.04x slower                                            |
| dask                       | 392 ms                                                       | 409 ms: 1.04x slower                                            |
| xml_etree_parse            | 144 ms                                                       | 150 ms: 1.04x slower                                            |
| sympy_expand               | 484 ms                                                       | 506 ms: 1.04x slower                                            |
| pprint_pformat             | 1.65 sec                                                     | 1.74 sec: 1.05x slower                                          |
| pprint_safe_repr           | 807 ms                                                       | 848 ms: 1.05x slower                                            |
| 2to3                       | 285 ms                                                       | 300 ms: 1.05x slower                                            |
| sqlglot_optimize           | 57.5 ms                                                      | 60.6 ms: 1.05x slower                                           |
| float                      | 76.6 ms                                                      | 81.2 ms: 1.06x slower                                           |
| tomli_loads                | 2.16 sec                                                     | 2.29 sec: 1.06x slower                                          |
| dulwich_log                | 65.4 ms                                                      | 69.4 ms: 1.06x slower                                           |
| pycparser                  | 1.23 sec                                                     | 1.31 sec: 1.06x slower                                          |
| nqueens                    | 89.9 ms                                                      | 95.7 ms: 1.06x slower                                           |
| regex_v8                   | 23.6 ms                                                      | 25.2 ms: 1.07x slower                                           |
| unpickle_pure_python       | 210 us                                                       | 227 us: 1.09x slower                                            |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                           |
| chaos                      | 64.0 ms                                                      | 69.8 ms: 1.09x slower                                           |
| richards                   | 45.7 ms                                                      | 50.3 ms: 1.10x slower                                           |
| richards_super             | 51.3 ms                                                      | 56.5 ms: 1.10x slower                                           |
| go                         | 150 ms                                                       | 166 ms: 1.11x slower                                            |
| scimark_monte_carlo        | 69.0 ms                                                      | 76.6 ms: 1.11x slower                                           |
| scimark_fft                | 301 ms                                                       | 348 ms: 1.16x slower                                            |
| coverage                   | 66.7 ms                                                      | 77.6 ms: 1.16x slower                                           |
| deltablue                  | 3.24 ms                                                      | 3.78 ms: 1.17x slower                                           |
| mako                       | 10.0 ms                                                      | 11.7 ms: 1.17x slower                                           |
| telco                      | 6.96 ms                                                      | 8.17 ms: 1.17x slower                                           |
| fannkuch                   | 350 ms                                                       | 412 ms: 1.18x slower                                            |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 5.01 ms: 1.19x slower                                           |
| nbody                      | 88.0 ms                                                      | 107 ms: 1.22x slower                                            |
| spectral_norm              | 91.6 ms                                                      | 113 ms: 1.24x slower                                            |
| pyflate                    | 439 ms                                                       | 546 ms: 1.24x slower                                            |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                           |
| hexiom                     | 5.96 ms                                                      | 7.66 ms: 1.28x slower                                           |
| scimark_sor                | 109 ms                                                       | 141 ms: 1.30x slower                                            |
| Geometric mean             | (ref)                                                        | 1.04x slower                                                    |

Benchmark hidden because not significant (10): deepcopy_reduce, xml_etree_process, chameleon, regex_effbot, docutils, bench_mp_pool, async_tree_cpu_io_mixed, scimark_lu, asyncio_websockets, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.92x