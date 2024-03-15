# Results vs. base

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 7b9e10f
- commit date: 2024-02-08
- overall geometric mean: 1.00x faster
- HPT reliability: 97.39%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                                 | 282 ms: 1.01x slower                                                           |
| chameleon      | 7.28 ms                                                                | 7.18 ms: 1.01x faster                                                          |
| docutils       | 2.70 sec                                                               | 2.69 sec: 1.00x faster                                                         |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|--------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none_tg | 454 ms                                                                 | 456 ms: 1.01x slower                                                           |
| async_tree_io_tg   | 1.20 sec                                                               | 1.21 sec: 1.01x slower                                                         |
| async_tree_io      | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                                         |
| Geometric mean     | (ref)                                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (5): async_tree_none, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| float          | 89.7 ms                                                                | 88.5 ms: 1.01x faster                                                          |
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x faster                                                           |
| nbody          | 112 ms                                                                 | 115 ms: 1.03x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                                 | 148 ms: 1.00x slower                                                           |
| regex_dna      | 221 ms                                                                 | 222 ms: 1.00x slower                                                           |
| regex_effbot   | 3.62 ms                                                                | 3.65 ms: 1.01x slower                                                          |
| regex_v8       | 24.2 ms                                                                | 25.0 ms: 1.03x slower                                                          |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|----------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| unpickle             | 16.4 us                                                                | 15.3 us: 1.07x faster                                                          |
| pickle_dict          | 36.3 us                                                                | 35.3 us: 1.03x faster                                                          |
| json_loads           | 27.8 us                                                                | 27.7 us: 1.01x faster                                                          |
| xml_etree_process    | 60.2 ms                                                                | 59.9 ms: 1.00x faster                                                          |
| xml_etree_parse      | 157 ms                                                                 | 157 ms: 1.00x faster                                                           |
| unpickle_pure_python | 232 us                                                                 | 231 us: 1.00x faster                                                           |
| pickle_pure_python   | 297 us                                                                 | 298 us: 1.00x slower                                                           |
| tomli_loads          | 2.52 sec                                                               | 2.54 sec: 1.01x slower                                                         |
| unpickle_list        | 4.86 us                                                                | 4.99 us: 1.03x slower                                                          |
| pickle_list          | 5.12 us                                                                | 5.28 us: 1.03x slower                                                          |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                   |

Benchmark hidden because not significant (4): xml_etree_generate, pickle, xml_etree_iterparse, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                                          |
| python_startup_no_site | 8.78 ms                                                                | 8.83 ms: 1.01x slower                                                          |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|-----------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 13.1 ms                                                                | 13.2 ms: 1.00x slower                                                          |

All benchmarks:
===============

