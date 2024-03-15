# Results vs. base

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 522c622
- commit date: 2023-12-20
- overall geometric mean: 1.00x slower
- HPT reliability: 76.32%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 264 ms: 1.00x slower                                                   |
| chameleon      | 7.00 ms                                                                | 6.96 ms: 1.01x faster                                                  |
| docutils       | 2.61 sec                                                               | 2.60 sec: 1.01x faster                                                 |
| tornado_http   | 94.3 ms                                                                | 95.1 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_memoization     | 568 ms                                                                 | 562 ms: 1.01x faster                                                   |
| async_tree_none_tg         | 457 ms                                                                 | 454 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 1.22 sec                                                               | 1.22 sec: 1.00x faster                                                 |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 729 ms: 1.03x slower                                                   |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 758 ms: 1.03x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_io, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 92.4 ms                                                                | 89.7 ms: 1.03x faster                                                  |
| float          | 80.9 ms                                                                | 82.4 ms: 1.02x slower                                                  |
| pidigits       | 196 ms                                                                 | 223 ms: 1.14x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.04x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 25.7 ms                                                                | 24.6 ms: 1.05x faster                                                  |
| regex_compile  | 133 ms                                                                 | 134 ms: 1.01x slower                                                   |
| regex_dna      | 219 ms                                                                 | 221 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle             | 15.5 us                                                                | 14.3 us: 1.08x faster                                                  |
| unpickle_list        | 5.04 us                                                                | 4.88 us: 1.03x faster                                                  |
| pickle_list          | 5.09 us                                                                | 5.00 us: 1.02x faster                                                  |
| pickle               | 11.6 us                                                                | 11.5 us: 1.01x faster                                                  |
| xml_etree_generate   | 86.6 ms                                                                | 85.8 ms: 1.01x faster                                                  |
| json_loads           | 28.2 us                                                                | 28.1 us: 1.00x faster                                                  |
| pickle_dict          | 34.3 us                                                                | 34.4 us: 1.00x slower                                                  |
| tomli_loads          | 2.14 sec                                                               | 2.17 sec: 1.01x slower                                                 |
| xml_etree_parse      | 157 ms                                                                 | 159 ms: 1.01x slower                                                   |
| pickle_pure_python   | 302 us                                                                 | 308 us: 1.02x slower                                                   |
| unpickle_pure_python | 217 us                                                                 | 223 us: 1.03x slower                                                   |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (3): xml_etree_process, json_dumps, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.4 ms                                                                | 10.4 ms: 1.00x slower                                                  |
| python_startup_no_site | 9.01 ms                                                                | 9.04 ms: 1.00x slower                                                  |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.4 ms                                                                | 11.1 ms: 1.02x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle                   | 15.5 us                                                                | 14.3 us: 1.08x faster                                                  |
| regex_v8                   | 25.7 ms                                                                | 24.6 ms: 1.05x faster                                                  |
| pycparser                  | 1.20 sec                                                               | 1.16 sec: 1.03x faster                                                 |
| unpickle_list              | 5.04 us                                                                | 4.88 us: 1.03x faster                                                  |
| nbody                      | 92.4 ms                                                                | 89.7 ms: 1.03x faster                                                  |
| mako                       | 11.4 ms                                                                | 11.1 ms: 1.02x faster                                                  |
| pickle_list                | 5.09 us                                                                | 5.00 us: 1.02x faster                                                  |
| meteor_contest             | 109 ms                                                                 | 108 ms: 1.02x faster                                                   |
| coverage                   | 95.4 ms                                                                | 94.0 ms: 1.01x faster                                                  |
| go                         | 142 ms                                                                 | 140 ms: 1.01x faster                                                   |
| pickle                     | 11.6 us                                                                | 11.5 us: 1.01x faster                                                  |
| async_tree_memoization     | 568 ms                                                                 | 562 ms: 1.01x faster                                                   |
| json                       | 5.19 ms                                                                | 5.13 ms: 1.01x faster                                                  |
| deepcopy_memo              | 39.0 us                                                                | 38.7 us: 1.01x faster                                                  |
| xml_etree_generate         | 86.6 ms                                                                | 85.8 ms: 1.01x faster                                                  |
| pyflate                    | 459 ms                                                                 | 455 ms: 1.01x faster                                                   |
| scimark_monte_carlo        | 69.3 ms                                                                | 68.8 ms: 1.01x faster                                                  |
| chameleon                  | 7.00 ms                                                                | 6.96 ms: 1.01x faster                                                  |
| pprint_pformat             | 1.51 sec                                                               | 1.50 sec: 1.01x faster                                                 |
| async_tree_none_tg         | 457 ms                                                                 | 454 ms: 1.01x faster                                                   |
| pprint_safe_repr           | 739 ms                                                                 | 735 ms: 1.01x faster                                                   |
| docutils                   | 2.61 sec                                                               | 2.60 sec: 1.01x faster                                                 |
| json_loads                 | 28.2 us                                                                | 28.1 us: 1.00x faster                                                  |
| dulwich_log                | 65.5 ms                                                                | 65.3 ms: 1.00x faster                                                  |
| async_tree_io_tg           | 1.22 sec                                                               | 1.22 sec: 1.00x faster                                                 |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.78 sec: 1.00x faster                                                 |
| python_startup             | 10.4 ms                                                                | 10.4 ms: 1.00x slower                                                  |
| bench_thread_pool          | 828 us                                                                 | 830 us: 1.00x slower                                                   |
| python_startup_no_site     | 9.01 ms                                                                | 9.04 ms: 1.00x slower                                                  |
| pickle_dict                | 34.3 us                                                                | 34.4 us: 1.00x slower                                                  |
| 2to3                       | 263 ms                                                                 | 264 ms: 1.00x slower                                                   |
| comprehensions             | 16.3 us                                                                | 16.4 us: 1.00x slower                                                  |
| sqlglot_optimize           | 53.5 ms                                                                | 53.8 ms: 1.01x slower                                                  |
| pathlib                    | 18.1 ms                                                                | 18.2 ms: 1.01x slower                                                  |
| deepcopy                   | 349 us                                                                 | 351 us: 1.01x slower                                                   |
| logging_format             | 6.32 us                                                                | 6.36 us: 1.01x slower                                                  |
| regex_compile              | 133 ms                                                                 | 134 ms: 1.01x slower                                                   |
| tornado_http               | 94.3 ms                                                                | 95.1 ms: 1.01x slower                                                  |
| scimark_sor                | 123 ms                                                                 | 124 ms: 1.01x slower                                                   |
| regex_dna                  | 219 ms                                                                 | 221 ms: 1.01x slower                                                   |
| sympy_expand               | 451 ms                                                                 | 456 ms: 1.01x slower                                                   |
| nqueens                    | 80.0 ms                                                                | 81.0 ms: 1.01x slower                                                  |
| richards_super             | 53.3 ms                                                                | 54.0 ms: 1.01x slower                                                  |
| sqlglot_normalize          | 105 ms                                                                 | 107 ms: 1.01x slower                                                   |
| unpack_sequence            | 46.6 ns                                                                | 47.2 ns: 1.01x slower                                                  |
| tomli_loads                | 2.14 sec                                                               | 2.17 sec: 1.01x slower                                                 |
| sympy_str                  | 267 ms                                                                 | 271 ms: 1.01x slower                                                   |
| sqlglot_parse              | 1.26 ms                                                                | 1.28 ms: 1.01x slower                                                  |
| xml_etree_parse            | 157 ms                                                                 | 159 ms: 1.01x slower                                                   |
| async_generators           | 443 ms                                                                 | 450 ms: 1.02x slower                                                   |
| sqlglot_transpile          | 1.57 ms                                                                | 1.60 ms: 1.02x slower                                                  |
| scimark_fft                | 366 ms                                                                 | 372 ms: 1.02x slower                                                   |
| coroutines                 | 21.7 ms                                                                | 22.1 ms: 1.02x slower                                                  |
| deltablue                  | 3.25 ms                                                                | 3.31 ms: 1.02x slower                                                  |
| create_gc_cycles           | 1.46 ms                                                                | 1.49 ms: 1.02x slower                                                  |
| deepcopy_reduce            | 3.09 us                                                                | 3.15 us: 1.02x slower                                                  |
| float                      | 80.9 ms                                                                | 82.4 ms: 1.02x slower                                                  |
| fannkuch                   | 394 ms                                                                 | 402 ms: 1.02x slower                                                   |
| pickle_pure_python         | 302 us                                                                 | 308 us: 1.02x slower                                                   |
| scimark_lu                 | 115 ms                                                                 | 118 ms: 1.02x slower                                                   |
| hexiom                     | 6.09 ms                                                                | 6.23 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed    | 710 ms                                                                 | 729 ms: 1.03x slower                                                   |
| async_tree_cpu_io_mixed_tg | 738 ms                                                                 | 758 ms: 1.03x slower                                                   |
| unpickle_pure_python       | 217 us                                                                 | 223 us: 1.03x slower                                                   |
| crypto_pyaes               | 70.9 ms                                                                | 73.3 ms: 1.03x slower                                                  |
| gc_traversal               | 4.16 ms                                                                | 4.31 ms: 1.03x slower                                                  |
| mdp                        | 2.56 sec                                                               | 2.77 sec: 1.08x slower                                                 |
| pidigits                   | 196 ms                                                                 | 223 ms: 1.14x slower                                                   |
| Geometric mean             | (ref)                                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (24): xml_etree_process, sqlite_synth, logging_silent, sympy_sum, regex_effbot, raytrace, asyncio_tcp, spectral_norm, sympy_integrate, scimark_sparse_mat_mult, chaos, mypy2, bench_mp_pool, asyncio_websockets, async_tree_memoization_tg, json_dumps, generators, async_tree_io, telco, async_tree_none, xml_etree_iterparse, logging_simple, typing_runtime_protocols, richards
Ignored benchmarks (1) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-linux-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: dask


# HPT report

- Reliability score: 76.32% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x