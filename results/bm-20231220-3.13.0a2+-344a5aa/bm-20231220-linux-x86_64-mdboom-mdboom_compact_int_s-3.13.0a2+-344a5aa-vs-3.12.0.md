
# Results vs. 3.12.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 344a5aa
- commit date: 2023-12-20
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.94 ms: 1.07x faster                                                  |
| docutils       | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                 |
| tornado_http   | 103 ms                                                 | 94.8 ms: 1.08x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 435 ms: 1.09x faster                                                   |
| async_tree_memoization     | 578 ms                                                 | 559 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 715 ms: 1.01x faster                                                   |
| async_tree_none_tg         | 450 ms                                                 | 453 ms: 1.01x slower                                                   |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 746 ms: 1.03x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.04x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 597 ms: 1.04x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 91.9 ms: 1.05x faster                                                  |
| float          | 84.7 ms                                                | 81.6 ms: 1.04x faster                                                  |
| pidigits       | 187 ms                                                 | 226 ms: 1.20x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 135 ms: 1.10x faster                                                   |
| regex_effbot   | 3.61 ms                                                | 3.66 ms: 1.01x slower                                                  |
| regex_dna      | 212 ms                                                 | 220 ms: 1.04x slower                                                   |
| regex_v8       | 23.1 ms                                                | 24.1 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.16 sec: 1.08x faster                                                 |
| pickle_dict          | 35.5 us                                                | 33.1 us: 1.07x faster                                                  |
| unpickle             | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| pickle_pure_python   | 324 us                                                 | 304 us: 1.07x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 58.8 ms: 1.05x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 219 us: 1.05x faster                                                   |
| unpickle_list        | 5.29 us                                                | 5.05 us: 1.05x faster                                                  |
| pickle               | 11.6 us                                                | 11.1 us: 1.05x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 85.4 ms: 1.04x faster                                                  |
| json_loads           | 28.5 us                                                | 27.8 us: 1.03x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.98 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                   |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                                   |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.3 ms: 1.08x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.95 ms: 1.29x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.18x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.35x faster                                                   |
| comprehensions             | 21.8 us                                                | 16.6 us: 1.31x faster                                                  |
| unpack_sequence            | 54.0 ns                                                | 43.4 ns: 1.24x faster                                                  |
| logging_format             | 7.23 us                                                | 6.20 us: 1.17x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| raytrace                   | 312 ms                                                 | 275 ms: 1.14x faster                                                   |
| logging_simple             | 6.46 us                                                | 5.72 us: 1.13x faster                                                  |
| crypto_pyaes               | 81.9 ms                                                | 72.8 ms: 1.13x faster                                                  |
| chaos                      | 67.0 ms                                                | 60.4 ms: 1.11x faster                                                  |
| deltablue                  | 3.72 ms                                                | 3.37 ms: 1.10x faster                                                  |
| regex_compile              | 148 ms                                                 | 135 ms: 1.10x faster                                                   |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| sympy_str                  | 300 ms                                                 | 273 ms: 1.10x faster                                                   |
| scimark_monte_carlo        | 75.1 ms                                                | 68.5 ms: 1.10x faster                                                  |
| async_tree_none            | 472 ms                                                 | 435 ms: 1.09x faster                                                   |
| tornado_http               | 103 ms                                                 | 94.8 ms: 1.08x faster                                                  |
| tomli_loads                | 2.33 sec                                               | 2.16 sec: 1.08x faster                                                 |
| pickle_dict                | 35.5 us                                                | 33.1 us: 1.07x faster                                                  |
| unpickle                   | 15.9 us                                                | 14.8 us: 1.07x faster                                                  |
| deepcopy_reduce            | 3.35 us                                                | 3.13 us: 1.07x faster                                                  |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                  |
| chameleon                  | 7.41 ms                                                | 6.94 ms: 1.07x faster                                                  |
| sqlglot_parse              | 1.36 ms                                                | 1.28 ms: 1.07x faster                                                  |
| docutils                   | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                 |
| pickle_pure_python         | 324 us                                                 | 304 us: 1.07x faster                                                   |
| pyflate                    | 482 ms                                                 | 453 ms: 1.06x faster                                                   |
| deepcopy                   | 371 us                                                 | 350 us: 1.06x faster                                                   |
| pathlib                    | 19.3 ms                                                | 18.3 ms: 1.06x faster                                                  |
| pprint_safe_repr           | 776 ms                                                 | 734 ms: 1.06x faster                                                   |
| nbody                      | 97.0 ms                                                | 91.9 ms: 1.05x faster                                                  |
| fannkuch                   | 417 ms                                                 | 396 ms: 1.05x faster                                                   |
| sqlglot_transpile          | 1.68 ms                                                | 1.60 ms: 1.05x faster                                                  |
| coroutines                 | 23.2 ms                                                | 22.0 ms: 1.05x faster                                                  |
| generators                 | 31.2 ms                                                | 29.7 ms: 1.05x faster                                                  |
| gc_traversal               | 3.79 ms                                                | 3.61 ms: 1.05x faster                                                  |
| sympy_expand               | 478 ms                                                 | 455 ms: 1.05x faster                                                   |
| deepcopy_memo              | 40.7 us                                                | 38.8 us: 1.05x faster                                                  |
| xml_etree_process          | 61.7 ms                                                | 58.8 ms: 1.05x faster                                                  |
| unpickle_pure_python       | 230 us                                                 | 219 us: 1.05x faster                                                   |
| unpickle_list              | 5.29 us                                                | 5.05 us: 1.05x faster                                                  |
| scimark_sor                | 129 ms                                                 | 123 ms: 1.05x faster                                                   |
| pprint_pformat             | 1.57 sec                                               | 1.50 sec: 1.05x faster                                                 |
| hexiom                     | 6.41 ms                                                | 6.12 ms: 1.05x faster                                                  |
| pickle                     | 11.6 us                                                | 11.1 us: 1.05x faster                                                  |
| spectral_norm              | 115 ms                                                 | 110 ms: 1.04x faster                                                   |
| xml_etree_generate         | 89.2 ms                                                | 85.4 ms: 1.04x faster                                                  |
| dulwich_log                | 68.5 ms                                                | 65.7 ms: 1.04x faster                                                  |
| async_generators           | 463 ms                                                 | 444 ms: 1.04x faster                                                   |
| scimark_fft                | 382 ms                                                 | 367 ms: 1.04x faster                                                   |
| 2to3                       | 274 ms                                                 | 264 ms: 1.04x faster                                                   |
| sqlglot_normalize          | 110 ms                                                 | 106 ms: 1.04x faster                                                   |
| float                      | 84.7 ms                                                | 81.6 ms: 1.04x faster                                                  |
| async_tree_memoization     | 578 ms                                                 | 559 ms: 1.03x faster                                                   |
| json_loads                 | 28.5 us                                                | 27.8 us: 1.03x faster                                                  |
| meteor_contest             | 112 ms                                                 | 110 ms: 1.02x faster                                                   |
| json                       | 5.26 ms                                                | 5.15 ms: 1.02x faster                                                  |
| nqueens                    | 83.3 ms                                                | 81.6 ms: 1.02x faster                                                  |
| pickle_list                | 5.08 us                                                | 4.98 us: 1.02x faster                                                  |
| xml_etree_parse            | 159 ms                                                 | 156 ms: 1.02x faster                                                   |
| sqlglot_optimize           | 54.8 ms                                                | 53.8 ms: 1.02x faster                                                  |
| xml_etree_iterparse        | 107 ms                                                 | 105 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 715 ms: 1.01x faster                                                   |
| scimark_lu                 | 118 ms                                                 | 116 ms: 1.01x faster                                                   |
| asyncio_tcp                | 491 ms                                                 | 484 ms: 1.01x faster                                                   |
| pycparser                  | 1.18 sec                                               | 1.16 sec: 1.01x faster                                                 |
| create_gc_cycles           | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                  |
| bench_thread_pool          | 842 us                                                 | 833 us: 1.01x faster                                                   |
| sqlite_synth               | 2.83 us                                                | 2.80 us: 1.01x faster                                                  |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.02 ms: 1.01x faster                                                  |
| go                         | 139 ms                                                 | 140 ms: 1.00x slower                                                   |
| async_tree_none_tg         | 450 ms                                                 | 453 ms: 1.01x slower                                                   |
| logging_silent             | 104 ns                                                 | 105 ns: 1.01x slower                                                   |
| regex_effbot               | 3.61 ms                                                | 3.66 ms: 1.01x slower                                                  |
| mdp                        | 2.63 sec                                               | 2.68 sec: 1.02x slower                                                 |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                 |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 746 ms: 1.03x slower                                                   |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.04x slower                                                 |
| async_tree_memoization_tg  | 575 ms                                                 | 597 ms: 1.04x slower                                                   |
| regex_dna                  | 212 ms                                                 | 220 ms: 1.04x slower                                                   |
| richards_super             | 51.5 ms                                                | 53.7 ms: 1.04x slower                                                  |
| regex_v8                   | 23.1 ms                                                | 24.1 ms: 1.04x slower                                                  |
| richards                   | 45.8 ms                                                | 48.2 ms: 1.05x slower                                                  |
| python_startup             | 9.55 ms                                                | 10.3 ms: 1.08x slower                                                  |
| telco                      | 7.10 ms                                                | 8.27 ms: 1.16x slower                                                  |
| pidigits                   | 187 ms                                                 | 226 ms: 1.20x slower                                                   |
| python_startup_no_site     | 6.94 ms                                                | 8.95 ms: 1.29x slower                                                  |
| coverage                   | 72.7 ms                                                | 93.9 ms: 1.29x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (5): json_dumps, asyncio_websockets, bench_mp_pool, asyncio_tcp_ssl, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.91x