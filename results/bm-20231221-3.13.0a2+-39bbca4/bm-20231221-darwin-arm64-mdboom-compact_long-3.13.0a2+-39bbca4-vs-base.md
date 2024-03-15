# Results vs. base

- fork: mdboom
- ref: compact_long
- machine: darwin-arm64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.01x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 175 ms                                                                 | 178 ms: 1.02x slower                                           |
| chameleon      | 5.13 ms                                                                | 5.16 ms: 1.01x slower                                          |
| docutils       | 1.50 sec                                                               | 1.51 sec: 1.01x slower                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none_tg         | 268 ms                                                                 | 270 ms: 1.01x slower                                           |
| async_tree_io              | 706 ms                                                                 | 713 ms: 1.01x slower                                           |
| async_tree_cpu_io_mixed_tg | 543 ms                                                                 | 550 ms: 1.01x slower                                           |
| async_tree_io_tg           | 686 ms                                                                 | 695 ms: 1.01x slower                                           |
| async_tree_cpu_io_mixed    | 526 ms                                                                 | 534 ms: 1.02x slower                                           |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (3): async_tree_none, async_tree_memoization, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 282 ms                                                                 | 274 ms: 1.03x faster                                           |
| nbody          | 82.1 ms                                                                | 81.7 ms: 1.00x faster                                          |
| float          | 58.0 ms                                                                | 58.5 ms: 1.01x slower                                          |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_v8       | 16.9 ms                                                                | 16.9 ms: 1.00x slower                                          |
| regex_compile  | 79.3 ms                                                                | 80.5 ms: 1.01x slower                                          |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (2): regex_dna, regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle               | 7.47 us                                                                | 7.36 us: 1.02x faster                                          |
| unpickle_list        | 3.14 us                                                                | 3.12 us: 1.01x faster                                          |
| unpickle             | 9.07 us                                                                | 9.13 us: 1.01x slower                                          |
| unpickle_pure_python | 165 us                                                                 | 166 us: 1.01x slower                                           |
| pickle_dict          | 17.9 us                                                                | 18.1 us: 1.01x slower                                          |
| json_loads           | 17.2 us                                                                | 17.4 us: 1.01x slower                                          |
| xml_etree_iterparse  | 76.1 ms                                                                | 77.1 ms: 1.01x slower                                          |
| pickle_list          | 2.88 us                                                                | 2.92 us: 1.01x slower                                          |
| json_dumps           | 6.59 ms                                                                | 6.72 ms: 1.02x slower                                          |
| xml_etree_process    | 40.7 ms                                                                | 42.0 ms: 1.03x slower                                          |
| xml_etree_generate   | 58.4 ms                                                                | 60.9 ms: 1.04x slower                                          |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (3): tomli_loads, pickle_pure_python, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 13.2 ms                                                                | 13.3 ms: 1.01x slower                                          |
| python_startup_no_site | 11.8 ms                                                                | 11.9 ms: 1.01x slower                                          |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.78 ms                                                                | 7.90 ms: 1.02x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| gc_traversal               | 2.54 ms                                                                | 2.40 ms: 1.06x faster                                          |
| pidigits                   | 282 ms                                                                 | 274 ms: 1.03x faster                                           |
| comprehensions             | 12.7 us                                                                | 12.4 us: 1.02x faster                                          |
| pickle                     | 7.47 us                                                                | 7.36 us: 1.02x faster                                          |
| unpickle_list              | 3.14 us                                                                | 3.12 us: 1.01x faster                                          |
| scimark_sor                | 107 ms                                                                 | 106 ms: 1.01x faster                                           |
| fannkuch                   | 289 ms                                                                 | 287 ms: 1.01x faster                                           |
| hexiom                     | 5.02 ms                                                                | 5.00 ms: 1.00x faster                                          |
| nbody                      | 82.1 ms                                                                | 81.7 ms: 1.00x faster                                          |
| dulwich_log                | 30.2 ms                                                                | 30.1 ms: 1.00x faster                                          |
| asyncio_websockets         | 410 ms                                                                 | 408 ms: 1.00x faster                                           |
| regex_v8                   | 16.9 ms                                                                | 16.9 ms: 1.00x slower                                          |
| create_gc_cycles           | 703 us                                                                 | 706 us: 1.00x slower                                           |
| chameleon                  | 5.13 ms                                                                | 5.16 ms: 1.01x slower                                          |
| unpickle                   | 9.07 us                                                                | 9.13 us: 1.01x slower                                          |
| pyflate                    | 344 ms                                                                 | 346 ms: 1.01x slower                                           |
| unpickle_pure_python       | 165 us                                                                 | 166 us: 1.01x slower                                           |
| docutils                   | 1.50 sec                                                               | 1.51 sec: 1.01x slower                                         |
| scimark_monte_carlo        | 48.5 ms                                                                | 48.9 ms: 1.01x slower                                          |
| coverage                   | 48.0 ms                                                                | 48.3 ms: 1.01x slower                                          |
| chaos                      | 43.2 ms                                                                | 43.5 ms: 1.01x slower                                          |
| json                       | 3.04 ms                                                                | 3.07 ms: 1.01x slower                                          |
| python_startup             | 13.2 ms                                                                | 13.3 ms: 1.01x slower                                          |
| async_tree_none_tg         | 268 ms                                                                 | 270 ms: 1.01x slower                                           |
| float                      | 58.0 ms                                                                | 58.5 ms: 1.01x slower                                          |
| pickle_dict                | 17.9 us                                                                | 18.1 us: 1.01x slower                                          |
| json_loads                 | 17.2 us                                                                | 17.4 us: 1.01x slower                                          |
| raytrace                   | 184 ms                                                                 | 185 ms: 1.01x slower                                           |
| spectral_norm              | 75.1 ms                                                                | 75.8 ms: 1.01x slower                                          |
| sqlglot_parse              | 829 us                                                                 | 837 us: 1.01x slower                                           |
| async_generators           | 305 ms                                                                 | 308 ms: 1.01x slower                                           |
| sqlglot_transpile          | 1.01 ms                                                                | 1.02 ms: 1.01x slower                                          |
| generators                 | 26.1 ms                                                                | 26.3 ms: 1.01x slower                                          |
| sympy_sum                  | 75.9 ms                                                                | 76.7 ms: 1.01x slower                                          |
| telco                      | 4.72 ms                                                                | 4.77 ms: 1.01x slower                                          |
| async_tree_io              | 706 ms                                                                 | 713 ms: 1.01x slower                                           |
| scimark_sparse_mat_mult    | 3.17 ms                                                                | 3.20 ms: 1.01x slower                                          |
| sqlglot_normalize          | 192 ms                                                                 | 194 ms: 1.01x slower                                           |
| sqlglot_optimize           | 35.8 ms                                                                | 36.2 ms: 1.01x slower                                          |
| python_startup_no_site     | 11.8 ms                                                                | 11.9 ms: 1.01x slower                                          |
| async_tree_cpu_io_mixed_tg | 543 ms                                                                 | 550 ms: 1.01x slower                                           |
| nqueens                    | 63.0 ms                                                                | 63.8 ms: 1.01x slower                                          |
| coroutines                 | 19.3 ms                                                                | 19.5 ms: 1.01x slower                                          |
| go                         | 106 ms                                                                 | 107 ms: 1.01x slower                                           |
| meteor_contest             | 75.3 ms                                                                | 76.3 ms: 1.01x slower                                          |
| async_tree_io_tg           | 686 ms                                                                 | 695 ms: 1.01x slower                                           |
| xml_etree_iterparse        | 76.1 ms                                                                | 77.1 ms: 1.01x slower                                          |
| unpack_sequence            | 29.0 ns                                                                | 29.5 ns: 1.01x slower                                          |
| logging_silent             | 71.0 ns                                                                | 72.0 ns: 1.01x slower                                          |
| pickle_list                | 2.88 us                                                                | 2.92 us: 1.01x slower                                          |
| deltablue                  | 2.45 ms                                                                | 2.48 ms: 1.01x slower                                          |
| regex_compile              | 79.3 ms                                                                | 80.5 ms: 1.01x slower                                          |
| sympy_integrate            | 11.2 ms                                                                | 11.3 ms: 1.01x slower                                          |
| async_tree_cpu_io_mixed    | 526 ms                                                                 | 534 ms: 1.02x slower                                           |
| scimark_lu                 | 75.9 ms                                                                | 77.1 ms: 1.02x slower                                          |
| mako                       | 7.78 ms                                                                | 7.90 ms: 1.02x slower                                          |
| sympy_expand               | 254 ms                                                                 | 258 ms: 1.02x slower                                           |
| 2to3                       | 175 ms                                                                 | 178 ms: 1.02x slower                                           |
| pprint_pformat             | 1.09 sec                                                               | 1.11 sec: 1.02x slower                                         |
| json_dumps                 | 6.59 ms                                                                | 6.72 ms: 1.02x slower                                          |
| pprint_safe_repr           | 536 ms                                                                 | 547 ms: 1.02x slower                                           |
| bench_thread_pool          | 516 us                                                                 | 527 us: 1.02x slower                                           |
| sympy_str                  | 147 ms                                                                 | 150 ms: 1.02x slower                                           |
| deepcopy_reduce            | 2.07 us                                                                | 2.12 us: 1.02x slower                                          |
| typing_runtime_protocols   | 77.5 us                                                                | 79.4 us: 1.02x slower                                          |
| logging_format             | 3.95 us                                                                | 4.06 us: 1.03x slower                                          |
| deepcopy                   | 232 us                                                                 | 240 us: 1.03x slower                                           |
| xml_etree_process          | 40.7 ms                                                                | 42.0 ms: 1.03x slower                                          |
| mdp                        | 1.66 sec                                                               | 1.72 sec: 1.04x slower                                         |
| logging_simple             | 3.63 us                                                                | 3.76 us: 1.04x slower                                          |
| deepcopy_memo              | 26.0 us                                                                | 27.0 us: 1.04x slower                                          |
| xml_etree_generate         | 58.4 ms                                                                | 60.9 ms: 1.04x slower                                          |
| crypto_pyaes               | 48.9 ms                                                                | 50.9 ms: 1.04x slower                                          |
| richards                   | 35.2 ms                                                                | 36.8 ms: 1.04x slower                                          |
| richards_super             | 38.9 ms                                                                | 40.7 ms: 1.04x slower                                          |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (17): tornado_http, pathlib, tomli_loads, regex_dna, scimark_fft, regex_effbot, sqlite_synth, pickle_pure_python, pycparser, mypy2, asyncio_tcp_ssl, xml_etree_parse, async_tree_none, async_tree_memoization, bench_mp_pool, async_tree_memoization_tg, asyncio_tcp
Ignored benchmarks (1) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: dask


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x