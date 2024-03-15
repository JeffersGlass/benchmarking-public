
# Results vs. 3.12.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 522c622
- commit date: 2023-12-20
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.96 ms: 1.07x faster                                                  |
| docutils       | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                 |
| tornado_http   | 103 ms                                                 | 95.1 ms: 1.08x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 436 ms: 1.08x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 562 ms: 1.03x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 454 ms: 1.01x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 598 ms: 1.04x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 758 ms: 1.04x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 89.7 ms: 1.08x faster                                                  |
| float          | 84.7 ms                                                | 82.4 ms: 1.03x faster                                                  |
| pidigits       | 187 ms                                                 | 223 ms: 1.19x slower                                                   |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 134 ms: 1.11x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                  |
| regex_dna      | 212 ms                                                 | 221 ms: 1.04x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle             | 15.9 us                                                | 14.3 us: 1.11x faster                                                  |
| unpickle_list        | 5.29 us                                                | 4.88 us: 1.08x faster                                                  |
| tomli_loads          | 2.33 sec                                               | 2.17 sec: 1.07x faster                                                 |
| pickle_pure_python   | 324 us                                                 | 308 us: 1.05x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 59.2 ms: 1.04x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 85.8 ms: 1.04x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.4 us: 1.03x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 223 us: 1.03x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.00 us: 1.02x faster                                                  |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                                  |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (3): xml_etree_iterparse, json_dumps, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 9.04 ms: 1.30x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 118 us: 1.34x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.4 us: 1.33x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| raytrace                   | 312 ms                                                 | 272 ms: 1.15x faster                                                   |
| unpack_sequence            | 54.0 ns                                                | 47.2 ns: 1.14x faster                                                  |
| logging_format             | 7.23 us                                                | 6.36 us: 1.14x faster                                                  |
| deltablue                  | 3.72 ms                                                | 3.31 ms: 1.12x faster                                                  |
| logging_simple             | 6.46 us                                                | 5.77 us: 1.12x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 73.3 ms: 1.12x faster                                                  |
| regex_compile              | 148 ms                                                 | 134 ms: 1.11x faster                                                   |
| sympy_str                  | 300 ms                                                 | 271 ms: 1.11x faster                                                   |
| unpickle                   | 15.9 us                                                | 14.3 us: 1.11x faster                                                  |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| chaos                      | 67.0 ms                                                | 60.8 ms: 1.10x faster                                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 68.8 ms: 1.09x faster                                                  |
| generators                 | 31.2 ms                                                | 28.7 ms: 1.09x faster                                                  |
| unpickle_list              | 5.29 us                                                | 4.88 us: 1.08x faster                                                  |
| async_tree_none            | 472 ms                                                 | 436 ms: 1.08x faster                                                   |
| nbody                      | 97.0 ms                                                | 89.7 ms: 1.08x faster                                                  |
| tornado_http               | 103 ms                                                 | 95.1 ms: 1.08x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.17 sec: 1.07x faster                                                 |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                 |
| chameleon                  | 7.41 ms                                                | 6.96 ms: 1.07x faster                                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.28 ms: 1.07x faster                                                  |
| pathlib                    | 19.3 ms                                                | 18.2 ms: 1.06x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.15 us: 1.06x faster                                                  |
| pyflate                    | 482 ms                                                 | 455 ms: 1.06x faster                                                   |
| deepcopy                   | 371 us                                                 | 351 us: 1.06x faster                                                   |
| pprint_safe_repr           | 776 ms                                                 | 735 ms: 1.06x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 38.7 us: 1.05x faster                                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.60 ms: 1.05x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 308 us: 1.05x faster                                                   |
| dulwich_log                | 68.5 ms                                                | 65.3 ms: 1.05x faster                                                  |
| coroutines                 | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                  |
| sympy_expand               | 478 ms                                                 | 456 ms: 1.05x faster                                                   |
| pprint_pformat             | 1.57 sec                                               | 1.50 sec: 1.05x faster                                                 |
| meteor_contest             | 112 ms                                                 | 108 ms: 1.04x faster                                                   |
| xml_etree_process          | 61.7 ms                                                | 59.2 ms: 1.04x faster                                                  |
| 2to3                       | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 85.8 ms: 1.04x faster                                                  |
| scimark_sor                | 129 ms                                                 | 124 ms: 1.04x faster                                                   |
| fannkuch                   | 417 ms                                                 | 402 ms: 1.04x faster                                                   |
| sqlglot_normalize          | 110 ms                                                 | 107 ms: 1.03x faster                                                   |
| pickle_dict                | 35.5 us                                                | 34.4 us: 1.03x faster                                                  |
| unpickle_pure_python       | 230 us                                                 | 223 us: 1.03x faster                                                   |
| spectral_norm              | 115 ms                                                 | 111 ms: 1.03x faster                                                   |
| hexiom                     | 6.41 ms                                                | 6.23 ms: 1.03x faster                                                  |
| async_generators           | 463 ms                                                 | 450 ms: 1.03x faster                                                   |
| nqueens                    | 83.3 ms                                                | 81.0 ms: 1.03x faster                                                  |
| async_tree_memoization     | 578 ms                                                 | 562 ms: 1.03x faster                                                   |
| float                      | 84.7 ms                                                | 82.4 ms: 1.03x faster                                                  |
| scimark_fft                | 382 ms                                                 | 372 ms: 1.03x faster                                                   |
| json                       | 5.26 ms                                                | 5.13 ms: 1.02x faster                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 53.8 ms: 1.02x faster                                                  |
| asyncio_tcp                | 491 ms                                                 | 483 ms: 1.02x faster                                                   |
| pickle_list                | 5.08 us                                                | 5.00 us: 1.02x faster                                                  |
| bench_thread_pool          | 842 us                                                 | 830 us: 1.01x faster                                                   |
| pycparser                  | 1.18 sec                                               | 1.16 sec: 1.01x faster                                                 |
| json_loads                 | 28.5 us                                                | 28.1 us: 1.01x faster                                                  |
| sqlite_synth               | 2.83 us                                                | 2.80 us: 1.01x faster                                                  |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.01 ms: 1.01x faster                                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                 |
| logging_silent             | 104 ns                                                 | 104 ns: 1.00x faster                                                   |
| go                         | 139 ms                                                 | 140 ms: 1.01x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 454 ms: 1.01x slower                                                   |
| create_gc_cycles           | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                  |
| regex_effbot               | 3.61 ms                                                | 3.68 ms: 1.02x slower                                                  |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 598 ms: 1.04x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 758 ms: 1.04x slower                                                   |
| regex_dna                  | 212 ms                                                 | 221 ms: 1.04x slower                                                   |
| richards_super             | 51.5 ms                                                | 54.0 ms: 1.05x slower                                                  |
| richards                   | 45.8 ms                                                | 48.2 ms: 1.05x slower                                                  |
| mdp                        | 2.63 sec                                               | 2.77 sec: 1.05x slower                                                 |
| regex_v8                   | 23.1 ms                                                | 24.6 ms: 1.06x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                  |
| gc_traversal               | 3.79 ms                                                | 4.31 ms: 1.14x slower                                                  |
| telco                      | 7.10 ms                                                | 8.36 ms: 1.18x slower                                                  |
| pidigits                   | 187 ms                                                 | 223 ms: 1.19x slower                                                   |
| coverage                   | 72.7 ms                                                | 94.0 ms: 1.29x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 9.04 ms: 1.30x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (8): xml_etree_iterparse, scimark_lu, json_dumps, xml_etree_parse, bench_mp_pool, asyncio_websockets, async_tree_cpu_io_mixed, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.91x