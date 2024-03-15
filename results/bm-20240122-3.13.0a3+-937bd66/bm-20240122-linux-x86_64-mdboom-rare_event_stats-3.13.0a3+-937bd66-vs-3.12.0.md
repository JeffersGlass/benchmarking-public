
# Results vs. 3.12.0

- fork: mdboom
- ref: rare_event_stats
- machine: linux-x86_64
- commit hash: 937bd66
- commit date: 2024-01-22
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                               |
| chameleon      | 7.41 ms                                                | 7.06 ms: 1.05x faster                                              |
| docutils       | 2.77 sec                                               | 2.60 sec: 1.07x faster                                             |
| tornado_http   | 103 ms                                                 | 94.2 ms: 1.09x faster                                              |
| Geometric mean | (ref)                                                  | 1.06x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 431 ms: 1.09x faster                                               |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 702 ms: 1.03x faster                                               |
| async_tree_memoization     | 578 ms                                                 | 560 ms: 1.03x faster                                               |
| async_tree_none_tg         | 450 ms                                                 | 438 ms: 1.03x faster                                               |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 716 ms: 1.01x faster                                               |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                             |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                             |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                       |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 86.1 ms: 1.13x faster                                              |
| float          | 84.7 ms                                                | 80.1 ms: 1.06x faster                                              |
| Geometric mean | (ref)                                                  | 1.06x faster                                                       |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 130 ms: 1.14x faster                                               |
| regex_effbot   | 3.61 ms                                                | 3.54 ms: 1.02x faster                                              |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                               |
| regex_v8       | 23.1 ms                                                | 25.5 ms: 1.10x slower                                              |
| Geometric mean | (ref)                                                  | 1.00x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.12 sec: 1.10x faster                                             |
| pickle_pure_python   | 324 us                                                 | 297 us: 1.09x faster                                               |
| unpickle_pure_python | 230 us                                                 | 212 us: 1.08x faster                                               |
| xml_etree_process    | 61.7 ms                                                | 58.6 ms: 1.05x faster                                              |
| xml_etree_generate   | 89.2 ms                                                | 85.6 ms: 1.04x faster                                              |
| unpickle             | 15.9 us                                                | 15.4 us: 1.03x faster                                              |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.03x faster                                               |
| pickle_dict          | 35.5 us                                                | 34.8 us: 1.02x faster                                              |
| json_loads           | 28.5 us                                                | 28.1 us: 1.02x faster                                              |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                               |
| pickle               | 11.6 us                                                | 11.7 us: 1.01x slower                                              |
| unpickle_list        | 5.29 us                                                | 5.41 us: 1.02x slower                                              |
| pickle_list          | 5.08 us                                                | 5.27 us: 1.04x slower                                              |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                       |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.05x slower                                              |
| python_startup_no_site | 6.94 ms                                                | 8.68 ms: 1.25x slower                                              |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.1 ms: 1.08x faster                                              |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 110 us: 1.43x faster                                               |
| comprehensions             | 21.8 us                                                | 16.1 us: 1.35x faster                                              |
| raytrace                   | 312 ms                                                 | 257 ms: 1.21x faster                                               |
| unpack_sequence            | 54.0 ns                                                | 45.2 ns: 1.19x faster                                              |
| deltablue                  | 3.72 ms                                                | 3.15 ms: 1.18x faster                                              |
| logging_format             | 7.23 us                                                | 6.26 us: 1.16x faster                                              |
| crypto_pyaes               | 81.9 ms                                                | 70.9 ms: 1.15x faster                                              |
| regex_compile              | 148 ms                                                 | 130 ms: 1.14x faster                                               |
| sympy_sum                  | 169 ms                                                 | 149 ms: 1.14x faster                                               |
| scimark_monte_carlo        | 75.1 ms                                                | 66.4 ms: 1.13x faster                                              |
| chaos                      | 67.0 ms                                                | 59.5 ms: 1.13x faster                                              |
| nbody                      | 97.0 ms                                                | 86.1 ms: 1.13x faster                                              |
| logging_simple             | 6.46 us                                                | 5.76 us: 1.12x faster                                              |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                              |
| tomli_loads                | 2.33 sec                                               | 2.12 sec: 1.10x faster                                             |
| async_tree_none            | 472 ms                                                 | 431 ms: 1.09x faster                                               |
| scimark_fft                | 382 ms                                                 | 350 ms: 1.09x faster                                               |
| pickle_pure_python         | 324 us                                                 | 297 us: 1.09x faster                                               |
| tornado_http               | 103 ms                                                 | 94.2 ms: 1.09x faster                                              |
| hexiom                     | 6.41 ms                                                | 5.89 ms: 1.09x faster                                              |
| deepcopy_reduce            | 3.35 us                                                | 3.07 us: 1.09x faster                                              |
| sqlglot_parse              | 1.36 ms                                                | 1.25 ms: 1.09x faster                                              |
| unpickle_pure_python       | 230 us                                                 | 212 us: 1.08x faster                                               |
| deepcopy_memo              | 40.7 us                                                | 37.7 us: 1.08x faster                                              |
| mako                       | 11.9 ms                                                | 11.1 ms: 1.08x faster                                              |
| sympy_str                  | 300 ms                                                 | 279 ms: 1.08x faster                                               |
| sqlglot_transpile          | 1.68 ms                                                | 1.58 ms: 1.07x faster                                              |
| deepcopy                   | 371 us                                                 | 348 us: 1.07x faster                                               |
| generators                 | 31.2 ms                                                | 29.3 ms: 1.07x faster                                              |
| docutils                   | 2.77 sec                                               | 2.60 sec: 1.07x faster                                             |
| scimark_sor                | 129 ms                                                 | 121 ms: 1.06x faster                                               |
| spectral_norm              | 115 ms                                                 | 108 ms: 1.06x faster                                               |
| pathlib                    | 19.3 ms                                                | 18.3 ms: 1.06x faster                                              |
| float                      | 84.7 ms                                                | 80.1 ms: 1.06x faster                                              |
| pprint_safe_repr           | 776 ms                                                 | 736 ms: 1.05x faster                                               |
| xml_etree_process          | 61.7 ms                                                | 58.6 ms: 1.05x faster                                              |
| chameleon                  | 7.41 ms                                                | 7.06 ms: 1.05x faster                                              |
| pyflate                    | 482 ms                                                 | 460 ms: 1.05x faster                                               |
| dulwich_log                | 68.5 ms                                                | 65.3 ms: 1.05x faster                                              |
| async_generators           | 463 ms                                                 | 442 ms: 1.05x faster                                               |
| scimark_lu                 | 118 ms                                                 | 113 ms: 1.05x faster                                               |
| xml_etree_generate         | 89.2 ms                                                | 85.6 ms: 1.04x faster                                              |
| meteor_contest             | 112 ms                                                 | 108 ms: 1.04x faster                                               |
| 2to3                       | 274 ms                                                 | 264 ms: 1.04x faster                                               |
| pprint_pformat             | 1.57 sec                                               | 1.51 sec: 1.04x faster                                             |
| nqueens                    | 83.3 ms                                                | 80.1 ms: 1.04x faster                                              |
| coroutines                 | 23.2 ms                                                | 22.3 ms: 1.04x faster                                              |
| fannkuch                   | 417 ms                                                 | 403 ms: 1.03x faster                                               |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 702 ms: 1.03x faster                                               |
| unpickle                   | 15.9 us                                                | 15.4 us: 1.03x faster                                              |
| dask                       | 372 ms                                                 | 360 ms: 1.03x faster                                               |
| async_tree_memoization     | 578 ms                                                 | 560 ms: 1.03x faster                                               |
| sympy_expand               | 478 ms                                                 | 464 ms: 1.03x faster                                               |
| json                       | 5.26 ms                                                | 5.11 ms: 1.03x faster                                              |
| sqlglot_normalize          | 110 ms                                                 | 107 ms: 1.03x faster                                               |
| xml_etree_iterparse        | 107 ms                                                 | 104 ms: 1.03x faster                                               |
| async_tree_none_tg         | 450 ms                                                 | 438 ms: 1.03x faster                                               |
| pycparser                  | 1.18 sec                                               | 1.15 sec: 1.02x faster                                             |
| asyncio_tcp                | 491 ms                                                 | 480 ms: 1.02x faster                                               |
| go                         | 139 ms                                                 | 137 ms: 1.02x faster                                               |
| bench_thread_pool          | 842 us                                                 | 825 us: 1.02x faster                                               |
| regex_effbot               | 3.61 ms                                                | 3.54 ms: 1.02x faster                                              |
| pickle_dict                | 35.5 us                                                | 34.8 us: 1.02x faster                                              |
| json_loads                 | 28.5 us                                                | 28.1 us: 1.02x faster                                              |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 716 ms: 1.01x faster                                               |
| sqlglot_optimize           | 54.8 ms                                                | 54.2 ms: 1.01x faster                                              |
| create_gc_cycles           | 1.48 ms                                                | 1.46 ms: 1.01x faster                                              |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                               |
| sqlite_synth               | 2.83 us                                                | 2.81 us: 1.01x faster                                              |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.00x faster                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                             |
| asyncio_websockets         | 551 ms                                                 | 557 ms: 1.01x slower                                               |
| pickle                     | 11.6 us                                                | 11.7 us: 1.01x slower                                              |
| logging_silent             | 104 ns                                                 | 106 ns: 1.01x slower                                               |
| async_tree_io              | 1.16 sec                                               | 1.17 sec: 1.01x slower                                             |
| unpickle_list              | 5.29 us                                                | 5.41 us: 1.02x slower                                              |
| richards                   | 45.8 ms                                                | 47.4 ms: 1.03x slower                                              |
| richards_super             | 51.5 ms                                                | 53.3 ms: 1.03x slower                                              |
| mdp                        | 2.63 sec                                               | 2.73 sec: 1.04x slower                                             |
| pickle_list                | 5.08 us                                                | 5.27 us: 1.04x slower                                              |
| gc_traversal               | 3.79 ms                                                | 3.94 ms: 1.04x slower                                              |
| regex_dna                  | 212 ms                                                 | 222 ms: 1.05x slower                                               |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.05x slower                                              |
| regex_v8                   | 23.1 ms                                                | 25.5 ms: 1.10x slower                                              |
| telco                      | 7.10 ms                                                | 8.24 ms: 1.16x slower                                              |
| python_startup_no_site     | 6.94 ms                                                | 8.68 ms: 1.25x slower                                              |
| coverage                   | 72.7 ms                                                | 94.4 ms: 1.30x slower                                              |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                       |

Benchmark hidden because not significant (6): async_tree_memoization_tg, scimark_sparse_mat_mult, pidigits, bench_mp_pool, json_dumps, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x