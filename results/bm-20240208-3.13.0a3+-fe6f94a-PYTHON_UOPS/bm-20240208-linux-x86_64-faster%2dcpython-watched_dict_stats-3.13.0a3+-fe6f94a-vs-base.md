# Results vs. base

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: fe6f94a
- commit date: 2024-02-08
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                                 | 288 ms: 1.03x slower                                                           |
| chameleon      | 7.28 ms                                                                | 7.37 ms: 1.01x slower                                                          |
| docutils       | 2.70 sec                                                               | 2.71 sec: 1.00x slower                                                         |
| tornado_http   | 98.5 ms                                                                | 99.4 ms: 1.01x slower                                                          |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.20 sec                                                               | 1.21 sec: 1.01x slower                                                         |
| async_tree_io              | 1.18 sec                                                               | 1.20 sec: 1.01x slower                                                         |
| async_tree_cpu_io_mixed    | 717 ms                                                                 | 727 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 724 ms                                                                 | 735 ms: 1.01x slower                                                           |
| async_tree_memoization_tg  | 588 ms                                                                 | 598 ms: 1.02x slower                                                           |
| async_tree_none_tg         | 454 ms                                                                 | 462 ms: 1.02x slower                                                           |
| async_tree_memoization     | 571 ms                                                                 | 582 ms: 1.02x slower                                                           |
| async_tree_none            | 445 ms                                                                 | 457 ms: 1.03x slower                                                           |
| Geometric mean             | (ref)                                                                  | 1.02x slower                                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 189 ms: 1.00x slower                                                           |
| float          | 89.7 ms                                                                | 105 ms: 1.18x slower                                                           |
| nbody          | 112 ms                                                                 | 141 ms: 1.26x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.14x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_v8       | 24.2 ms                                                                | 24.4 ms: 1.01x slower                                                          |
| regex_dna      | 221 ms                                                                 | 225 ms: 1.02x slower                                                           |
| regex_effbot   | 3.62 ms                                                                | 3.70 ms: 1.02x slower                                                          |
| regex_compile  | 148 ms                                                                 | 157 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| unpickle             | 16.4 us                                                                | 15.2 us: 1.08x faster                                                          |
| pickle_dict          | 36.3 us                                                                | 35.3 us: 1.03x faster                                                          |
| pickle_pure_python   | 297 us                                                                 | 301 us: 1.01x slower                                                           |
| pickle_list          | 5.12 us                                                                | 5.24 us: 1.02x slower                                                          |
| xml_etree_process    | 60.2 ms                                                                | 61.8 ms: 1.03x slower                                                          |
| unpickle_pure_python | 232 us                                                                 | 240 us: 1.03x slower                                                           |
| xml_etree_generate   | 88.3 ms                                                                | 91.3 ms: 1.03x slower                                                          |
| xml_etree_iterparse  | 109 ms                                                                 | 115 ms: 1.06x slower                                                           |
| unpickle_list        | 4.86 us                                                                | 5.17 us: 1.06x slower                                                          |
| tomli_loads          | 2.52 sec                                                               | 2.84 sec: 1.13x slower                                                         |
| Geometric mean       | (ref)                                                                  | 1.02x slower                                                                   |

