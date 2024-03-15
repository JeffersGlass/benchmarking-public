
# Results vs. 3.12.0

- fork: mdboom
- ref: compact_long
- machine: linux-x86_64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                           |
| chameleon      | 7.41 ms                                                | 7.06 ms: 1.05x faster                                          |
| docutils       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                         |
| tornado_http   | 103 ms                                                 | 95.0 ms: 1.08x faster                                          |
| Geometric mean | (ref)                                                  | 1.06x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 438 ms: 1.08x faster                                           |
| async_tree_memoization     | 578 ms                                                 | 565 ms: 1.02x faster                                           |
| async_tree_none_tg         | 450 ms                                                 | 455 ms: 1.01x slower                                           |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.04x slower                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 597 ms: 1.04x slower                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 755 ms: 1.04x slower                                           |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 91.2 ms: 1.06x faster                                          |
| float          | 84.7 ms                                                | 81.9 ms: 1.03x faster                                          |
| pidigits       | 187 ms                                                 | 222 ms: 1.19x slower                                           |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 134 ms: 1.10x faster                                           |
| regex_effbot   | 3.61 ms                                                | 3.50 ms: 1.03x faster                                          |
| regex_dna      | 212 ms                                                 | 217 ms: 1.02x slower                                           |
| regex_v8       | 23.1 ms                                                | 24.4 ms: 1.05x slower                                          |
| Geometric mean | (ref)                                                  | 1.01x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.17 sec: 1.07x faster                                         |
| pickle_pure_python   | 324 us                                                 | 301 us: 1.07x faster                                           |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                          |
| pickle               | 11.6 us                                                | 11.1 us: 1.05x faster                                          |
| unpickle_pure_python | 230 us                                                 | 220 us: 1.05x faster                                           |
| xml_etree_process    | 61.7 ms                                                | 59.0 ms: 1.05x faster                                          |
| unpickle_list        | 5.29 us                                                | 5.07 us: 1.04x faster                                          |
| xml_etree_generate   | 89.2 ms                                                | 85.9 ms: 1.04x faster                                          |
| pickle_dict          | 35.5 us                                                | 34.3 us: 1.04x faster                                          |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                          |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                           |
| pickle_list          | 5.08 us                                                | 5.05 us: 1.01x faster                                          |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                          |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                   |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.08x slower                                          |
| python_startup_no_site | 6.94 ms                                                | 8.99 ms: 1.30x slower                                          |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.4 ms: 1.04x faster                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-linux-x86_64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 118 us: 1.34x faster                                           |
| comprehensions             | 21.8 us                                                | 16.3 us: 1.33x faster                                          |
| logging_format             | 7.23 us                                                | 6.24 us: 1.16x faster                                          |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                           |
| logging_simple             | 6.46 us                                                | 5.68 us: 1.14x faster                                          |
| raytrace                   | 312 ms                                                 | 275 ms: 1.14x faster                                           |
| deltablue                  | 3.72 ms                                                | 3.32 ms: 1.12x faster                                          |
| sympy_str                  | 300 ms                                                 | 269 ms: 1.11x faster                                           |
| regex_compile              | 148 ms                                                 | 134 ms: 1.10x faster                                           |
| chaos                      | 67.0 ms                                                | 60.9 ms: 1.10x faster                                          |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                          |
| scimark_monte_carlo        | 75.1 ms                                                | 68.5 ms: 1.10x faster                                          |
| crypto_pyaes               | 81.9 ms                                                | 75.0 ms: 1.09x faster                                          |
| deepcopy_reduce            | 3.35 us                                                | 3.07 us: 1.09x faster                                          |
| tornado_http               | 103 ms                                                 | 95.0 ms: 1.08x faster                                          |
| async_tree_none            | 472 ms                                                 | 438 ms: 1.08x faster                                           |
| tomli_loads                | 2.33 sec                                               | 2.17 sec: 1.07x faster                                         |
| pickle_pure_python         | 324 us                                                 | 301 us: 1.07x faster                                           |
| generators                 | 31.2 ms                                                | 29.1 ms: 1.07x faster                                          |
| sqlglot_parse              | 1.36 ms                                                | 1.27 ms: 1.07x faster                                          |
| docutils                   | 2.77 sec                                               | 2.59 sec: 1.07x faster                                         |
| nbody                      | 97.0 ms                                                | 91.2 ms: 1.06x faster                                          |
| sqlglot_transpile          | 1.68 ms                                                | 1.59 ms: 1.06x faster                                          |
| unpickle                   | 15.9 us                                                | 15.0 us: 1.06x faster                                          |
| deepcopy                   | 371 us                                                 | 351 us: 1.06x faster                                           |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                          |
| fannkuch                   | 417 ms                                                 | 397 ms: 1.05x faster                                           |
| chameleon                  | 7.41 ms                                                | 7.06 ms: 1.05x faster                                          |
| async_generators           | 463 ms                                                 | 442 ms: 1.05x faster                                           |
| pickle                     | 11.6 us                                                | 11.1 us: 1.05x faster                                          |
| unpickle_pure_python       | 230 us                                                 | 220 us: 1.05x faster                                           |
| xml_etree_process          | 61.7 ms                                                | 59.0 ms: 1.05x faster                                          |
| sympy_expand               | 478 ms                                                 | 457 ms: 1.05x faster                                           |
| scimark_sor                | 129 ms                                                 | 124 ms: 1.04x faster                                           |
| unpickle_list              | 5.29 us                                                | 5.07 us: 1.04x faster                                          |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.85 ms: 1.04x faster                                          |
| nqueens                    | 83.3 ms                                                | 79.9 ms: 1.04x faster                                          |
| hexiom                     | 6.41 ms                                                | 6.15 ms: 1.04x faster                                          |
| pprint_safe_repr           | 776 ms                                                 | 745 ms: 1.04x faster                                           |
| mako                       | 11.9 ms                                                | 11.4 ms: 1.04x faster                                          |
| dulwich_log                | 68.5 ms                                                | 65.8 ms: 1.04x faster                                          |
| deepcopy_memo              | 40.7 us                                                | 39.2 us: 1.04x faster                                          |
| spectral_norm              | 115 ms                                                 | 111 ms: 1.04x faster                                           |
| 2to3                       | 274 ms                                                 | 264 ms: 1.04x faster                                           |
| sqlglot_normalize          | 110 ms                                                 | 106 ms: 1.04x faster                                           |
| xml_etree_generate         | 89.2 ms                                                | 85.9 ms: 1.04x faster                                          |
| pprint_pformat             | 1.57 sec                                               | 1.51 sec: 1.04x faster                                         |
| pickle_dict                | 35.5 us                                                | 34.3 us: 1.04x faster                                          |
| float                      | 84.7 ms                                                | 81.9 ms: 1.03x faster                                          |
| scimark_fft                | 382 ms                                                 | 369 ms: 1.03x faster                                           |
| coroutines                 | 23.2 ms                                                | 22.5 ms: 1.03x faster                                          |
| regex_effbot               | 3.61 ms                                                | 3.50 ms: 1.03x faster                                          |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                           |
| pycparser                  | 1.18 sec                                               | 1.15 sec: 1.03x faster                                         |
| async_tree_memoization     | 578 ms                                                 | 565 ms: 1.02x faster                                           |
| pyflate                    | 482 ms                                                 | 472 ms: 1.02x faster                                           |
| sqlglot_optimize           | 54.8 ms                                                | 53.8 ms: 1.02x faster                                          |
| json                       | 5.26 ms                                                | 5.16 ms: 1.02x faster                                          |
| bench_thread_pool          | 842 us                                                 | 827 us: 1.02x faster                                           |
| mdp                        | 2.63 sec                                               | 2.59 sec: 1.01x faster                                         |
| asyncio_tcp                | 491 ms                                                 | 485 ms: 1.01x faster                                           |
| scimark_lu                 | 118 ms                                                 | 117 ms: 1.01x faster                                           |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                          |
| logging_silent             | 104 ns                                                 | 103 ns: 1.01x faster                                           |
| xml_etree_iterparse        | 107 ms                                                 | 106 ms: 1.01x faster                                           |
| go                         | 139 ms                                                 | 139 ms: 1.01x faster                                           |
| pickle_list                | 5.08 us                                                | 5.05 us: 1.01x faster                                          |
| json_dumps                 | 10.4 ms                                                | 10.4 ms: 1.00x slower                                          |
| async_tree_none_tg         | 450 ms                                                 | 455 ms: 1.01x slower                                           |
| unpack_sequence            | 54.0 ns                                                | 54.7 ns: 1.01x slower                                          |
| regex_dna                  | 212 ms                                                 | 217 ms: 1.02x slower                                           |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                         |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.04x slower                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 597 ms: 1.04x slower                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 755 ms: 1.04x slower                                           |
| richards                   | 45.8 ms                                                | 47.7 ms: 1.04x slower                                          |
| richards_super             | 51.5 ms                                                | 53.7 ms: 1.04x slower                                          |
| regex_v8                   | 23.1 ms                                                | 24.4 ms: 1.05x slower                                          |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.08x slower                                          |
| gc_traversal               | 3.79 ms                                                | 4.30 ms: 1.13x slower                                          |
| pidigits                   | 187 ms                                                 | 222 ms: 1.19x slower                                           |
| telco                      | 7.10 ms                                                | 8.55 ms: 1.20x slower                                          |
| coverage                   | 72.7 ms                                                | 93.0 ms: 1.28x slower                                          |
| python_startup_no_site     | 6.94 ms                                                | 8.99 ms: 1.30x slower                                          |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                   |

Benchmark hidden because not significant (8): xml_etree_parse, sqlite_synth, create_gc_cycles, bench_mp_pool, asyncio_tcp_ssl, async_tree_cpu_io_mixed, asyncio_websockets, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.91x