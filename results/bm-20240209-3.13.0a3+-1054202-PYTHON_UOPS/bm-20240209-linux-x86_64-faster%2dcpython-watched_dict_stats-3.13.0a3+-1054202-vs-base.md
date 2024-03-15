# Results vs. base

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 1054202
- commit date: 2024-02-09
- overall geometric mean: 1.01x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                                 | 282 ms: 1.01x slower                                                           |
| chameleon      | 7.28 ms                                                                | 7.40 ms: 1.02x slower                                                          |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_io              | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                                         |
| async_tree_io_tg           | 1.20 sec                                                               | 1.21 sec: 1.01x slower                                                         |
| async_tree_memoization     | 571 ms                                                                 | 577 ms: 1.01x slower                                                           |
| async_tree_none_tg         | 454 ms                                                                 | 459 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 724 ms                                                                 | 733 ms: 1.01x slower                                                           |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x slower                                                           |
| float          | 89.7 ms                                                                | 91.4 ms: 1.02x slower                                                          |
| nbody          | 112 ms                                                                 | 121 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                                 | 150 ms: 1.02x slower                                                           |
| regex_dna      | 221 ms                                                                 | 228 ms: 1.03x slower                                                           |
| regex_v8       | 24.2 ms                                                                | 25.1 ms: 1.04x slower                                                          |
| regex_effbot   | 3.62 ms                                                                | 3.77 ms: 1.04x slower                                                          |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|--------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| unpickle           | 16.4 us                                                                | 15.3 us: 1.08x faster                                                          |
| pickle_dict        | 36.3 us                                                                | 34.7 us: 1.05x faster                                                          |
| pickle             | 11.9 us                                                                | 11.6 us: 1.02x faster                                                          |
| xml_etree_generate | 88.3 ms                                                                | 88.5 ms: 1.00x slower                                                          |
| json_dumps         | 10.5 ms                                                                | 10.6 ms: 1.00x slower                                                          |
| xml_etree_process  | 60.2 ms                                                                | 60.6 ms: 1.01x slower                                                          |
| xml_etree_parse    | 157 ms                                                                 | 159 ms: 1.01x slower                                                           |
| pickle_list        | 5.12 us                                                                | 5.25 us: 1.02x slower                                                          |
| unpickle_list      | 4.86 us                                                                | 5.03 us: 1.04x slower                                                          |
| tomli_loads        | 2.52 sec                                                               | 2.62 sec: 1.04x slower                                                         |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                                   |

