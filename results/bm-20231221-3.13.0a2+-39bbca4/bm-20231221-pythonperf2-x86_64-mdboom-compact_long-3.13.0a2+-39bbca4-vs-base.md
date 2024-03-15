# Results vs. base

- fork: mdboom
- ref: compact_long
- machine: linux-x86_64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.00x faster
- HPT reliability: 78.65%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 293 ms                                                                       | 294 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                         |

Benchmark hidden because not significant (3): chameleon, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io_tg           | 1.09 sec                                                                     | 1.10 sec: 1.01x slower                                               |
| async_tree_none_tg         | 436 ms                                                                       | 444 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed    | 699 ms                                                                       | 713 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed_tg | 715 ms                                                                       | 734 ms: 1.03x slower                                                 |
| Geometric mean             | (ref)                                                                        | 1.01x slower                                                         |

Benchmark hidden because not significant (4): async_tree_io, async_tree_memoization, async_tree_memoization_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 79.4 ms                                                                      | 76.8 ms: 1.03x faster                                                |
| nbody          | 85.9 ms                                                                      | 84.3 ms: 1.02x faster                                                |
| pidigits       | 264 ms                                                                       | 267 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 3.46 ms                                                                      | 3.44 ms: 1.01x faster                                                |
| regex_v8       | 24.8 ms                                                                      | 24.7 ms: 1.01x faster                                                |
| regex_compile  | 145 ms                                                                       | 146 ms: 1.00x slower                                                 |
| regex_dna      | 236 ms                                                                       | 240 ms: 1.02x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle_list        | 4.71 us                                                                      | 4.54 us: 1.04x faster                                                |
| pickle_dict          | 32.8 us                                                                      | 31.6 us: 1.04x faster                                                |
| pickle               | 10.3 us                                                                      | 9.98 us: 1.03x faster                                                |
| pickle_list          | 4.46 us                                                                      | 4.34 us: 1.03x faster                                                |
| xml_etree_iterparse  | 107 ms                                                                       | 105 ms: 1.02x faster                                                 |
| unpickle_pure_python | 213 us                                                                       | 211 us: 1.01x faster                                                 |
| pickle_pure_python   | 312 us                                                                       | 308 us: 1.01x faster                                                 |
| xml_etree_process    | 58.5 ms                                                                      | 58.7 ms: 1.00x slower                                                |
| unpickle             | 14.5 us                                                                      | 14.6 us: 1.01x slower                                                |
| tomli_loads          | 2.23 sec                                                                     | 2.35 sec: 1.05x slower                                               |
| Geometric mean       | (ref)                                                                        | 1.01x faster                                                         |

