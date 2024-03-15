
# Results vs. 3.12.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 01a12af
- commit date: 2023-12-19
- overall geometric mean: 1.03x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 7.01 ms: 1.06x faster                                                  |
| docutils       | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.9 ms: 1.08x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 436 ms: 1.08x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 561 ms: 1.03x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 454 ms: 1.01x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.04x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 596 ms: 1.04x slower                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 834 ms: 1.15x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 866 ms: 1.19x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 89.2 ms: 1.09x faster                                                  |
| float          | 84.7 ms                                                | 81.5 ms: 1.04x faster                                                  |
| pidigits       | 187 ms                                                 | 289 ms: 1.54x slower                                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 136 ms: 1.09x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.69 ms: 1.02x slower                                                  |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.5 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 32.8 us: 1.08x faster                                                  |
| tomli_loads          | 2.33 sec                                               | 2.17 sec: 1.07x faster                                                 |
| unpickle             | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 306 us: 1.06x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 222 us: 1.04x faster                                                   |
| xml_etree_generate   | 89.2 ms                                                | 86.2 ms: 1.03x faster                                                  |
| pickle               | 11.6 us                                                | 11.3 us: 1.03x faster                                                  |
| unpickle_list        | 5.29 us                                                | 5.16 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.15 us: 1.01x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.08x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 9.00 ms: 1.30x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.35x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.5 us: 1.32x faster                                                  |
| logging_format             | 7.23 us                                                | 6.25 us: 1.16x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 46.7 ns: 1.16x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| raytrace                   | 312 ms                                                 | 272 ms: 1.15x faster                                                   |
| logging_simple             | 6.46 us                                                | 5.69 us: 1.14x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 72.3 ms: 1.13x faster                                                  |
| deltablue                  | 3.72 ms                                                | 3.30 ms: 1.13x faster                                                  |
| sympy_str                  | 300 ms                                                 | 269 ms: 1.11x faster                                                   |
| chaos                      | 67.0 ms                                                | 60.6 ms: 1.10x faster                                                  |
| sympy_integrate            | 21.4 ms                                                | 19.6 ms: 1.10x faster                                                  |
| regex_compile              | 148 ms                                                 | 136 ms: 1.09x faster                                                   |
| scimark_monte_carlo        | 75.1 ms                                                | 68.8 ms: 1.09x faster                                                  |
| nbody                      | 97.0 ms                                                | 89.2 ms: 1.09x faster                                                  |
| pickle_dict                | 35.5 us                                                | 32.8 us: 1.08x faster                                                  |
| async_tree_none            | 472 ms                                                 | 436 ms: 1.08x faster                                                   |
| tornado_http               | 103 ms                                                 | 94.9 ms: 1.08x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.17 sec: 1.07x faster                                                 |
| unpickle                   | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.12 us: 1.07x faster                                                  |
| pyflate                    | 482 ms                                                 | 452 ms: 1.07x faster                                                   |
| sqlglot_parse              | 1.36 ms                                                | 1.28 ms: 1.07x faster                                                  |
| generators                 | 31.2 ms                                                | 29.3 ms: 1.06x faster                                                  |
| mako                       | 11.9 ms                                                | 11.2 ms: 1.06x faster                                                  |
| pathlib                    | 19.3 ms                                                | 18.2 ms: 1.06x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| coroutines                 | 23.2 ms                                                | 21.9 ms: 1.06x faster                                                  |
| hexiom                     | 6.41 ms                                                | 6.06 ms: 1.06x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 306 us: 1.06x faster                                                   |
| chameleon                  | 7.41 ms                                                | 7.01 ms: 1.06x faster                                                  |
| scimark_fft                | 382 ms                                                 | 362 ms: 1.06x faster                                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.60 ms: 1.05x faster                                                  |
| sympy_expand               | 478 ms                                                 | 455 ms: 1.05x faster                                                   |
| fannkuch                   | 417 ms                                                 | 397 ms: 1.05x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 38.8 us: 1.05x faster                                                  |
| scimark_sor                | 129 ms                                                 | 123 ms: 1.05x faster                                                   |
| dulwich_log                | 68.5 ms                                                | 65.4 ms: 1.05x faster                                                  |
| pprint_safe_repr           | 776 ms                                                 | 741 ms: 1.05x faster                                                   |
| spectral_norm              | 115 ms                                                 | 110 ms: 1.04x faster                                                   |
| deepcopy                   | 371 us                                                 | 356 us: 1.04x faster                                                   |
| nqueens                    | 83.3 ms                                                | 80.0 ms: 1.04x faster                                                  |
| async_generators           | 463 ms                                                 | 445 ms: 1.04x faster                                                   |
| pprint_pformat             | 1.57 sec                                               | 1.51 sec: 1.04x faster                                                 |
| xml_etree_process          | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                  |
| float                      | 84.7 ms                                                | 81.5 ms: 1.04x faster                                                  |
| 2to3                       | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| unpickle_pure_python       | 230 us                                                 | 222 us: 1.04x faster                                                   |
| sqlglot_normalize          | 110 ms                                                 | 106 ms: 1.04x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 86.2 ms: 1.03x faster                                                  |
| scimark_lu                 | 118 ms                                                 | 114 ms: 1.03x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 561 ms: 1.03x faster                                                   |
| pickle                     | 11.6 us                                                | 11.3 us: 1.03x faster                                                  |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                                   |
| json                       | 5.26 ms                                                | 5.13 ms: 1.03x faster                                                  |
| unpickle_list              | 5.29 us                                                | 5.16 us: 1.02x faster                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 53.8 ms: 1.02x faster                                                  |
| pycparser                  | 1.18 sec                                               | 1.16 sec: 1.02x faster                                                 |
| bench_thread_pool          | 842 us                                                 | 830 us: 1.01x faster                                                   |
| asyncio_tcp                | 491 ms                                                 | 485 ms: 1.01x faster                                                   |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.01 ms: 1.01x faster                                                  |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                                  |
| xml_etree_iterparse        | 107 ms                                                 | 106 ms: 1.01x faster                                                   |
| mdp                        | 2.63 sec                                               | 2.61 sec: 1.01x faster                                                 |
| sqlite_synth               | 2.83 us                                                | 2.81 us: 1.01x faster                                                  |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.79 sec: 1.00x slower                                                 |
| go                         | 139 ms                                                 | 140 ms: 1.01x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 454 ms: 1.01x slower                                                   |
| create_gc_cycles           | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                  |
| pickle_list                | 5.08 us                                                | 5.15 us: 1.01x slower                                                  |
| regex_effbot               | 3.61 ms                                                | 3.69 ms: 1.02x slower                                                  |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| richards                   | 45.8 ms                                                | 47.4 ms: 1.03x slower                                                  |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.04x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 596 ms: 1.04x slower                                                   |
| richards_super             | 51.5 ms                                                | 53.5 ms: 1.04x slower                                                  |
| gc_traversal               | 3.79 ms                                                | 3.96 ms: 1.04x slower                                                  |
| regex_dna                  | 212 ms                                                 | 222 ms: 1.05x slower                                                   |
| regex_v8                   | 23.1 ms                                                | 24.5 ms: 1.06x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.08x slower                                                  |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 834 ms: 1.15x slower                                                   |
| telco                      | 7.10 ms                                                | 8.30 ms: 1.17x slower                                                  |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 866 ms: 1.19x slower                                                   |
| coverage                   | 72.7 ms                                                | 94.2 ms: 1.30x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 9.00 ms: 1.30x slower                                                  |
| pidigits                   | 187 ms                                                 | 289 ms: 1.54x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (5): json_dumps, asyncio_websockets, bench_mp_pool, logging_silent, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.91x