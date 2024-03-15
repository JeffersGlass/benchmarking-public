# Results vs. base

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 01a12af
- commit date: 2023-12-19
- overall geometric mean: 1.01x slower
- HPT reliability: 88.93%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 264 ms: 1.00x slower                                                   |
| tornado_http   | 94.3 ms                                                                | 94.9 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (2): chameleon, docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_memoization     | 568 ms                                                                 | 561 ms: 1.01x faster                                                   |
| async_tree_none_tg         | 457 ms                                                                 | 454 ms: 1.01x faster                                                   |
| async_tree_io              | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                                 |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 834 ms: 1.17x slower                                                   |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 866 ms: 1.17x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_none, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 92.4 ms                                                                | 89.2 ms: 1.04x faster                                                  |
| float          | 80.9 ms                                                                | 81.5 ms: 1.01x slower                                                  |
| pidigits       | 196 ms                                                                 | 289 ms: 1.48x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.13x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 25.7 ms                                                                | 24.5 ms: 1.05x faster                                                  |
| regex_effbot   | 3.68 ms                                                                | 3.69 ms: 1.00x slower                                                  |
| regex_dna      | 219 ms                                                                 | 222 ms: 1.01x slower                                                   |
| regex_compile  | 133 ms                                                                 | 136 ms: 1.02x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_dict          | 34.3 us                                                                | 32.8 us: 1.05x faster                                                  |
| unpickle             | 15.5 us                                                                | 14.8 us: 1.05x faster                                                  |
| pickle               | 11.6 us                                                                | 11.3 us: 1.03x faster                                                  |
| xml_etree_generate   | 86.6 ms                                                                | 86.2 ms: 1.00x faster                                                  |
| xml_etree_parse      | 157 ms                                                                 | 158 ms: 1.00x slower                                                   |
| pickle_list          | 5.09 us                                                                | 5.15 us: 1.01x slower                                                  |
| tomli_loads          | 2.14 sec                                                               | 2.17 sec: 1.01x slower                                                 |
| pickle_pure_python   | 302 us                                                                 | 306 us: 1.01x slower                                                   |
| unpickle_pure_python | 217 us                                                                 | 222 us: 1.02x slower                                                   |
| unpickle_list        | 5.04 us                                                                | 5.16 us: 1.02x slower                                                  |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (4): json_loads, json_dumps, xml_etree_process, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup_no_site | 9.01 ms                                                                | 9.00 ms: 1.00x faster                                                  |
| python_startup         | 10.4 ms                                                                | 10.4 ms: 1.00x faster                                                  |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.4 ms                                                                | 11.2 ms: 1.02x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| gc_traversal               | 4.16 ms                                                                | 3.96 ms: 1.05x faster                                                  |
| regex_v8                   | 25.7 ms                                                                | 24.5 ms: 1.05x faster                                                  |
| pickle_dict                | 34.3 us                                                                | 32.8 us: 1.05x faster                                                  |
| unpickle                   | 15.5 us                                                                | 14.8 us: 1.05x faster                                                  |
| pycparser                  | 1.20 sec                                                               | 1.16 sec: 1.04x faster                                                 |
| nbody                      | 92.4 ms                                                                | 89.2 ms: 1.04x faster                                                  |
| pickle                     | 11.6 us                                                                | 11.3 us: 1.03x faster                                                  |
| mako                       | 11.4 ms                                                                | 11.2 ms: 1.02x faster                                                  |
| pyflate                    | 459 ms                                                                 | 452 ms: 1.02x faster                                                   |
| go                         | 142 ms                                                                 | 140 ms: 1.02x faster                                                   |
| async_tree_memoization     | 568 ms                                                                 | 561 ms: 1.01x faster                                                   |
| spectral_norm              | 112 ms                                                                 | 110 ms: 1.01x faster                                                   |
| scimark_fft                | 366 ms                                                                 | 362 ms: 1.01x faster                                                   |
| coverage                   | 95.4 ms                                                                | 94.2 ms: 1.01x faster                                                  |
| json                       | 5.19 ms                                                                | 5.13 ms: 1.01x faster                                                  |
| logging_format             | 6.32 us                                                                | 6.25 us: 1.01x faster                                                  |
| logging_simple             | 5.74 us                                                                | 5.69 us: 1.01x faster                                                  |
| scimark_monte_carlo        | 69.3 ms                                                                | 68.8 ms: 1.01x faster                                                  |
| deepcopy_memo              | 39.0 us                                                                | 38.8 us: 1.01x faster                                                  |
| scimark_lu                 | 115 ms                                                                 | 114 ms: 1.01x faster                                                   |
| async_tree_none_tg         | 457 ms                                                                 | 454 ms: 1.01x faster                                                   |
| xml_etree_generate         | 86.6 ms                                                                | 86.2 ms: 1.00x faster                                                  |
| hexiom                     | 6.09 ms                                                                | 6.06 ms: 1.00x faster                                                  |
| chaos                      | 60.9 ms                                                                | 60.6 ms: 1.00x faster                                                  |
| python_startup_no_site     | 9.01 ms                                                                | 9.00 ms: 1.00x faster                                                  |
| scimark_sparse_mat_mult    | 5.02 ms                                                                | 5.01 ms: 1.00x faster                                                  |
| meteor_contest             | 109 ms                                                                 | 109 ms: 1.00x faster                                                   |
| python_startup             | 10.4 ms                                                                | 10.4 ms: 1.00x faster                                                  |
| bench_thread_pool          | 828 us                                                                 | 830 us: 1.00x slower                                                   |
| asyncio_tcp                | 483 ms                                                                 | 485 ms: 1.00x slower                                                   |
| regex_effbot               | 3.68 ms                                                                | 3.69 ms: 1.00x slower                                                  |
| 2to3                       | 263 ms                                                                 | 264 ms: 1.00x slower                                                   |
| sympy_integrate            | 19.5 ms                                                                | 19.6 ms: 1.00x slower                                                  |
| async_generators           | 443 ms                                                                 | 445 ms: 1.00x slower                                                   |
| xml_etree_parse            | 157 ms                                                                 | 158 ms: 1.00x slower                                                   |
| async_tree_io              | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                                 |
| sqlglot_optimize           | 53.5 ms                                                                | 53.8 ms: 1.01x slower                                                  |
| pathlib                    | 18.1 ms                                                                | 18.2 ms: 1.01x slower                                                  |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.79 sec: 1.01x slower                                                 |
| tornado_http               | 94.3 ms                                                                | 94.9 ms: 1.01x slower                                                  |
| sqlglot_normalize          | 105 ms                                                                 | 106 ms: 1.01x slower                                                   |
| coroutines                 | 21.7 ms                                                                | 21.9 ms: 1.01x slower                                                  |
| fannkuch                   | 394 ms                                                                 | 397 ms: 1.01x slower                                                   |
| sympy_expand               | 451 ms                                                                 | 455 ms: 1.01x slower                                                   |
| float                      | 80.9 ms                                                                | 81.5 ms: 1.01x slower                                                  |
| deepcopy_reduce            | 3.09 us                                                                | 3.12 us: 1.01x slower                                                  |
| regex_dna                  | 219 ms                                                                 | 222 ms: 1.01x slower                                                   |
| pickle_list                | 5.09 us                                                                | 5.15 us: 1.01x slower                                                  |
| tomli_loads                | 2.14 sec                                                               | 2.17 sec: 1.01x slower                                                 |
| sqlglot_parse              | 1.26 ms                                                                | 1.28 ms: 1.01x slower                                                  |
| comprehensions             | 16.3 us                                                                | 16.5 us: 1.01x slower                                                  |
| pickle_pure_python         | 302 us                                                                 | 306 us: 1.01x slower                                                   |
| deltablue                  | 3.25 ms                                                                | 3.30 ms: 1.01x slower                                                  |
| sqlglot_transpile          | 1.57 ms                                                                | 1.60 ms: 1.02x slower                                                  |
| deepcopy                   | 349 us                                                                 | 356 us: 1.02x slower                                                   |
| crypto_pyaes               | 70.9 ms                                                                | 72.3 ms: 1.02x slower                                                  |
| create_gc_cycles           | 1.46 ms                                                                | 1.49 ms: 1.02x slower                                                  |
| regex_compile              | 133 ms                                                                 | 136 ms: 1.02x slower                                                   |
| mdp                        | 2.56 sec                                                               | 2.61 sec: 1.02x slower                                                 |
| unpickle_pure_python       | 217 us                                                                 | 222 us: 1.02x slower                                                   |
| unpickle_list              | 5.04 us                                                                | 5.16 us: 1.02x slower                                                  |
| generators                 | 28.6 ms                                                                | 29.3 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 834 ms: 1.17x slower                                                   |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 866 ms: 1.17x slower                                                   |
| pidigits                   | 196 ms                                                                 | 289 ms: 1.48x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (27): richards, telco, async_tree_memoization_tg, dulwich_log, sympy_sum, docutils, mypy2, scimark_sor, nqueens, raytrace, json_loads, pprint_pformat, asyncio_websockets, json_dumps, bench_mp_pool, xml_etree_process, typing_runtime_protocols, sqlite_synth, xml_etree_iterparse, chameleon, unpack_sequence, richards_super, async_tree_none, pprint_safe_repr, async_tree_io_tg, logging_silent, sympy_str
Ignored benchmarks (1) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: dask


# HPT report

- Reliability score: 88.93% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x