Benchmark hidden because not significant (4): json_loads, unpickle_pure_python, pickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                          |
| python_startup_no_site | 8.78 ms                                                                | 8.75 ms: 1.00x faster                                                          |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|-----------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 13.1 ms                                                                | 13.9 ms: 1.06x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240209-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-1054202 |
|----------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| go                         | 173 ms                                                                 | 156 ms: 1.11x faster                                                           |
| unpickle                   | 16.4 us                                                                | 15.3 us: 1.08x faster                                                          |
| pickle_dict                | 36.3 us                                                                | 34.7 us: 1.05x faster                                                          |
| scimark_sor                | 124 ms                                                                 | 121 ms: 1.02x faster                                                           |
| typing_runtime_protocols   | 117 us                                                                 | 115 us: 1.02x faster                                                           |
| pickle                     | 11.9 us                                                                | 11.6 us: 1.02x faster                                                          |
| async_generators           | 455 ms                                                                 | 449 ms: 1.02x faster                                                           |
| pathlib                    | 18.6 ms                                                                | 18.4 ms: 1.01x faster                                                          |
| telco                      | 8.72 ms                                                                | 8.65 ms: 1.01x faster                                                          |
| dulwich_log                | 69.3 ms                                                                | 69.0 ms: 1.01x faster                                                          |
| pprint_pformat             | 1.67 sec                                                               | 1.66 sec: 1.01x faster                                                         |
| generators                 | 29.5 ms                                                                | 29.4 ms: 1.00x faster                                                          |
| python_startup             | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                          |
| python_startup_no_site     | 8.78 ms                                                                | 8.75 ms: 1.00x faster                                                          |
| pidigits                   | 188 ms                                                                 | 188 ms: 1.00x slower                                                           |
| bench_thread_pool          | 844 us                                                                 | 846 us: 1.00x slower                                                           |
| asyncio_tcp_ssl            | 1.80 sec                                                               | 1.81 sec: 1.00x slower                                                         |
| xml_etree_generate         | 88.3 ms                                                                | 88.5 ms: 1.00x slower                                                          |
| coverage                   | 94.4 ms                                                                | 94.8 ms: 1.00x slower                                                          |
| json_dumps                 | 10.5 ms                                                                | 10.6 ms: 1.00x slower                                                          |
| sqlglot_parse              | 1.33 ms                                                                | 1.33 ms: 1.00x slower                                                          |
| mdp                        | 2.62 sec                                                               | 2.64 sec: 1.00x slower                                                         |
| xml_etree_process          | 60.2 ms                                                                | 60.6 ms: 1.01x slower                                                          |
| sqlglot_transpile          | 1.66 ms                                                                | 1.67 ms: 1.01x slower                                                          |
| 2to3                       | 280 ms                                                                 | 282 ms: 1.01x slower                                                           |
| deepcopy_reduce            | 3.12 us                                                                | 3.14 us: 1.01x slower                                                          |
| create_gc_cycles           | 1.46 ms                                                                | 1.48 ms: 1.01x slower                                                          |
| xml_etree_parse            | 157 ms                                                                 | 159 ms: 1.01x slower                                                           |
| sympy_integrate            | 21.1 ms                                                                | 21.3 ms: 1.01x slower                                                          |
| async_tree_io              | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                                         |
| asyncio_tcp                | 488 ms                                                                 | 492 ms: 1.01x slower                                                           |
| deepcopy_memo              | 39.3 us                                                                | 39.7 us: 1.01x slower                                                          |
| raytrace                   | 295 ms                                                                 | 298 ms: 1.01x slower                                                           |
| logging_simple             | 5.97 us                                                                | 6.03 us: 1.01x slower                                                          |
| sympy_str                  | 292 ms                                                                 | 294 ms: 1.01x slower                                                           |
| async_tree_io_tg           | 1.20 sec                                                               | 1.21 sec: 1.01x slower                                                         |
| async_tree_memoization     | 571 ms                                                                 | 577 ms: 1.01x slower                                                           |
| async_tree_none_tg         | 454 ms                                                                 | 459 ms: 1.01x slower                                                           |
| sqlglot_normalize          | 114 ms                                                                 | 115 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 724 ms                                                                 | 733 ms: 1.01x slower                                                           |
| meteor_contest             | 112 ms                                                                 | 113 ms: 1.01x slower                                                           |
| sympy_sum                  | 161 ms                                                                 | 163 ms: 1.01x slower                                                           |
| sqlglot_optimize           | 57.6 ms                                                                | 58.4 ms: 1.01x slower                                                          |
| regex_compile              | 148 ms                                                                 | 150 ms: 1.02x slower                                                           |
| chameleon                  | 7.28 ms                                                                | 7.40 ms: 1.02x slower                                                          |
| logging_silent             | 99.6 ns                                                                | 101 ns: 1.02x slower                                                           |
| float                      | 89.7 ms                                                                | 91.4 ms: 1.02x slower                                                          |
| crypto_pyaes               | 82.8 ms                                                                | 84.5 ms: 1.02x slower                                                          |
| pycparser                  | 1.20 sec                                                               | 1.23 sec: 1.02x slower                                                         |
| scimark_fft                | 431 ms                                                                 | 440 ms: 1.02x slower                                                           |
| richards_super             | 54.4 ms                                                                | 55.7 ms: 1.02x slower                                                          |
| richards                   | 48.1 ms                                                                | 49.3 ms: 1.02x slower                                                          |
| pickle_list                | 5.12 us                                                                | 5.25 us: 1.02x slower                                                          |
| chaos                      | 71.3 ms                                                                | 73.2 ms: 1.03x slower                                                          |
| scimark_lu                 | 113 ms                                                                 | 116 ms: 1.03x slower                                                           |
| fannkuch                   | 428 ms                                                                 | 440 ms: 1.03x slower                                                           |
| pyflate                    | 511 ms                                                                 | 526 ms: 1.03x slower                                                           |
| regex_dna                  | 221 ms                                                                 | 228 ms: 1.03x slower                                                           |
| comprehensions             | 20.7 us                                                                | 21.4 us: 1.03x slower                                                          |
| scimark_monte_carlo        | 78.5 ms                                                                | 81.1 ms: 1.03x slower                                                          |
| unpickle_list              | 4.86 us                                                                | 5.03 us: 1.04x slower                                                          |
| hexiom                     | 8.14 ms                                                                | 8.44 ms: 1.04x slower                                                          |
| regex_v8                   | 24.2 ms                                                                | 25.1 ms: 1.04x slower                                                          |
| regex_effbot               | 3.62 ms                                                                | 3.77 ms: 1.04x slower                                                          |
| tomli_loads                | 2.52 sec                                                               | 2.62 sec: 1.04x slower                                                         |
| mako                       | 13.1 ms                                                                | 13.9 ms: 1.06x slower                                                          |
| nqueens                    | 92.0 ms                                                                | 97.6 ms: 1.06x slower                                                          |
| gc_traversal               | 3.49 ms                                                                | 3.71 ms: 1.06x slower                                                          |
| spectral_norm              | 135 ms                                                                 | 144 ms: 1.07x slower                                                           |
| nbody                      | 112 ms                                                                 | 121 ms: 1.08x slower                                                           |
| unpack_sequence            | 52.9 ns                                                                | 57.1 ns: 1.08x slower                                                          |
| scimark_sparse_mat_mult    | 5.43 ms                                                                | 6.11 ms: 1.13x slower                                                          |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (21): logging_format, pprint_safe_repr, json_loads, unpickle_pure_python, coroutines, bench_mp_pool, asyncio_websockets, tornado_http, deepcopy, pickle_pure_python, docutils, json, sqlite_synth, xml_etree_iterparse, deltablue, sympy_expand, dask, mypy2, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_none


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x