Benchmark hidden because not significant (4): json_loads, pickle, json_dumps, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                                          |
| python_startup_no_site | 8.78 ms                                                                | 8.81 ms: 1.00x slower                                                          |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|-----------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 13.1 ms                                                                | 15.4 ms: 1.17x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| unpickle                   | 16.4 us                                                                | 15.2 us: 1.08x faster                                                          |
| pickle_dict                | 36.3 us                                                                | 35.3 us: 1.03x faster                                                          |
| asyncio_tcp_ssl            | 1.80 sec                                                               | 1.81 sec: 1.00x slower                                                         |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                                          |
| python_startup_no_site     | 8.78 ms                                                                | 8.81 ms: 1.00x slower                                                          |
| docutils                   | 2.70 sec                                                               | 2.71 sec: 1.00x slower                                                         |
| pidigits                   | 188 ms                                                                 | 189 ms: 1.00x slower                                                           |
| asyncio_tcp                | 488 ms                                                                 | 490 ms: 1.01x slower                                                           |
| create_gc_cycles           | 1.46 ms                                                                | 1.47 ms: 1.01x slower                                                          |
| pathlib                    | 18.6 ms                                                                | 18.7 ms: 1.01x slower                                                          |
| sqlite_synth               | 2.87 us                                                                | 2.90 us: 1.01x slower                                                          |
| tornado_http               | 98.5 ms                                                                | 99.4 ms: 1.01x slower                                                          |
| regex_v8                   | 24.2 ms                                                                | 24.4 ms: 1.01x slower                                                          |
| async_tree_io_tg           | 1.20 sec                                                               | 1.21 sec: 1.01x slower                                                         |
| deepcopy                   | 352 us                                                                 | 356 us: 1.01x slower                                                           |
| json                       | 5.09 ms                                                                | 5.15 ms: 1.01x slower                                                          |
| pickle_pure_python         | 297 us                                                                 | 301 us: 1.01x slower                                                           |
| chameleon                  | 7.28 ms                                                                | 7.37 ms: 1.01x slower                                                          |
| bench_thread_pool          | 844 us                                                                 | 855 us: 1.01x slower                                                           |
| typing_runtime_protocols   | 117 us                                                                 | 119 us: 1.01x slower                                                           |
| async_tree_io              | 1.18 sec                                                               | 1.20 sec: 1.01x slower                                                         |
| async_tree_cpu_io_mixed    | 717 ms                                                                 | 727 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 724 ms                                                                 | 735 ms: 1.01x slower                                                           |
| regex_dna                  | 221 ms                                                                 | 225 ms: 1.02x slower                                                           |
| async_tree_memoization_tg  | 588 ms                                                                 | 598 ms: 1.02x slower                                                           |
| async_tree_none_tg         | 454 ms                                                                 | 462 ms: 1.02x slower                                                           |
| logging_format             | 6.82 us                                                                | 6.94 us: 1.02x slower                                                          |
| async_tree_memoization     | 571 ms                                                                 | 582 ms: 1.02x slower                                                           |
| go                         | 173 ms                                                                 | 177 ms: 1.02x slower                                                           |
| logging_simple             | 5.97 us                                                                | 6.10 us: 1.02x slower                                                          |
| pycparser                  | 1.20 sec                                                               | 1.23 sec: 1.02x slower                                                         |
| regex_effbot               | 3.62 ms                                                                | 3.70 ms: 1.02x slower                                                          |
| sympy_sum                  | 161 ms                                                                 | 165 ms: 1.02x slower                                                           |
| sqlglot_normalize          | 114 ms                                                                 | 117 ms: 1.02x slower                                                           |
| pickle_list                | 5.12 us                                                                | 5.24 us: 1.02x slower                                                          |
| sqlglot_optimize           | 57.6 ms                                                                | 59.0 ms: 1.03x slower                                                          |
| 2to3                       | 280 ms                                                                 | 288 ms: 1.03x slower                                                           |
| telco                      | 8.72 ms                                                                | 8.95 ms: 1.03x slower                                                          |
| xml_etree_process          | 60.2 ms                                                                | 61.8 ms: 1.03x slower                                                          |
| sqlglot_transpile          | 1.66 ms                                                                | 1.70 ms: 1.03x slower                                                          |
| async_tree_none            | 445 ms                                                                 | 457 ms: 1.03x slower                                                           |
| sympy_str                  | 292 ms                                                                 | 299 ms: 1.03x slower                                                           |
| sympy_integrate            | 21.1 ms                                                                | 21.7 ms: 1.03x slower                                                          |
| sqlglot_parse              | 1.33 ms                                                                | 1.37 ms: 1.03x slower                                                          |
| unpack_sequence            | 52.9 ns                                                                | 54.6 ns: 1.03x slower                                                          |
| unpickle_pure_python       | 232 us                                                                 | 240 us: 1.03x slower                                                           |
| xml_etree_generate         | 88.3 ms                                                                | 91.3 ms: 1.03x slower                                                          |
| coroutines                 | 22.2 ms                                                                | 22.9 ms: 1.03x slower                                                          |
| pprint_safe_repr           | 802 ms                                                                 | 834 ms: 1.04x slower                                                           |
| richards_super             | 54.4 ms                                                                | 56.8 ms: 1.04x slower                                                          |
| richards                   | 48.1 ms                                                                | 50.2 ms: 1.04x slower                                                          |
| deepcopy_memo              | 39.3 us                                                                | 41.2 us: 1.05x slower                                                          |
| pprint_pformat             | 1.67 sec                                                               | 1.75 sec: 1.05x slower                                                         |
| deltablue                  | 3.46 ms                                                                | 3.63 ms: 1.05x slower                                                          |
| meteor_contest             | 112 ms                                                                 | 118 ms: 1.06x slower                                                           |
| raytrace                   | 295 ms                                                                 | 312 ms: 1.06x slower                                                           |
| xml_etree_iterparse        | 109 ms                                                                 | 115 ms: 1.06x slower                                                           |
| gc_traversal               | 3.49 ms                                                                | 3.70 ms: 1.06x slower                                                          |
| scimark_lu                 | 113 ms                                                                 | 119 ms: 1.06x slower                                                           |
| unpickle_list              | 4.86 us                                                                | 5.17 us: 1.06x slower                                                          |
| logging_silent             | 99.6 ns                                                                | 106 ns: 1.06x slower                                                           |
| regex_compile              | 148 ms                                                                 | 157 ms: 1.06x slower                                                           |
| mdp                        | 2.62 sec                                                               | 2.83 sec: 1.08x slower                                                         |
| chaos                      | 71.3 ms                                                                | 79.8 ms: 1.12x slower                                                          |
| pyflate                    | 511 ms                                                                 | 573 ms: 1.12x slower                                                           |
| tomli_loads                | 2.52 sec                                                               | 2.84 sec: 1.13x slower                                                         |
| crypto_pyaes               | 82.8 ms                                                                | 93.8 ms: 1.13x slower                                                          |
| nqueens                    | 92.0 ms                                                                | 104 ms: 1.13x slower                                                           |
| fannkuch                   | 428 ms                                                                 | 490 ms: 1.14x slower                                                           |
| scimark_monte_carlo        | 78.5 ms                                                                | 89.8 ms: 1.14x slower                                                          |
| scimark_fft                | 431 ms                                                                 | 496 ms: 1.15x slower                                                           |
| comprehensions             | 20.7 us                                                                | 23.9 us: 1.15x slower                                                          |
| mako                       | 13.1 ms                                                                | 15.4 ms: 1.17x slower                                                          |
| float                      | 89.7 ms                                                                | 105 ms: 1.18x slower                                                           |
| hexiom                     | 8.14 ms                                                                | 9.60 ms: 1.18x slower                                                          |
| spectral_norm              | 135 ms                                                                 | 167 ms: 1.23x slower                                                           |
| scimark_sparse_mat_mult    | 5.43 ms                                                                | 6.74 ms: 1.24x slower                                                          |
| nbody                      | 112 ms                                                                 | 141 ms: 1.26x slower                                                           |
| Geometric mean             | (ref)                                                                  | 1.04x slower                                                                   |

Benchmark hidden because not significant (15): json_loads, pickle, dulwich_log, bench_mp_pool, asyncio_websockets, async_generators, scimark_sor, deepcopy_reduce, json_dumps, dask, coverage, generators, xml_etree_parse, sympy_expand, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.00x