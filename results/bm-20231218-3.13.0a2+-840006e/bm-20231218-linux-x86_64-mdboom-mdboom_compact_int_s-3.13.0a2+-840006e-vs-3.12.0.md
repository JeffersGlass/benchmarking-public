
# Results vs. 3.12.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 840006e
- commit date: 2023-12-18
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 266 ms: 1.03x faster                                                   |
| chameleon      | 7.41 ms                                                | 7.08 ms: 1.05x faster                                                  |
| docutils       | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                 |
| tornado_http   | 103 ms                                                 | 95.2 ms: 1.08x faster                                                  |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 438 ms: 1.08x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 561 ms: 1.03x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 453 ms: 1.01x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 595 ms: 1.04x slower                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 831 ms: 1.15x slower                                                   |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 861 ms: 1.19x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 89.2 ms: 1.09x faster                                                  |
| float          | 84.7 ms                                                | 81.9 ms: 1.03x faster                                                  |
| pidigits       | 187 ms                                                 | 288 ms: 1.54x slower                                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 135 ms: 1.10x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.52 ms: 1.02x faster                                                  |
| regex_dna      | 212 ms                                                 | 220 ms: 1.04x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.13 sec: 1.09x faster                                                 |
| unpickle_list        | 5.29 us                                                | 4.87 us: 1.09x faster                                                  |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 59.1 ms: 1.04x faster                                                  |
| pickle               | 11.6 us                                                | 11.2 us: 1.04x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 222 us: 1.04x faster                                                   |
| xml_etree_generate   | 89.2 ms                                                | 86.5 ms: 1.03x faster                                                  |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                  |
| pickle_dict          | 35.5 us                                                | 35.3 us: 1.01x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_dumps           | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                  |
| pickle_list          | 5.08 us                                                | 5.33 us: 1.05x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.08x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.99 ms: 1.30x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.4 ms: 1.05x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 116 us: 1.37x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.4 us: 1.33x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 43.3 ns: 1.25x faster                                                  |
| logging_format             | 7.23 us                                                | 6.28 us: 1.15x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| crypto_pyaes               | 81.9 ms                                                | 72.7 ms: 1.13x faster                                                  |
| logging_simple             | 6.46 us                                                | 5.76 us: 1.12x faster                                                  |
| raytrace                   | 312 ms                                                 | 279 ms: 1.12x faster                                                   |
| deltablue                  | 3.72 ms                                                | 3.34 ms: 1.11x faster                                                  |
| chaos                      | 67.0 ms                                                | 60.3 ms: 1.11x faster                                                  |
| scimark_monte_carlo        | 75.1 ms                                                | 68.1 ms: 1.10x faster                                                  |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| regex_compile              | 148 ms                                                 | 135 ms: 1.10x faster                                                   |
| sympy_str                  | 300 ms                                                 | 273 ms: 1.10x faster                                                   |
| tomli_loads                | 2.33 sec                                               | 2.13 sec: 1.09x faster                                                 |
| coroutines                 | 23.2 ms                                                | 21.3 ms: 1.09x faster                                                  |
| nbody                      | 97.0 ms                                                | 89.2 ms: 1.09x faster                                                  |
| unpickle_list              | 5.29 us                                                | 4.87 us: 1.09x faster                                                  |
| tornado_http               | 103 ms                                                 | 95.2 ms: 1.08x faster                                                  |
| async_tree_none            | 472 ms                                                 | 438 ms: 1.08x faster                                                   |
| pathlib                    | 19.3 ms                                                | 18.0 ms: 1.08x faster                                                  |
| pyflate                    | 482 ms                                                 | 448 ms: 1.08x faster                                                   |
| generators                 | 31.2 ms                                                | 29.0 ms: 1.08x faster                                                  |
| scimark_fft                | 382 ms                                                 | 357 ms: 1.07x faster                                                   |
| unpickle                   | 15.9 us                                                | 14.9 us: 1.07x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.14 us: 1.07x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                 |
| sqlglot_parse              | 1.36 ms                                                | 1.28 ms: 1.06x faster                                                  |
| pickle_pure_python         | 324 us                                                 | 305 us: 1.06x faster                                                   |
| spectral_norm              | 115 ms                                                 | 108 ms: 1.06x faster                                                   |
| fannkuch                   | 417 ms                                                 | 394 ms: 1.06x faster                                                   |
| gc_traversal               | 3.79 ms                                                | 3.59 ms: 1.06x faster                                                  |
| nqueens                    | 83.3 ms                                                | 79.1 ms: 1.05x faster                                                  |
| sqlglot_transpile          | 1.68 ms                                                | 1.60 ms: 1.05x faster                                                  |
| sympy_expand               | 478 ms                                                 | 456 ms: 1.05x faster                                                   |
| mdp                        | 2.63 sec                                               | 2.51 sec: 1.05x faster                                                 |
| deepcopy                   | 371 us                                                 | 355 us: 1.05x faster                                                   |
| chameleon                  | 7.41 ms                                                | 7.08 ms: 1.05x faster                                                  |
| dulwich_log                | 68.5 ms                                                | 65.5 ms: 1.05x faster                                                  |
| mako                       | 11.9 ms                                                | 11.4 ms: 1.05x faster                                                  |
| xml_etree_process          | 61.7 ms                                                | 59.1 ms: 1.04x faster                                                  |
| pickle                     | 11.6 us                                                | 11.2 us: 1.04x faster                                                  |
| unpickle_pure_python       | 230 us                                                 | 222 us: 1.04x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 39.3 us: 1.04x faster                                                  |
| pprint_safe_repr           | 776 ms                                                 | 749 ms: 1.03x faster                                                   |
| float                      | 84.7 ms                                                | 81.9 ms: 1.03x faster                                                  |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                                   |
| sqlglot_normalize          | 110 ms                                                 | 107 ms: 1.03x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 86.5 ms: 1.03x faster                                                  |
| async_tree_memoization     | 578 ms                                                 | 561 ms: 1.03x faster                                                   |
| 2to3                       | 274 ms                                                 | 266 ms: 1.03x faster                                                   |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.91 ms: 1.03x faster                                                  |
| pprint_pformat             | 1.57 sec                                               | 1.53 sec: 1.03x faster                                                 |
| hexiom                     | 6.41 ms                                                | 6.25 ms: 1.03x faster                                                  |
| regex_effbot               | 3.61 ms                                                | 3.52 ms: 1.02x faster                                                  |
| sqlite_synth               | 2.83 us                                                | 2.77 us: 1.02x faster                                                  |
| async_generators           | 463 ms                                                 | 453 ms: 1.02x faster                                                   |
| json                       | 5.26 ms                                                | 5.15 ms: 1.02x faster                                                  |
| sqlglot_optimize           | 54.8 ms                                                | 54.1 ms: 1.01x faster                                                  |
| scimark_lu                 | 118 ms                                                 | 117 ms: 1.01x faster                                                   |
| bench_thread_pool          | 842 us                                                 | 832 us: 1.01x faster                                                   |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                                  |
| scimark_sor                | 129 ms                                                 | 128 ms: 1.01x faster                                                   |
| asyncio_tcp                | 491 ms                                                 | 486 ms: 1.01x faster                                                   |
| pycparser                  | 1.18 sec                                               | 1.17 sec: 1.01x faster                                                 |
| pickle_dict                | 35.5 us                                                | 35.3 us: 1.01x faster                                                  |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.79 sec: 1.00x slower                                                 |
| json_dumps                 | 10.4 ms                                                | 10.4 ms: 1.00x slower                                                  |
| async_tree_none_tg         | 450 ms                                                 | 453 ms: 1.01x slower                                                   |
| go                         | 139 ms                                                 | 141 ms: 1.01x slower                                                   |
| logging_silent             | 104 ns                                                 | 107 ns: 1.02x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 595 ms: 1.04x slower                                                   |
| regex_dna                  | 212 ms                                                 | 220 ms: 1.04x slower                                                   |
| pickle_list                | 5.08 us                                                | 5.33 us: 1.05x slower                                                  |
| richards                   | 45.8 ms                                                | 48.3 ms: 1.05x slower                                                  |
| richards_super             | 51.5 ms                                                | 54.7 ms: 1.06x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.08x slower                                                  |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 831 ms: 1.15x slower                                                   |
| telco                      | 7.10 ms                                                | 8.30 ms: 1.17x slower                                                  |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 861 ms: 1.19x slower                                                   |
| coverage                   | 72.7 ms                                                | 93.7 ms: 1.29x slower                                                  |
| python_startup_no_site     | 6.94 ms                                                | 8.99 ms: 1.30x slower                                                  |
| pidigits                   | 187 ms                                                 | 288 ms: 1.54x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (5): xml_etree_iterparse, create_gc_cycles, bench_mp_pool, asyncio_websockets, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.91x