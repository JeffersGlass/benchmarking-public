# Results vs. base

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 344a5aa
- commit date: 2023-12-20
- overall geometric mean: 1.00x faster
- HPT reliability: 74.10%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 264 ms: 1.00x slower                                                   |
| chameleon      | 7.00 ms                                                                | 6.94 ms: 1.01x faster                                                  |
| docutils       | 2.61 sec                                                               | 2.60 sec: 1.01x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_memoization     | 568 ms                                                                 | 559 ms: 1.02x faster                                                   |
| async_tree_none_tg         | 457 ms                                                                 | 453 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 746 ms: 1.01x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (5): async_tree_memoization_tg, async_tree_none, async_tree_io_tg, async_tree_io, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 80.9 ms                                                                | 81.6 ms: 1.01x slower                                                  |
| pidigits       | 196 ms                                                                 | 226 ms: 1.15x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 25.7 ms                                                                | 24.1 ms: 1.07x faster                                                  |
| regex_effbot   | 3.68 ms                                                                | 3.66 ms: 1.01x faster                                                  |
| regex_dna      | 219 ms                                                                 | 220 ms: 1.01x slower                                                   |
| regex_compile  | 133 ms                                                                 | 135 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle               | 11.6 us                                                                | 11.1 us: 1.05x faster                                                  |
| unpickle             | 15.5 us                                                                | 14.8 us: 1.05x faster                                                  |
| pickle_dict          | 34.3 us                                                                | 33.1 us: 1.04x faster                                                  |
| pickle_list          | 5.09 us                                                                | 4.98 us: 1.02x faster                                                  |
| json_loads           | 28.2 us                                                                | 27.8 us: 1.02x faster                                                  |
| xml_etree_generate   | 86.6 ms                                                                | 85.4 ms: 1.01x faster                                                  |
| xml_etree_process    | 59.4 ms                                                                | 58.8 ms: 1.01x faster                                                  |
| xml_etree_iterparse  | 106 ms                                                                 | 105 ms: 1.01x faster                                                   |
| xml_etree_parse      | 157 ms                                                                 | 156 ms: 1.00x faster                                                   |
| tomli_loads          | 2.14 sec                                                               | 2.16 sec: 1.01x slower                                                 |
| pickle_pure_python   | 302 us                                                                 | 304 us: 1.01x slower                                                   |
| unpickle_pure_python | 217 us                                                                 | 219 us: 1.01x slower                                                   |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (2): unpickle_list, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup_no_site | 9.01 ms                                                                | 8.95 ms: 1.01x faster                                                  |
| python_startup         | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                                  |
| Geometric mean         | (ref)                                                                  | 1.01x faster                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.4 ms                                                                | 11.1 ms: 1.02x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| gc_traversal               | 4.16 ms                                                                | 3.61 ms: 1.15x faster                                                  |
| unpack_sequence            | 46.6 ns                                                                | 43.4 ns: 1.07x faster                                                  |
| regex_v8                   | 25.7 ms                                                                | 24.1 ms: 1.07x faster                                                  |
| pickle                     | 11.6 us                                                                | 11.1 us: 1.05x faster                                                  |
| unpickle                   | 15.5 us                                                                | 14.8 us: 1.05x faster                                                  |
| pickle_dict                | 34.3 us                                                                | 33.1 us: 1.04x faster                                                  |
| pycparser                  | 1.20 sec                                                               | 1.16 sec: 1.03x faster                                                 |
| mako                       | 11.4 ms                                                                | 11.1 ms: 1.02x faster                                                  |
| pickle_list                | 5.09 us                                                                | 4.98 us: 1.02x faster                                                  |
| logging_format             | 6.32 us                                                                | 6.20 us: 1.02x faster                                                  |
| go                         | 142 ms                                                                 | 140 ms: 1.02x faster                                                   |
| async_tree_memoization     | 568 ms                                                                 | 559 ms: 1.02x faster                                                   |
| json_loads                 | 28.2 us                                                                | 27.8 us: 1.02x faster                                                  |
| coverage                   | 95.4 ms                                                                | 93.9 ms: 1.02x faster                                                  |
| xml_etree_generate         | 86.6 ms                                                                | 85.4 ms: 1.01x faster                                                  |
| spectral_norm              | 112 ms                                                                 | 110 ms: 1.01x faster                                                   |
| pyflate                    | 459 ms                                                                 | 453 ms: 1.01x faster                                                   |
| scimark_monte_carlo        | 69.3 ms                                                                | 68.5 ms: 1.01x faster                                                  |
| xml_etree_process          | 59.4 ms                                                                | 58.8 ms: 1.01x faster                                                  |
| telco                      | 8.34 ms                                                                | 8.27 ms: 1.01x faster                                                  |
| chameleon                  | 7.00 ms                                                                | 6.94 ms: 1.01x faster                                                  |
| async_tree_none_tg         | 457 ms                                                                 | 453 ms: 1.01x faster                                                   |
| pprint_pformat             | 1.51 sec                                                               | 1.50 sec: 1.01x faster                                                 |
| pprint_safe_repr           | 739 ms                                                                 | 734 ms: 1.01x faster                                                   |
| deepcopy_memo              | 39.0 us                                                                | 38.8 us: 1.01x faster                                                  |
| json                       | 5.19 ms                                                                | 5.15 ms: 1.01x faster                                                  |
| xml_etree_iterparse        | 106 ms                                                                 | 105 ms: 1.01x faster                                                   |
| regex_effbot               | 3.68 ms                                                                | 3.66 ms: 1.01x faster                                                  |
| chaos                      | 60.9 ms                                                                | 60.4 ms: 1.01x faster                                                  |
| python_startup_no_site     | 9.01 ms                                                                | 8.95 ms: 1.01x faster                                                  |
| python_startup             | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                                  |
| docutils                   | 2.61 sec                                                               | 2.60 sec: 1.01x faster                                                 |
| xml_etree_parse            | 157 ms                                                                 | 156 ms: 1.00x faster                                                   |
| create_gc_cycles           | 1.46 ms                                                                | 1.46 ms: 1.00x faster                                                  |
| scimark_fft                | 366 ms                                                                 | 367 ms: 1.00x slower                                                   |
| dulwich_log                | 65.5 ms                                                                | 65.7 ms: 1.00x slower                                                  |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.79 sec: 1.00x slower                                                 |
| 2to3                       | 263 ms                                                                 | 264 ms: 1.00x slower                                                   |
| sqlglot_optimize           | 53.5 ms                                                                | 53.8 ms: 1.01x slower                                                  |
| meteor_contest             | 109 ms                                                                 | 110 ms: 1.01x slower                                                   |
| regex_dna                  | 219 ms                                                                 | 220 ms: 1.01x slower                                                   |
| hexiom                     | 6.09 ms                                                                | 6.12 ms: 1.01x slower                                                  |
| fannkuch                   | 394 ms                                                                 | 396 ms: 1.01x slower                                                   |
| bench_thread_pool          | 828 us                                                                 | 833 us: 1.01x slower                                                   |
| tomli_loads                | 2.14 sec                                                               | 2.16 sec: 1.01x slower                                                 |
| sympy_expand               | 451 ms                                                                 | 455 ms: 1.01x slower                                                   |
| sqlglot_normalize          | 105 ms                                                                 | 106 ms: 1.01x slower                                                   |
| pickle_pure_python         | 302 us                                                                 | 304 us: 1.01x slower                                                   |
| logging_silent             | 104 ns                                                                 | 105 ns: 1.01x slower                                                   |
| raytrace                   | 272 ms                                                                 | 275 ms: 1.01x slower                                                   |
| float                      | 80.9 ms                                                                | 81.6 ms: 1.01x slower                                                  |
| deepcopy_reduce            | 3.09 us                                                                | 3.13 us: 1.01x slower                                                  |
| scimark_lu                 | 115 ms                                                                 | 116 ms: 1.01x slower                                                   |
| pathlib                    | 18.1 ms                                                                | 18.3 ms: 1.01x slower                                                  |
| unpickle_pure_python       | 217 us                                                                 | 219 us: 1.01x slower                                                   |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 746 ms: 1.01x slower                                                   |
| sqlglot_parse              | 1.26 ms                                                                | 1.28 ms: 1.01x slower                                                  |
| regex_compile              | 133 ms                                                                 | 135 ms: 1.01x slower                                                   |
| coroutines                 | 21.7 ms                                                                | 22.0 ms: 1.02x slower                                                  |
| sqlglot_transpile          | 1.57 ms                                                                | 1.60 ms: 1.02x slower                                                  |
| comprehensions             | 16.3 us                                                                | 16.6 us: 1.02x slower                                                  |
| nqueens                    | 80.0 ms                                                                | 81.6 ms: 1.02x slower                                                  |
| sympy_str                  | 267 ms                                                                 | 273 ms: 1.02x slower                                                   |
| crypto_pyaes               | 70.9 ms                                                                | 72.8 ms: 1.03x slower                                                  |
| deltablue                  | 3.25 ms                                                                | 3.37 ms: 1.04x slower                                                  |
| generators                 | 28.6 ms                                                                | 29.7 ms: 1.04x slower                                                  |
| mdp                        | 2.56 sec                                                               | 2.68 sec: 1.05x slower                                                 |
| pidigits                   | 196 ms                                                                 | 226 ms: 1.15x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (24): nbody, typing_runtime_protocols, logging_simple, sqlite_synth, async_tree_memoization_tg, mypy2, sympy_sum, asyncio_websockets, scimark_sor, async_tree_none, scimark_sparse_mat_mult, bench_mp_pool, sympy_integrate, unpickle_list, asyncio_tcp, json_dumps, async_tree_io_tg, deepcopy, async_tree_io, async_generators, tornado_http, richards, async_tree_cpu_io_mixed, richards_super
Ignored benchmarks (1) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: dask


# HPT report

- Reliability score: 74.10% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x