Benchmark hidden because not significant (4): json_loads, xml_etree_generate, xml_etree_parse, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 11.2 ms                                                                      | 11.3 ms: 1.00x slower                                                |
| python_startup         | 12.8 ms                                                                      | 12.8 ms: 1.00x slower                                                |
| Geometric mean         | (ref)                                                                        | 1.00x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.2 ms                                                                      | 10.3 ms: 1.01x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-pythonperf2-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| gc_traversal               | 3.75 ms                                                                      | 3.57 ms: 1.05x faster                                                |
| scimark_fft                | 314 ms                                                                       | 299 ms: 1.05x faster                                                 |
| unpickle_list              | 4.71 us                                                                      | 4.54 us: 1.04x faster                                                |
| scimark_monte_carlo        | 67.4 ms                                                                      | 65.0 ms: 1.04x faster                                                |
| pickle_dict                | 32.8 us                                                                      | 31.6 us: 1.04x faster                                                |
| float                      | 79.4 ms                                                                      | 76.8 ms: 1.03x faster                                                |
| logging_format             | 7.51 us                                                                      | 7.27 us: 1.03x faster                                                |
| scimark_sor                | 149 ms                                                                       | 144 ms: 1.03x faster                                                 |
| pickle                     | 10.3 us                                                                      | 9.98 us: 1.03x faster                                                |
| typing_runtime_protocols   | 126 us                                                                       | 122 us: 1.03x faster                                                 |
| chaos                      | 62.0 ms                                                                      | 60.2 ms: 1.03x faster                                                |
| raytrace                   | 278 ms                                                                       | 270 ms: 1.03x faster                                                 |
| pickle_list                | 4.46 us                                                                      | 4.34 us: 1.03x faster                                                |
| scimark_lu                 | 102 ms                                                                       | 99.5 ms: 1.03x faster                                                |
| fannkuch                   | 390 ms                                                                       | 380 ms: 1.03x faster                                                 |
| coroutines                 | 22.5 ms                                                                      | 22.0 ms: 1.02x faster                                                |
| scimark_sparse_mat_mult    | 4.25 ms                                                                      | 4.16 ms: 1.02x faster                                                |
| logging_simple             | 6.68 us                                                                      | 6.54 us: 1.02x faster                                                |
| xml_etree_iterparse        | 107 ms                                                                       | 105 ms: 1.02x faster                                                 |
| sqlglot_parse              | 1.41 ms                                                                      | 1.39 ms: 1.02x faster                                                |
| nbody                      | 85.9 ms                                                                      | 84.3 ms: 1.02x faster                                                |
| comprehensions             | 16.9 us                                                                      | 16.6 us: 1.02x faster                                                |
| sqlglot_optimize           | 58.6 ms                                                                      | 57.7 ms: 1.02x faster                                                |
| sqlglot_transpile          | 1.82 ms                                                                      | 1.79 ms: 1.02x faster                                                |
| coverage                   | 80.6 ms                                                                      | 79.4 ms: 1.01x faster                                                |
| logging_silent             | 97.0 ns                                                                      | 95.6 ns: 1.01x faster                                                |
| deepcopy_memo              | 37.8 us                                                                      | 37.3 us: 1.01x faster                                                |
| unpickle_pure_python       | 213 us                                                                       | 211 us: 1.01x faster                                                 |
| deepcopy                   | 373 us                                                                       | 368 us: 1.01x faster                                                 |
| pickle_pure_python         | 312 us                                                                       | 308 us: 1.01x faster                                                 |
| hexiom                     | 6.47 ms                                                                      | 6.41 ms: 1.01x faster                                                |
| sqlglot_normalize          | 116 ms                                                                       | 115 ms: 1.01x faster                                                 |
| regex_effbot               | 3.46 ms                                                                      | 3.44 ms: 1.01x faster                                                |
| regex_v8                   | 24.8 ms                                                                      | 24.7 ms: 1.01x faster                                                |
| nqueens                    | 88.3 ms                                                                      | 87.9 ms: 1.00x faster                                                |
| python_startup_no_site     | 11.2 ms                                                                      | 11.3 ms: 1.00x slower                                                |
| python_startup             | 12.8 ms                                                                      | 12.8 ms: 1.00x slower                                                |
| sympy_integrate            | 23.0 ms                                                                      | 23.0 ms: 1.00x slower                                                |
| pyflate                    | 505 ms                                                                       | 507 ms: 1.00x slower                                                 |
| regex_compile              | 145 ms                                                                       | 146 ms: 1.00x slower                                                 |
| sympy_str                  | 290 ms                                                                       | 291 ms: 1.00x slower                                                 |
| xml_etree_process          | 58.5 ms                                                                      | 58.7 ms: 1.00x slower                                                |
| dulwich_log                | 67.7 ms                                                                      | 68.0 ms: 1.01x slower                                                |
| 2to3                       | 293 ms                                                                       | 294 ms: 1.01x slower                                                 |
| mdp                        | 2.52 sec                                                                     | 2.53 sec: 1.01x slower                                               |
| async_tree_io_tg           | 1.09 sec                                                                     | 1.10 sec: 1.01x slower                                               |
| json                       | 5.22 ms                                                                      | 5.27 ms: 1.01x slower                                                |
| unpickle                   | 14.5 us                                                                      | 14.6 us: 1.01x slower                                                |
| spectral_norm              | 90.5 ms                                                                      | 91.5 ms: 1.01x slower                                                |
| meteor_contest             | 129 ms                                                                       | 130 ms: 1.01x slower                                                 |
| pidigits                   | 264 ms                                                                       | 267 ms: 1.01x slower                                                 |
| mako                       | 10.2 ms                                                                      | 10.3 ms: 1.01x slower                                                |
| sympy_expand               | 490 ms                                                                       | 496 ms: 1.01x slower                                                 |
| go                         | 167 ms                                                                       | 169 ms: 1.01x slower                                                 |
| generators                 | 34.3 ms                                                                      | 34.8 ms: 1.01x slower                                                |
| richards                   | 53.9 ms                                                                      | 54.6 ms: 1.01x slower                                                |
| pathlib                    | 19.0 ms                                                                      | 19.3 ms: 1.01x slower                                                |
| async_tree_none_tg         | 436 ms                                                                       | 444 ms: 1.02x slower                                                 |
| regex_dna                  | 236 ms                                                                       | 240 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed    | 699 ms                                                                       | 713 ms: 1.02x slower                                                 |
| async_tree_cpu_io_mixed_tg | 715 ms                                                                       | 734 ms: 1.03x slower                                                 |
| pprint_pformat             | 1.58 sec                                                                     | 1.64 sec: 1.04x slower                                               |
| pprint_safe_repr           | 773 ms                                                                       | 804 ms: 1.04x slower                                                 |
| tomli_loads                | 2.23 sec                                                                     | 2.35 sec: 1.05x slower                                               |
| unpack_sequence            | 48.3 ns                                                                      | 51.7 ns: 1.07x slower                                                |
| crypto_pyaes               | 69.6 ms                                                                      | 74.9 ms: 1.08x slower                                                |
| Geometric mean             | (ref)                                                                        | 1.00x faster                                                         |

Benchmark hidden because not significant (26): bench_mp_pool, json_loads, sqlite_synth, mypy2, pycparser, deltablue, richards_super, xml_etree_generate, tornado_http, asyncio_tcp_ssl, xml_etree_parse, asyncio_tcp, asyncio_websockets, docutils, async_generators, sympy_sum, async_tree_io, json_dumps, chameleon, bench_thread_pool, async_tree_memoization, create_gc_cycles, deepcopy_reduce, telco, async_tree_memoization_tg, async_tree_none
Ignored benchmarks (1) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: dask


# HPT report

- Reliability score: 78.65% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x