| Benchmark                | bm-20240208-linux-x86_64-python-17689e3c41d9f61bcd19-3.13.0a3+-17689e3 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-7b9e10f |
|--------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| unpack_sequence          | 52.9 ns                                                                | 39.9 ns: 1.33x faster                                                          |
| unpickle                 | 16.4 us                                                                | 15.3 us: 1.07x faster                                                          |
| pickle_dict              | 36.3 us                                                                | 35.3 us: 1.03x faster                                                          |
| typing_runtime_protocols | 117 us                                                                 | 114 us: 1.03x faster                                                           |
| pprint_pformat           | 1.67 sec                                                               | 1.64 sec: 1.02x faster                                                         |
| pathlib                  | 18.6 ms                                                                | 18.3 ms: 1.02x faster                                                          |
| chameleon                | 7.28 ms                                                                | 7.18 ms: 1.01x faster                                                          |
| scimark_fft              | 431 ms                                                                 | 425 ms: 1.01x faster                                                           |
| pprint_safe_repr         | 802 ms                                                                 | 790 ms: 1.01x faster                                                           |
| pyflate                  | 511 ms                                                                 | 504 ms: 1.01x faster                                                           |
| float                    | 89.7 ms                                                                | 88.5 ms: 1.01x faster                                                          |
| comprehensions           | 20.7 us                                                                | 20.5 us: 1.01x faster                                                          |
| scimark_monte_carlo      | 78.5 ms                                                                | 77.6 ms: 1.01x faster                                                          |
| crypto_pyaes             | 82.8 ms                                                                | 82.0 ms: 1.01x faster                                                          |
| chaos                    | 71.3 ms                                                                | 70.6 ms: 1.01x faster                                                          |
| scimark_sor              | 124 ms                                                                 | 123 ms: 1.01x faster                                                           |
| logging_format           | 6.82 us                                                                | 6.76 us: 1.01x faster                                                          |
| generators               | 29.5 ms                                                                | 29.3 ms: 1.01x faster                                                          |
| sympy_sum                | 161 ms                                                                 | 160 ms: 1.01x faster                                                           |
| json_loads               | 27.8 us                                                                | 27.7 us: 1.01x faster                                                          |
| go                       | 173 ms                                                                 | 172 ms: 1.01x faster                                                           |
| xml_etree_process        | 60.2 ms                                                                | 59.9 ms: 1.00x faster                                                          |
| sympy_integrate          | 21.1 ms                                                                | 21.0 ms: 1.00x faster                                                          |
| xml_etree_parse          | 157 ms                                                                 | 157 ms: 1.00x faster                                                           |
| unpickle_pure_python     | 232 us                                                                 | 231 us: 1.00x faster                                                           |
| docutils                 | 2.70 sec                                                               | 2.69 sec: 1.00x faster                                                         |
| mdp                      | 2.62 sec                                                               | 2.62 sec: 1.00x faster                                                         |
| bench_thread_pool        | 844 us                                                                 | 842 us: 1.00x faster                                                           |
| pidigits                 | 188 ms                                                                 | 188 ms: 1.00x faster                                                           |
| gc_traversal             | 3.49 ms                                                                | 3.49 ms: 1.00x slower                                                          |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                         |
| deepcopy                 | 352 us                                                                 | 354 us: 1.00x slower                                                           |
| pickle_pure_python       | 297 us                                                                 | 298 us: 1.00x slower                                                           |
| regex_compile            | 148 ms                                                                 | 148 ms: 1.00x slower                                                           |
| mako                     | 13.1 ms                                                                | 13.2 ms: 1.00x slower                                                          |
| regex_dna                | 221 ms                                                                 | 222 ms: 1.00x slower                                                           |
| python_startup           | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                                          |
| 2to3                     | 280 ms                                                                 | 282 ms: 1.01x slower                                                           |
| richards                 | 48.1 ms                                                                | 48.3 ms: 1.01x slower                                                          |
| python_startup_no_site   | 8.78 ms                                                                | 8.83 ms: 1.01x slower                                                          |
| sqlglot_parse            | 1.33 ms                                                                | 1.33 ms: 1.01x slower                                                          |
| async_tree_none_tg       | 454 ms                                                                 | 456 ms: 1.01x slower                                                           |
| async_tree_io_tg         | 1.20 sec                                                               | 1.21 sec: 1.01x slower                                                         |
| async_tree_io            | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                                         |
| sqlglot_optimize         | 57.6 ms                                                                | 58.0 ms: 1.01x slower                                                          |
| regex_effbot             | 3.62 ms                                                                | 3.65 ms: 1.01x slower                                                          |
| sqlglot_transpile        | 1.66 ms                                                                | 1.67 ms: 1.01x slower                                                          |
| async_generators         | 455 ms                                                                 | 460 ms: 1.01x slower                                                           |
| hexiom                   | 8.14 ms                                                                | 8.21 ms: 1.01x slower                                                          |
| deepcopy_memo            | 39.3 us                                                                | 39.7 us: 1.01x slower                                                          |
| tomli_loads              | 2.52 sec                                                               | 2.54 sec: 1.01x slower                                                         |
| fannkuch                 | 428 ms                                                                 | 433 ms: 1.01x slower                                                           |
| meteor_contest           | 112 ms                                                                 | 113 ms: 1.01x slower                                                           |
| json                     | 5.09 ms                                                                | 5.16 ms: 1.01x slower                                                          |
| deltablue                | 3.46 ms                                                                | 3.51 ms: 1.01x slower                                                          |
| nqueens                  | 92.0 ms                                                                | 93.5 ms: 1.02x slower                                                          |
| spectral_norm            | 135 ms                                                                 | 137 ms: 1.02x slower                                                           |
| sqlglot_normalize        | 114 ms                                                                 | 116 ms: 1.02x slower                                                           |
| scimark_lu               | 113 ms                                                                 | 115 ms: 1.02x slower                                                           |
| unpickle_list            | 4.86 us                                                                | 4.99 us: 1.03x slower                                                          |
| logging_silent           | 99.6 ns                                                                | 102 ns: 1.03x slower                                                           |
| nbody                    | 112 ms                                                                 | 115 ms: 1.03x slower                                                           |
| pickle_list              | 5.12 us                                                                | 5.28 us: 1.03x slower                                                          |
| regex_v8                 | 24.2 ms                                                                | 25.0 ms: 1.03x slower                                                          |
| pycparser                | 1.20 sec                                                               | 1.25 sec: 1.04x slower                                                         |
| scimark_sparse_mat_mult  | 5.43 ms                                                                | 5.75 ms: 1.06x slower                                                          |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                   |

Benchmark hidden because not significant (27): sqlite_synth, logging_simple, coroutines, deepcopy_reduce, richards_super, xml_etree_generate, asyncio_websockets, pickle, create_gc_cycles, xml_etree_iterparse, bench_mp_pool, dulwich_log, asyncio_tcp, json_dumps, dask, raytrace, tornado_http, coverage, telco, async_tree_none, async_tree_cpu_io_mixed, sympy_expand, async_tree_memoization, mypy2, sympy_str, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg


# HPT report

- Reliability score: 97.39% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x