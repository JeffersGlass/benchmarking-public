# Results vs. base

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 840006e
- commit date: 2023-12-18
- overall geometric mean: 1.01x slower
- HPT reliability: 81.48%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 266 ms: 1.01x slower                                                   |
| chameleon      | 7.00 ms                                                                | 7.08 ms: 1.01x slower                                                  |
| docutils       | 2.61 sec                                                               | 2.60 sec: 1.00x faster                                                 |
| tornado_http   | 94.3 ms                                                                | 95.2 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_memoization     | 568 ms                                                                 | 561 ms: 1.01x faster                                                   |
| async_tree_none_tg         | 457 ms                                                                 | 453 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 1.22 sec                                                               | 1.22 sec: 1.00x faster                                                 |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 861 ms: 1.17x slower                                                   |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 831 ms: 1.17x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_io, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 92.4 ms                                                                | 89.2 ms: 1.04x faster                                                  |
| float          | 80.9 ms                                                                | 81.9 ms: 1.01x slower                                                  |
| pidigits       | 196 ms                                                                 | 288 ms: 1.47x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.13x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.68 ms                                                                | 3.52 ms: 1.04x faster                                                  |
| regex_v8       | 25.7 ms                                                                | 24.9 ms: 1.03x faster                                                  |
| regex_dna      | 219 ms                                                                 | 220 ms: 1.00x slower                                                   |
| regex_compile  | 133 ms                                                                 | 135 ms: 1.02x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle               | 11.6 us                                                                | 11.2 us: 1.04x faster                                                  |
| unpickle             | 15.5 us                                                                | 14.9 us: 1.04x faster                                                  |
| unpickle_list        | 5.04 us                                                                | 4.87 us: 1.04x faster                                                  |
| xml_etree_process    | 59.4 ms                                                                | 59.1 ms: 1.00x faster                                                  |
| json_dumps           | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                                  |
| xml_etree_iterparse  | 106 ms                                                                 | 106 ms: 1.01x slower                                                   |
| xml_etree_parse      | 157 ms                                                                 | 158 ms: 1.01x slower                                                   |
| pickle_pure_python   | 302 us                                                                 | 305 us: 1.01x slower                                                   |
| unpickle_pure_python | 217 us                                                                 | 222 us: 1.02x slower                                                   |
| pickle_dict          | 34.3 us                                                                | 35.3 us: 1.03x slower                                                  |
| pickle_list          | 5.09 us                                                                | 5.33 us: 1.05x slower                                                  |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (3): tomli_loads, json_loads, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup_no_site | 9.01 ms                                                                | 8.99 ms: 1.00x faster                                                  |
| python_startup         | 10.4 ms                                                                | 10.4 ms: 1.00x faster                                                  |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                           |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| gc_traversal               | 4.16 ms                                                                | 3.59 ms: 1.16x faster                                                  |
| unpack_sequence            | 46.6 ns                                                                | 43.3 ns: 1.08x faster                                                  |
| regex_effbot               | 3.68 ms                                                                | 3.52 ms: 1.04x faster                                                  |
| pickle                     | 11.6 us                                                                | 11.2 us: 1.04x faster                                                  |
| unpickle                   | 15.5 us                                                                | 14.9 us: 1.04x faster                                                  |
| nbody                      | 92.4 ms                                                                | 89.2 ms: 1.04x faster                                                  |
| unpickle_list              | 5.04 us                                                                | 4.87 us: 1.04x faster                                                  |
| spectral_norm              | 112 ms                                                                 | 108 ms: 1.03x faster                                                   |
| regex_v8                   | 25.7 ms                                                                | 24.9 ms: 1.03x faster                                                  |
| pycparser                  | 1.20 sec                                                               | 1.17 sec: 1.03x faster                                                 |
| scimark_fft                | 366 ms                                                                 | 357 ms: 1.02x faster                                                   |
| pyflate                    | 459 ms                                                                 | 448 ms: 1.02x faster                                                   |
| scimark_sparse_mat_mult    | 5.02 ms                                                                | 4.91 ms: 1.02x faster                                                  |
| coroutines                 | 21.7 ms                                                                | 21.3 ms: 1.02x faster                                                  |
| mdp                        | 2.56 sec                                                               | 2.51 sec: 1.02x faster                                                 |
| coverage                   | 95.4 ms                                                                | 93.7 ms: 1.02x faster                                                  |
| scimark_monte_carlo        | 69.3 ms                                                                | 68.1 ms: 1.02x faster                                                  |
| typing_runtime_protocols   | 117 us                                                                 | 116 us: 1.01x faster                                                   |
| sqlite_synth               | 2.81 us                                                                | 2.77 us: 1.01x faster                                                  |
| async_tree_memoization     | 568 ms                                                                 | 561 ms: 1.01x faster                                                   |
| nqueens                    | 80.0 ms                                                                | 79.1 ms: 1.01x faster                                                  |
| go                         | 142 ms                                                                 | 141 ms: 1.01x faster                                                   |
| chaos                      | 60.9 ms                                                                | 60.3 ms: 1.01x faster                                                  |
| async_tree_none_tg         | 457 ms                                                                 | 453 ms: 1.01x faster                                                   |
| json                       | 5.19 ms                                                                | 5.15 ms: 1.01x faster                                                  |
| pathlib                    | 18.1 ms                                                                | 18.0 ms: 1.01x faster                                                  |
| meteor_contest             | 109 ms                                                                 | 109 ms: 1.00x faster                                                   |
| xml_etree_process          | 59.4 ms                                                                | 59.1 ms: 1.00x faster                                                  |
| async_tree_io_tg           | 1.22 sec                                                               | 1.22 sec: 1.00x faster                                                 |
| docutils                   | 2.61 sec                                                               | 2.60 sec: 1.00x faster                                                 |
| python_startup_no_site     | 9.01 ms                                                                | 8.99 ms: 1.00x faster                                                  |
| python_startup             | 10.4 ms                                                                | 10.4 ms: 1.00x faster                                                  |
| sympy_integrate            | 19.5 ms                                                                | 19.5 ms: 1.00x slower                                                  |
| regex_dna                  | 219 ms                                                                 | 220 ms: 1.00x slower                                                   |
| bench_thread_pool          | 828 us                                                                 | 832 us: 1.00x slower                                                   |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.79 sec: 1.00x slower                                                 |
| json_dumps                 | 10.4 ms                                                                | 10.4 ms: 1.01x slower                                                  |
| xml_etree_iterparse        | 106 ms                                                                 | 106 ms: 1.01x slower                                                   |
| comprehensions             | 16.3 us                                                                | 16.4 us: 1.01x slower                                                  |
| asyncio_tcp                | 483 ms                                                                 | 486 ms: 1.01x slower                                                   |
| create_gc_cycles           | 1.46 ms                                                                | 1.47 ms: 1.01x slower                                                  |
| sympy_sum                  | 147 ms                                                                 | 148 ms: 1.01x slower                                                   |
| deepcopy_memo              | 39.0 us                                                                | 39.3 us: 1.01x slower                                                  |
| xml_etree_parse            | 157 ms                                                                 | 158 ms: 1.01x slower                                                   |
| sympy_expand               | 451 ms                                                                 | 456 ms: 1.01x slower                                                   |
| pickle_pure_python         | 302 us                                                                 | 305 us: 1.01x slower                                                   |
| tornado_http               | 94.3 ms                                                                | 95.2 ms: 1.01x slower                                                  |
| pprint_pformat             | 1.51 sec                                                               | 1.53 sec: 1.01x slower                                                 |
| sqlglot_optimize           | 53.5 ms                                                                | 54.1 ms: 1.01x slower                                                  |
| chameleon                  | 7.00 ms                                                                | 7.08 ms: 1.01x slower                                                  |
| scimark_lu                 | 115 ms                                                                 | 117 ms: 1.01x slower                                                   |
| float                      | 80.9 ms                                                                | 81.9 ms: 1.01x slower                                                  |
| 2to3                       | 263 ms                                                                 | 266 ms: 1.01x slower                                                   |
| sqlglot_normalize          | 105 ms                                                                 | 107 ms: 1.01x slower                                                   |
| generators                 | 28.6 ms                                                                | 29.0 ms: 1.01x slower                                                  |
| pprint_safe_repr           | 739 ms                                                                 | 749 ms: 1.01x slower                                                   |
| sqlglot_parse              | 1.26 ms                                                                | 1.28 ms: 1.02x slower                                                  |
| deepcopy_reduce            | 3.09 us                                                                | 3.14 us: 1.02x slower                                                  |
| deepcopy                   | 349 us                                                                 | 355 us: 1.02x slower                                                   |
| regex_compile              | 133 ms                                                                 | 135 ms: 1.02x slower                                                   |
| sqlglot_transpile          | 1.57 ms                                                                | 1.60 ms: 1.02x slower                                                  |
| logging_silent             | 104 ns                                                                 | 107 ns: 1.02x slower                                                   |
| sympy_str                  | 267 ms                                                                 | 273 ms: 1.02x slower                                                   |
| async_generators           | 443 ms                                                                 | 453 ms: 1.02x slower                                                   |
| unpickle_pure_python       | 217 us                                                                 | 222 us: 1.02x slower                                                   |
| crypto_pyaes               | 70.9 ms                                                                | 72.7 ms: 1.03x slower                                                  |
| raytrace                   | 272 ms                                                                 | 279 ms: 1.03x slower                                                   |
| richards_super             | 53.3 ms                                                                | 54.7 ms: 1.03x slower                                                  |
| hexiom                     | 6.09 ms                                                                | 6.25 ms: 1.03x slower                                                  |
| deltablue                  | 3.25 ms                                                                | 3.34 ms: 1.03x slower                                                  |
| pickle_dict                | 34.3 us                                                                | 35.3 us: 1.03x slower                                                  |
| scimark_sor                | 123 ms                                                                 | 128 ms: 1.04x slower                                                   |
| pickle_list                | 5.09 us                                                                | 5.33 us: 1.05x slower                                                  |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 861 ms: 1.17x slower                                                   |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 831 ms: 1.17x slower                                                   |
| pidigits                   | 196 ms                                                                 | 288 ms: 1.47x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (16): logging_format, async_tree_memoization_tg, telco, tomli_loads, mypy2, json_loads, xml_etree_generate, dulwich_log, fannkuch, mako, bench_mp_pool, asyncio_websockets, async_tree_io, logging_simple, async_tree_none, richards
Ignored benchmarks (1) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: dask


# HPT report

- Reliability score: 81.48% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x