# Results vs. base

- fork: mdboom
- ref: compact_long
- machine: linux-x86_64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.00x slower
- HPT reliability: 99.81%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 264 ms: 1.00x slower                                           |
| chameleon      | 7.00 ms                                                                | 7.06 ms: 1.01x slower                                          |
| docutils       | 2.61 sec                                                               | 2.59 sec: 1.01x faster                                         |
| tornado_http   | 94.3 ms                                                                | 95.0 ms: 1.01x slower                                          |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io              | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                         |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 727 ms: 1.02x slower                                           |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 755 ms: 1.02x slower                                           |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (5): async_tree_memoization, async_tree_none_tg, async_tree_memoization_tg, async_tree_io_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 92.4 ms                                                                | 91.2 ms: 1.01x faster                                          |
| float          | 80.9 ms                                                                | 81.9 ms: 1.01x slower                                          |
| pidigits       | 196 ms                                                                 | 222 ms: 1.14x slower                                           |
| Geometric mean | (ref)                                                                  | 1.04x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_v8       | 25.7 ms                                                                | 24.4 ms: 1.06x faster                                          |
| regex_effbot   | 3.68 ms                                                                | 3.50 ms: 1.05x faster                                          |
| regex_dna      | 219 ms                                                                 | 217 ms: 1.01x faster                                           |
| regex_compile  | 133 ms                                                                 | 134 ms: 1.01x slower                                           |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle               | 11.6 us                                                                | 11.1 us: 1.05x faster                                          |
| unpickle             | 15.5 us                                                                | 15.0 us: 1.03x faster                                          |
| xml_etree_generate   | 86.6 ms                                                                | 85.9 ms: 1.01x faster                                          |
| pickle_list          | 5.09 us                                                                | 5.05 us: 1.01x faster                                          |
| xml_etree_process    | 59.4 ms                                                                | 59.0 ms: 1.01x faster                                          |
| json_dumps           | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                          |
| xml_etree_parse      | 157 ms                                                                 | 159 ms: 1.01x slower                                           |
| unpickle_pure_python | 217 us                                                                 | 220 us: 1.01x slower                                           |
| tomli_loads          | 2.14 sec                                                               | 2.17 sec: 1.01x slower                                         |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (5): json_loads, pickle_pure_python, pickle_dict, xml_etree_iterparse, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.4 ms                                                                | 10.4 ms: 1.00x faster                                          |
| python_startup_no_site | 9.01 ms                                                                | 8.99 ms: 1.00x faster                                          |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.4 ms                                                                | 11.4 ms: 1.00x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_v8                   | 25.7 ms                                                                | 24.4 ms: 1.06x faster                                          |
| pickle                     | 11.6 us                                                                | 11.1 us: 1.05x faster                                          |
| regex_effbot               | 3.68 ms                                                                | 3.50 ms: 1.05x faster                                          |
| pycparser                  | 1.20 sec                                                               | 1.15 sec: 1.05x faster                                         |
| scimark_sparse_mat_mult    | 5.02 ms                                                                | 4.85 ms: 1.04x faster                                          |
| unpickle                   | 15.5 us                                                                | 15.0 us: 1.03x faster                                          |
| go                         | 142 ms                                                                 | 139 ms: 1.03x faster                                           |
| coverage                   | 95.4 ms                                                                | 93.0 ms: 1.03x faster                                          |
| nbody                      | 92.4 ms                                                                | 91.2 ms: 1.01x faster                                          |
| logging_simple             | 5.74 us                                                                | 5.68 us: 1.01x faster                                          |
| logging_format             | 6.32 us                                                                | 6.24 us: 1.01x faster                                          |
| regex_dna                  | 219 ms                                                                 | 217 ms: 1.01x faster                                           |
| scimark_monte_carlo        | 69.3 ms                                                                | 68.5 ms: 1.01x faster                                          |
| docutils                   | 2.61 sec                                                               | 2.59 sec: 1.01x faster                                         |
| logging_silent             | 104 ns                                                                 | 103 ns: 1.01x faster                                           |
| spectral_norm              | 112 ms                                                                 | 111 ms: 1.01x faster                                           |
| xml_etree_generate         | 86.6 ms                                                                | 85.9 ms: 1.01x faster                                          |
| deepcopy_reduce            | 3.09 us                                                                | 3.07 us: 1.01x faster                                          |
| pickle_list                | 5.09 us                                                                | 5.05 us: 1.01x faster                                          |
| xml_etree_process          | 59.4 ms                                                                | 59.0 ms: 1.01x faster                                          |
| python_startup             | 10.4 ms                                                                | 10.4 ms: 1.00x faster                                          |
| python_startup_no_site     | 9.01 ms                                                                | 8.99 ms: 1.00x faster                                          |
| meteor_contest             | 109 ms                                                                 | 109 ms: 1.00x faster                                           |
| asyncio_tcp                | 483 ms                                                                 | 485 ms: 1.00x slower                                           |
| comprehensions             | 16.3 us                                                                | 16.3 us: 1.00x slower                                          |
| deepcopy_memo              | 39.0 us                                                                | 39.2 us: 1.00x slower                                          |
| mako                       | 11.4 ms                                                                | 11.4 ms: 1.00x slower                                          |
| 2to3                       | 263 ms                                                                 | 264 ms: 1.00x slower                                           |
| dulwich_log                | 65.5 ms                                                                | 65.8 ms: 1.00x slower                                          |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.79 sec: 1.00x slower                                         |
| sympy_sum                  | 147 ms                                                                 | 148 ms: 1.00x slower                                           |
| sqlglot_optimize           | 53.5 ms                                                                | 53.8 ms: 1.00x slower                                          |
| json_dumps                 | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                          |
| fannkuch                   | 394 ms                                                                 | 397 ms: 1.01x slower                                           |
| deepcopy                   | 349 us                                                                 | 351 us: 1.01x slower                                           |
| create_gc_cycles           | 1.46 ms                                                                | 1.48 ms: 1.01x slower                                          |
| async_tree_io              | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                         |
| tornado_http               | 94.3 ms                                                                | 95.0 ms: 1.01x slower                                          |
| sqlglot_normalize          | 105 ms                                                                 | 106 ms: 1.01x slower                                           |
| pprint_safe_repr           | 739 ms                                                                 | 745 ms: 1.01x slower                                           |
| chameleon                  | 7.00 ms                                                                | 7.06 ms: 1.01x slower                                          |
| raytrace                   | 272 ms                                                                 | 275 ms: 1.01x slower                                           |
| scimark_fft                | 366 ms                                                                 | 369 ms: 1.01x slower                                           |
| sqlglot_parse              | 1.26 ms                                                                | 1.27 ms: 1.01x slower                                          |
| sqlglot_transpile          | 1.57 ms                                                                | 1.59 ms: 1.01x slower                                          |
| hexiom                     | 6.09 ms                                                                | 6.15 ms: 1.01x slower                                          |
| regex_compile              | 133 ms                                                                 | 134 ms: 1.01x slower                                           |
| xml_etree_parse            | 157 ms                                                                 | 159 ms: 1.01x slower                                           |
| float                      | 80.9 ms                                                                | 81.9 ms: 1.01x slower                                          |
| unpickle_pure_python       | 217 us                                                                 | 220 us: 1.01x slower                                           |
| tomli_loads                | 2.14 sec                                                               | 2.17 sec: 1.01x slower                                         |
| sympy_expand               | 451 ms                                                                 | 457 ms: 1.01x slower                                           |
| scimark_lu                 | 115 ms                                                                 | 117 ms: 1.01x slower                                           |
| mdp                        | 2.56 sec                                                               | 2.59 sec: 1.01x slower                                         |
| pathlib                    | 18.1 ms                                                                | 18.4 ms: 1.02x slower                                          |
| generators                 | 28.6 ms                                                                | 29.1 ms: 1.02x slower                                          |
| deltablue                  | 3.25 ms                                                                | 3.32 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 727 ms: 1.02x slower                                           |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 755 ms: 1.02x slower                                           |
| telco                      | 8.34 ms                                                                | 8.55 ms: 1.03x slower                                          |
| pyflate                    | 459 ms                                                                 | 472 ms: 1.03x slower                                           |
| gc_traversal               | 4.16 ms                                                                | 4.30 ms: 1.03x slower                                          |
| coroutines                 | 21.7 ms                                                                | 22.5 ms: 1.04x slower                                          |
| crypto_pyaes               | 70.9 ms                                                                | 75.0 ms: 1.06x slower                                          |
| pidigits                   | 196 ms                                                                 | 222 ms: 1.14x slower                                           |
| unpack_sequence            | 46.6 ns                                                                | 54.7 ns: 1.18x slower                                          |
| Geometric mean             | (ref)                                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (26): async_tree_memoization, json, async_tree_none_tg, richards, async_tree_memoization_tg, async_generators, json_loads, nqueens, mypy2, pickle_pure_python, pickle_dict, bench_thread_pool, bench_mp_pool, chaos, sympy_integrate, asyncio_websockets, async_tree_io_tg, xml_etree_iterparse, pprint_pformat, scimark_sor, typing_runtime_protocols, unpickle_list, sqlite_synth, sympy_str, richards_super, async_tree_none
Ignored benchmarks (1) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: dask


# HPT report

- Reliability score: 99.81% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x