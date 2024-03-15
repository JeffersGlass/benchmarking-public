
# Results vs. 3.12.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 2f0a32b
- commit date: 2023-12-19
- overall geometric mean: 1.02x faster
- HPT reliability: 99.93%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 266 ms: 1.03x faster                                                   |
| chameleon      | 7.41 ms                                                | 7.07 ms: 1.05x faster                                                  |
| docutils       | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| tornado_http   | 103 ms                                                 | 95.2 ms: 1.08x faster                                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 439 ms: 1.08x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 566 ms: 1.02x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 758 ms: 1.04x slower                                                   |
| async_tree_memoization_tg  | 575 ms                                                 | 607 ms: 1.06x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 90.5 ms: 1.07x faster                                                  |
| float          | 84.7 ms                                                | 82.4 ms: 1.03x faster                                                  |
| pidigits       | 187 ms                                                 | 228 ms: 1.21x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 135 ms: 1.10x faster                                                   |
| regex_dna      | 212 ms                                                 | 216 ms: 1.02x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 4.93 us: 1.07x faster                                                  |
| tomli_loads          | 2.33 sec                                               | 2.18 sec: 1.07x faster                                                 |
| unpickle             | 15.9 us                                                | 15.0 us: 1.05x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 307 us: 1.05x faster                                                   |
| pickle_dict          | 35.5 us                                                | 34.1 us: 1.04x faster                                                  |
| xml_etree_process    | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 86.6 ms: 1.03x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 224 us: 1.03x faster                                                   |
| pickle_list          | 5.08 us                                                | 4.98 us: 1.02x faster                                                  |
| pickle               | 11.6 us                                                | 11.4 us: 1.02x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_loads           | 28.5 us                                                | 28.4 us: 1.00x faster                                                  |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 9.04 ms: 1.30x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.35x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.6 us: 1.31x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 46.9 ns: 1.15x faster                                                  |
| logging_format             | 7.23 us                                                | 6.31 us: 1.15x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| raytrace                   | 312 ms                                                 | 274 ms: 1.14x faster                                                   |
| logging_simple             | 6.46 us                                                | 5.79 us: 1.12x faster                                                  |
| regex_compile              | 148 ms                                                 | 135 ms: 1.10x faster                                                   |
| crypto_pyaes               | 81.9 ms                                                | 74.4 ms: 1.10x faster                                                  |
| sympy_str                  | 300 ms                                                 | 273 ms: 1.10x faster                                                   |
| scimark_monte_carlo        | 75.1 ms                                                | 68.5 ms: 1.10x faster                                                  |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| deltablue                  | 3.72 ms                                                | 3.43 ms: 1.08x faster                                                  |
| tornado_http               | 103 ms                                                 | 95.2 ms: 1.08x faster                                                  |
| chaos                      | 67.0 ms                                                | 62.2 ms: 1.08x faster                                                  |
| async_tree_none            | 472 ms                                                 | 439 ms: 1.08x faster                                                   |
| unpickle_list              | 5.29 us                                                | 4.93 us: 1.07x faster                                                  |
| nbody                      | 97.0 ms                                                | 90.5 ms: 1.07x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.18 sec: 1.07x faster                                                 |
| deepcopy_reduce            | 3.35 us                                                | 3.14 us: 1.06x faster                                                  |
| pathlib                    | 19.3 ms                                                | 18.2 ms: 1.06x faster                                                  |
| coroutines                 | 23.2 ms                                                | 21.8 ms: 1.06x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| mako                       | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.29 ms: 1.06x faster                                                  |
| unpickle                   | 15.9 us                                                | 15.0 us: 1.05x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 307 us: 1.05x faster                                                   |
| chameleon                  | 7.41 ms                                                | 7.07 ms: 1.05x faster                                                  |
| pprint_safe_repr           | 776 ms                                                 | 741 ms: 1.05x faster                                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.61 ms: 1.05x faster                                                  |
| generators                 | 31.2 ms                                                | 30.0 ms: 1.04x faster                                                  |
| deepcopy                   | 371 us                                                 | 356 us: 1.04x faster                                                   |
| pickle_dict                | 35.5 us                                                | 34.1 us: 1.04x faster                                                  |
| sympy_expand               | 478 ms                                                 | 460 ms: 1.04x faster                                                   |
| fannkuch                   | 417 ms                                                 | 401 ms: 1.04x faster                                                   |
| pprint_pformat             | 1.57 sec                                               | 1.51 sec: 1.04x faster                                                 |
| xml_etree_process          | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                  |
| async_generators           | 463 ms                                                 | 446 ms: 1.04x faster                                                   |
| dulwich_log                | 68.5 ms                                                | 66.0 ms: 1.04x faster                                                  |
| sqlglot_normalize          | 110 ms                                                 | 107 ms: 1.03x faster                                                   |
| 2to3                       | 274 ms                                                 | 266 ms: 1.03x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 86.6 ms: 1.03x faster                                                  |
| scimark_fft                | 382 ms                                                 | 371 ms: 1.03x faster                                                   |
| scimark_sor                | 129 ms                                                 | 126 ms: 1.03x faster                                                   |
| unpickle_pure_python       | 230 us                                                 | 224 us: 1.03x faster                                                   |
| pyflate                    | 482 ms                                                 | 469 ms: 1.03x faster                                                   |
| float                      | 84.7 ms                                                | 82.4 ms: 1.03x faster                                                  |
| asyncio_tcp                | 491 ms                                                 | 479 ms: 1.02x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 39.9 us: 1.02x faster                                                  |
| async_tree_memoization     | 578 ms                                                 | 566 ms: 1.02x faster                                                   |
| pickle_list                | 5.08 us                                                | 4.98 us: 1.02x faster                                                  |
| nqueens                    | 83.3 ms                                                | 81.7 ms: 1.02x faster                                                  |
| scimark_lu                 | 118 ms                                                 | 116 ms: 1.02x faster                                                   |
| pickle                     | 11.6 us                                                | 11.4 us: 1.02x faster                                                  |
| sqlite_synth               | 2.83 us                                                | 2.80 us: 1.01x faster                                                  |
| meteor_contest             | 112 ms                                                 | 111 ms: 1.01x faster                                                   |
| json                       | 5.26 ms                                                | 5.20 ms: 1.01x faster                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 54.3 ms: 1.01x faster                                                  |
| bench_thread_pool          | 842 us                                                 | 834 us: 1.01x faster                                                   |
| hexiom                     | 6.41 ms                                                | 6.36 ms: 1.01x faster                                                  |
| xml_etree_iterparse        | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_loads                 | 28.5 us                                                | 28.4 us: 1.00x faster                                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                 |
| mdp                        | 2.63 sec                                               | 2.64 sec: 1.00x slower                                                 |
| create_gc_cycles           | 1.48 ms                                                | 1.48 ms: 1.00x slower                                                  |
| json_dumps                 | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                  |
| gc_traversal               | 3.79 ms                                                | 3.82 ms: 1.01x slower                                                  |
| logging_silent             | 104 ns                                                 | 106 ns: 1.02x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 458 ms: 1.02x slower                                                   |
| regex_dna                  | 212 ms                                                 | 216 ms: 1.02x slower                                                   |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.17 ms: 1.02x slower                                                  |
| go                         | 139 ms                                                 | 143 ms: 1.03x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| pycparser                  | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 758 ms: 1.04x slower                                                   |
| richards                   | 45.8 ms                                                | 47.9 ms: 1.05x slower                                                  |
| async_tree_memoization_tg  | 575 ms                                                 | 607 ms: 1.06x slower                                                   |
| richards_super             | 51.5 ms                                                | 54.5 ms: 1.06x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 25.7 ms: 1.11x slower                                                  |
| telco                      | 7.10 ms                                                | 8.39 ms: 1.18x slower                                                  |
| pidigits                   | 187 ms                                                 | 228 ms: 1.21x slower                                                   |
| python_startup_no_site     | 6.94 ms                                                | 9.04 ms: 1.30x slower                                                  |
| coverage                   | 72.7 ms                                                | 95.3 ms: 1.31x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (6): regex_effbot, spectral_norm, bench_mp_pool, asyncio_websockets, async_tree_cpu_io_mixed, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.93% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.91x