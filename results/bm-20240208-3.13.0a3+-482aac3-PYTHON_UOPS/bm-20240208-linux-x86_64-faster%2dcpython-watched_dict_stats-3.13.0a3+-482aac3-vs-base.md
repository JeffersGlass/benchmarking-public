# Results vs. base

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 482aac3
- commit date: 2024-02-08
- overall geometric mean: 1.03x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                                 | 287 ms: 1.02x slower                                                           |
| chameleon      | 7.28 ms                                                                | 7.39 ms: 1.01x slower                                                          |
| docutils       | 2.70 sec                                                               | 2.71 sec: 1.00x slower                                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none_tg         | 454 ms                                                                 | 461 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed    | 717 ms                                                                 | 728 ms: 1.02x slower                                                           |
| async_tree_cpu_io_mixed_tg | 724 ms                                                                 | 738 ms: 1.02x slower                                                           |
| async_tree_io_tg           | 1.20 sec                                                               | 1.22 sec: 1.02x slower                                                         |
| async_tree_io              | 1.18 sec                                                               | 1.21 sec: 1.02x slower                                                         |
| async_tree_none            | 445 ms                                                                 | 455 ms: 1.02x slower                                                           |
| async_tree_memoization     | 571 ms                                                                 | 585 ms: 1.02x slower                                                           |
| async_tree_memoization_tg  | 588 ms                                                                 | 608 ms: 1.03x slower                                                           |
| Geometric mean             | (ref)                                                                  | 1.02x slower                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 189 ms: 1.00x slower                                                           |
| float          | 89.7 ms                                                                | 101 ms: 1.13x slower                                                           |
| nbody          | 112 ms                                                                 | 129 ms: 1.15x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.09x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_effbot   | 3.62 ms                                                                | 3.63 ms: 1.00x slower                                                          |
| regex_dna      | 221 ms                                                                 | 226 ms: 1.02x slower                                                           |
| regex_v8       | 24.2 ms                                                                | 25.3 ms: 1.05x slower                                                          |
| regex_compile  | 148 ms                                                                 | 156 ms: 1.05x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_dict          | 36.3 us                                                                | 33.8 us: 1.07x faster                                                          |
| unpickle             | 16.4 us                                                                | 15.4 us: 1.07x faster                                                          |
| pickle               | 11.9 us                                                                | 11.8 us: 1.01x faster                                                          |
| pickle_pure_python   | 297 us                                                                 | 301 us: 1.01x slower                                                           |
| pickle_list          | 5.12 us                                                                | 5.20 us: 1.01x slower                                                          |
| xml_etree_process    | 60.2 ms                                                                | 61.6 ms: 1.02x slower                                                          |
| unpickle_pure_python | 232 us                                                                 | 237 us: 1.02x slower                                                           |
| xml_etree_generate   | 88.3 ms                                                                | 90.3 ms: 1.02x slower                                                          |
| unpickle_list        | 4.86 us                                                                | 4.98 us: 1.02x slower                                                          |
| xml_etree_iterparse  | 109 ms                                                                 | 113 ms: 1.04x slower                                                           |
| tomli_loads          | 2.52 sec                                                               | 2.80 sec: 1.11x slower                                                         |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (3): json_loads, json_dumps, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                          |
| python_startup_no_site | 8.78 ms                                                                | 8.76 ms: 1.00x faster                                                          |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|-----------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 13.1 ms                                                                | 15.2 ms: 1.16x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| unpack_sequence            | 52.9 ns                                                                | 45.0 ns: 1.18x faster                                                          |
| pickle_dict                | 36.3 us                                                                | 33.8 us: 1.07x faster                                                          |
| unpickle                   | 16.4 us                                                                | 15.4 us: 1.07x faster                                                          |
| pickle                     | 11.9 us                                                                | 11.8 us: 1.01x faster                                                          |
| python_startup             | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                          |
| python_startup_no_site     | 8.78 ms                                                                | 8.76 ms: 1.00x faster                                                          |
| asyncio_tcp                | 488 ms                                                                 | 489 ms: 1.00x slower                                                           |
| docutils                   | 2.70 sec                                                               | 2.71 sec: 1.00x slower                                                         |
| regex_effbot               | 3.62 ms                                                                | 3.63 ms: 1.00x slower                                                          |
| deepcopy                   | 352 us                                                                 | 354 us: 1.00x slower                                                           |
| pidigits                   | 188 ms                                                                 | 189 ms: 1.00x slower                                                           |
| coverage                   | 94.4 ms                                                                | 94.9 ms: 1.01x slower                                                          |
| deepcopy_reduce            | 3.12 us                                                                | 3.13 us: 1.01x slower                                                          |
| sympy_expand               | 492 ms                                                                 | 495 ms: 1.01x slower                                                           |
| telco                      | 8.72 ms                                                                | 8.82 ms: 1.01x slower                                                          |
| logging_simple             | 5.97 us                                                                | 6.04 us: 1.01x slower                                                          |
| pickle_pure_python         | 297 us                                                                 | 301 us: 1.01x slower                                                           |
| json                       | 5.09 ms                                                                | 5.16 ms: 1.01x slower                                                          |
| pickle_list                | 5.12 us                                                                | 5.20 us: 1.01x slower                                                          |
| chameleon                  | 7.28 ms                                                                | 7.39 ms: 1.01x slower                                                          |
| async_tree_none_tg         | 454 ms                                                                 | 461 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed    | 717 ms                                                                 | 728 ms: 1.02x slower                                                           |
| bench_thread_pool          | 844 us                                                                 | 858 us: 1.02x slower                                                           |
| mdp                        | 2.62 sec                                                               | 2.67 sec: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 724 ms                                                                 | 738 ms: 1.02x slower                                                           |
| coroutines                 | 22.2 ms                                                                | 22.6 ms: 1.02x slower                                                          |
| async_tree_io_tg           | 1.20 sec                                                               | 1.22 sec: 1.02x slower                                                         |
| async_tree_io              | 1.18 sec                                                               | 1.21 sec: 1.02x slower                                                         |
| go                         | 173 ms                                                                 | 177 ms: 1.02x slower                                                           |
| regex_dna                  | 221 ms                                                                 | 226 ms: 1.02x slower                                                           |
| xml_etree_process          | 60.2 ms                                                                | 61.6 ms: 1.02x slower                                                          |
| unpickle_pure_python       | 232 us                                                                 | 237 us: 1.02x slower                                                           |
| xml_etree_generate         | 88.3 ms                                                                | 90.3 ms: 1.02x slower                                                          |
| async_tree_none            | 445 ms                                                                 | 455 ms: 1.02x slower                                                           |
| 2to3                       | 280 ms                                                                 | 287 ms: 1.02x slower                                                           |
| unpickle_list              | 4.86 us                                                                | 4.98 us: 1.02x slower                                                          |
| sympy_str                  | 292 ms                                                                 | 299 ms: 1.02x slower                                                           |
| async_tree_memoization     | 571 ms                                                                 | 585 ms: 1.02x slower                                                           |
| pycparser                  | 1.20 sec                                                               | 1.23 sec: 1.02x slower                                                         |
| sympy_integrate            | 21.1 ms                                                                | 21.7 ms: 1.02x slower                                                          |
| sqlglot_parse              | 1.33 ms                                                                | 1.36 ms: 1.03x slower                                                          |
| sympy_sum                  | 161 ms                                                                 | 166 ms: 1.03x slower                                                           |
| sqlglot_transpile          | 1.66 ms                                                                | 1.70 ms: 1.03x slower                                                          |
| deepcopy_memo              | 39.3 us                                                                | 40.7 us: 1.03x slower                                                          |
| async_tree_memoization_tg  | 588 ms                                                                 | 608 ms: 1.03x slower                                                           |
| sqlglot_optimize           | 57.6 ms                                                                | 59.6 ms: 1.04x slower                                                          |
| sqlglot_normalize          | 114 ms                                                                 | 118 ms: 1.04x slower                                                           |
| xml_etree_iterparse        | 109 ms                                                                 | 113 ms: 1.04x slower                                                           |
| pprint_pformat             | 1.67 sec                                                               | 1.74 sec: 1.04x slower                                                         |
| regex_v8                   | 24.2 ms                                                                | 25.3 ms: 1.05x slower                                                          |
| meteor_contest             | 112 ms                                                                 | 117 ms: 1.05x slower                                                           |
| richards_super             | 54.4 ms                                                                | 57.1 ms: 1.05x slower                                                          |
| pprint_safe_repr           | 802 ms                                                                 | 842 ms: 1.05x slower                                                           |
| raytrace                   | 295 ms                                                                 | 310 ms: 1.05x slower                                                           |
| logging_silent             | 99.6 ns                                                                | 105 ns: 1.05x slower                                                           |
| regex_compile              | 148 ms                                                                 | 156 ms: 1.05x slower                                                           |
| scimark_lu                 | 113 ms                                                                 | 119 ms: 1.05x slower                                                           |
| gc_traversal               | 3.49 ms                                                                | 3.70 ms: 1.06x slower                                                          |
| richards                   | 48.1 ms                                                                | 51.0 ms: 1.06x slower                                                          |
| deltablue                  | 3.46 ms                                                                | 3.69 ms: 1.07x slower                                                          |
| pyflate                    | 511 ms                                                                 | 553 ms: 1.08x slower                                                           |
| chaos                      | 71.3 ms                                                                | 77.8 ms: 1.09x slower                                                          |
| scimark_fft                | 431 ms                                                                 | 475 ms: 1.10x slower                                                           |
| tomli_loads                | 2.52 sec                                                               | 2.80 sec: 1.11x slower                                                         |
| crypto_pyaes               | 82.8 ms                                                                | 92.1 ms: 1.11x slower                                                          |
| fannkuch                   | 428 ms                                                                 | 476 ms: 1.11x slower                                                           |
| scimark_monte_carlo        | 78.5 ms                                                                | 88.3 ms: 1.13x slower                                                          |
| float                      | 89.7 ms                                                                | 101 ms: 1.13x slower                                                           |
| nqueens                    | 92.0 ms                                                                | 104 ms: 1.13x slower                                                           |
| comprehensions             | 20.7 us                                                                | 23.5 us: 1.13x slower                                                          |
| nbody                      | 112 ms                                                                 | 129 ms: 1.15x slower                                                           |
| mako                       | 13.1 ms                                                                | 15.2 ms: 1.16x slower                                                          |
| hexiom                     | 8.14 ms                                                                | 9.42 ms: 1.16x slower                                                          |
| spectral_norm              | 135 ms                                                                 | 157 ms: 1.16x slower                                                           |
| scimark_sparse_mat_mult    | 5.43 ms                                                                | 6.42 ms: 1.18x slower                                                          |
| Geometric mean             | (ref)                                                                  | 1.03x slower                                                                   |

Benchmark hidden because not significant (18): typing_runtime_protocols, pathlib, json_loads, json_dumps, create_gc_cycles, asyncio_websockets, bench_mp_pool, generators, asyncio_tcp_ssl, xml_etree_parse, scimark_sor, dulwich_log, async_generators, dask, tornado_http, sqlite_synth, logging_format, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.00x