# Results vs. base

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 2f0a32b
- commit date: 2023-12-19
- overall geometric mean: 1.01x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 266 ms: 1.01x slower                                                   |
| chameleon      | 7.00 ms                                                                | 7.07 ms: 1.01x slower                                                  |
| tornado_http   | 94.3 ms                                                                | 95.2 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_io_tg           | 1.22 sec                                                               | 1.23 sec: 1.01x slower                                                 |
| async_tree_io              | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                                 |
| async_tree_memoization_tg  | 598 ms                                                                 | 607 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 728 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 758 ms: 1.03x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (3): async_tree_memoization, async_tree_none_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 92.4 ms                                                                | 90.5 ms: 1.02x faster                                                  |
| float          | 80.9 ms                                                                | 82.4 ms: 1.02x slower                                                  |
| pidigits       | 196 ms                                                                 | 228 ms: 1.16x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.05x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.68 ms                                                                | 3.60 ms: 1.02x faster                                                  |
| regex_dna      | 219 ms                                                                 | 216 ms: 1.01x faster                                                   |
| regex_compile  | 133 ms                                                                 | 135 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle             | 15.5 us                                                                | 15.0 us: 1.03x faster                                                  |
| unpickle_list        | 5.04 us                                                                | 4.93 us: 1.02x faster                                                  |
| pickle               | 11.6 us                                                                | 11.4 us: 1.02x faster                                                  |
| pickle_list          | 5.09 us                                                                | 4.98 us: 1.02x faster                                                  |
| pickle_dict          | 34.3 us                                                                | 34.1 us: 1.00x faster                                                  |
| json_loads           | 28.2 us                                                                | 28.4 us: 1.01x slower                                                  |
| json_dumps           | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                                  |
| xml_etree_parse      | 157 ms                                                                 | 158 ms: 1.01x slower                                                   |
| tomli_loads          | 2.14 sec                                                               | 2.18 sec: 1.02x slower                                                 |
| pickle_pure_python   | 302 us                                                                 | 307 us: 1.02x slower                                                   |
| unpickle_pure_python | 217 us                                                                 | 224 us: 1.03x slower                                                   |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (3): xml_etree_generate, xml_etree_process, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.4 ms                                                                | 10.4 ms: 1.00x slower                                                  |
| python_startup_no_site | 9.01 ms                                                                | 9.04 ms: 1.00x slower                                                  |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.4 ms                                                                | 11.2 ms: 1.01x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| gc_traversal               | 4.16 ms                                                                | 3.82 ms: 1.09x faster                                                  |
| unpickle                   | 15.5 us                                                                | 15.0 us: 1.03x faster                                                  |
| unpickle_list              | 5.04 us                                                                | 4.93 us: 1.02x faster                                                  |
| regex_effbot               | 3.68 ms                                                                | 3.60 ms: 1.02x faster                                                  |
| pickle                     | 11.6 us                                                                | 11.4 us: 1.02x faster                                                  |
| nbody                      | 92.4 ms                                                                | 90.5 ms: 1.02x faster                                                  |
| pickle_list                | 5.09 us                                                                | 4.98 us: 1.02x faster                                                  |
| regex_dna                  | 219 ms                                                                 | 216 ms: 1.01x faster                                                   |
| mako                       | 11.4 ms                                                                | 11.2 ms: 1.01x faster                                                  |
| scimark_monte_carlo        | 69.3 ms                                                                | 68.5 ms: 1.01x faster                                                  |
| asyncio_tcp                | 483 ms                                                                 | 479 ms: 1.01x faster                                                   |
| pickle_dict                | 34.3 us                                                                | 34.1 us: 1.00x faster                                                  |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.78 sec: 1.00x slower                                                 |
| python_startup             | 10.4 ms                                                                | 10.4 ms: 1.00x slower                                                  |
| python_startup_no_site     | 9.01 ms                                                                | 9.04 ms: 1.00x slower                                                  |
| sympy_integrate            | 19.5 ms                                                                | 19.5 ms: 1.00x slower                                                  |
| json_loads                 | 28.2 us                                                                | 28.4 us: 1.01x slower                                                  |
| raytrace                   | 272 ms                                                                 | 274 ms: 1.01x slower                                                   |
| pathlib                    | 18.1 ms                                                                | 18.2 ms: 1.01x slower                                                  |
| sympy_sum                  | 147 ms                                                                 | 148 ms: 1.01x slower                                                   |
| json_dumps                 | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                                  |
| go                         | 142 ms                                                                 | 143 ms: 1.01x slower                                                   |
| async_generators           | 443 ms                                                                 | 446 ms: 1.01x slower                                                   |
| unpack_sequence            | 46.6 ns                                                                | 46.9 ns: 1.01x slower                                                  |
| bench_thread_pool          | 828 us                                                                 | 834 us: 1.01x slower                                                   |
| xml_etree_parse            | 157 ms                                                                 | 158 ms: 1.01x slower                                                   |
| dulwich_log                | 65.5 ms                                                                | 66.0 ms: 1.01x slower                                                  |
| logging_simple             | 5.74 us                                                                | 5.79 us: 1.01x slower                                                  |
| async_tree_io_tg           | 1.22 sec                                                               | 1.23 sec: 1.01x slower                                                 |
| tornado_http               | 94.3 ms                                                                | 95.2 ms: 1.01x slower                                                  |
| async_tree_io              | 1.18 sec                                                               | 1.19 sec: 1.01x slower                                                 |
| chameleon                  | 7.00 ms                                                                | 7.07 ms: 1.01x slower                                                  |
| create_gc_cycles           | 1.46 ms                                                                | 1.48 ms: 1.01x slower                                                  |
| 2to3                       | 263 ms                                                                 | 266 ms: 1.01x slower                                                   |
| pycparser                  | 1.20 sec                                                               | 1.22 sec: 1.01x slower                                                 |
| scimark_fft                | 366 ms                                                                 | 371 ms: 1.01x slower                                                   |
| sqlglot_normalize          | 105 ms                                                                 | 107 ms: 1.01x slower                                                   |
| sqlglot_optimize           | 53.5 ms                                                                | 54.3 ms: 1.01x slower                                                  |
| async_tree_memoization_tg  | 598 ms                                                                 | 607 ms: 1.01x slower                                                   |
| regex_compile              | 133 ms                                                                 | 135 ms: 1.01x slower                                                   |
| meteor_contest             | 109 ms                                                                 | 111 ms: 1.02x slower                                                   |
| deepcopy_reduce            | 3.09 us                                                                | 3.14 us: 1.02x slower                                                  |
| logging_silent             | 104 ns                                                                 | 106 ns: 1.02x slower                                                   |
| fannkuch                   | 394 ms                                                                 | 401 ms: 1.02x slower                                                   |
| sympy_expand               | 451 ms                                                                 | 460 ms: 1.02x slower                                                   |
| scimark_sor                | 123 ms                                                                 | 126 ms: 1.02x slower                                                   |
| tomli_loads                | 2.14 sec                                                               | 2.18 sec: 1.02x slower                                                 |
| pickle_pure_python         | 302 us                                                                 | 307 us: 1.02x slower                                                   |
| float                      | 80.9 ms                                                                | 82.4 ms: 1.02x slower                                                  |
| nqueens                    | 80.0 ms                                                                | 81.7 ms: 1.02x slower                                                  |
| deepcopy                   | 349 us                                                                 | 356 us: 1.02x slower                                                   |
| comprehensions             | 16.3 us                                                                | 16.6 us: 1.02x slower                                                  |
| chaos                      | 60.9 ms                                                                | 62.2 ms: 1.02x slower                                                  |
| pyflate                    | 459 ms                                                                 | 469 ms: 1.02x slower                                                   |
| richards_super             | 53.3 ms                                                                | 54.5 ms: 1.02x slower                                                  |
| deepcopy_memo              | 39.0 us                                                                | 39.9 us: 1.02x slower                                                  |
| sqlglot_transpile          | 1.57 ms                                                                | 1.61 ms: 1.02x slower                                                  |
| sympy_str                  | 267 ms                                                                 | 273 ms: 1.02x slower                                                   |
| sqlglot_parse              | 1.26 ms                                                                | 1.29 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 728 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 758 ms: 1.03x slower                                                   |
| spectral_norm              | 112 ms                                                                 | 115 ms: 1.03x slower                                                   |
| scimark_sparse_mat_mult    | 5.02 ms                                                                | 5.17 ms: 1.03x slower                                                  |
| unpickle_pure_python       | 217 us                                                                 | 224 us: 1.03x slower                                                   |
| mdp                        | 2.56 sec                                                               | 2.64 sec: 1.03x slower                                                 |
| hexiom                     | 6.09 ms                                                                | 6.36 ms: 1.04x slower                                                  |
| generators                 | 28.6 ms                                                                | 30.0 ms: 1.05x slower                                                  |
| crypto_pyaes               | 70.9 ms                                                                | 74.4 ms: 1.05x slower                                                  |
| deltablue                  | 3.25 ms                                                                | 3.43 ms: 1.06x slower                                                  |
| pidigits                   | 196 ms                                                                 | 228 ms: 1.16x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (22): typing_runtime_protocols, sqlite_synth, async_tree_memoization, logging_format, coverage, xml_etree_generate, docutils, bench_mp_pool, pprint_pformat, asyncio_websockets, xml_etree_process, richards, regex_v8, async_tree_none_tg, xml_etree_iterparse, pprint_safe_repr, json, mypy2, coroutines, telco, scimark_lu, async_tree_none
Ignored benchmarks (1) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: dask


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x