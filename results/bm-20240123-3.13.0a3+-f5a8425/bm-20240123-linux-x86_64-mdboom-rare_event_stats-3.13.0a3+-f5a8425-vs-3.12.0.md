
# Results vs. 3.12.0

- fork: mdboom
- ref: rare_event_stats
- machine: linux-x86_64
- commit hash: f5a8425
- commit date: 2024-01-23
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 263 ms: 1.04x faster                                               |
| chameleon      | 7.41 ms                                                | 6.87 ms: 1.08x faster                                              |
| docutils       | 2.77 sec                                               | 2.64 sec: 1.05x faster                                             |
| tornado_http   | 103 ms                                                 | 94.8 ms: 1.08x faster                                              |
| Geometric mean | (ref)                                                  | 1.06x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 433 ms: 1.09x faster                                               |
| async_tree_memoization     | 578 ms                                                 | 561 ms: 1.03x faster                                               |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 705 ms: 1.03x faster                                               |
| async_tree_none_tg         | 450 ms                                                 | 438 ms: 1.03x faster                                               |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 716 ms: 1.01x faster                                               |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                             |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                             |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                       |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.6 ms: 1.09x faster                                              |
| float          | 84.7 ms                                                | 80.5 ms: 1.05x faster                                              |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                               |
| Geometric mean | (ref)                                                  | 1.05x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                               |
| regex_effbot   | 3.61 ms                                                | 3.55 ms: 1.02x faster                                              |
| regex_dna      | 212 ms                                                 | 221 ms: 1.04x slower                                               |
| regex_v8       | 23.1 ms                                                | 25.4 ms: 1.10x slower                                              |
| Geometric mean | (ref)                                                  | 1.00x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.14 sec: 1.09x faster                                             |
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                               |
| unpickle_pure_python | 230 us                                                 | 215 us: 1.07x faster                                               |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                              |
| xml_etree_process    | 61.7 ms                                                | 58.8 ms: 1.05x faster                                              |
| pickle_dict          | 35.5 us                                                | 34.0 us: 1.04x faster                                              |
| xml_etree_generate   | 89.2 ms                                                | 86.3 ms: 1.03x faster                                              |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                               |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                              |
| pickle_list          | 5.08 us                                                | 5.11 us: 1.01x slower                                              |
| unpickle_list        | 5.29 us                                                | 5.32 us: 1.01x slower                                              |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                              |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                       |

Benchmark hidden because not significant (2): xml_etree_parse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                              |
| python_startup_no_site | 6.94 ms                                                | 8.73 ms: 1.26x slower                                              |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.0 ms: 1.08x faster                                              |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 109 us: 1.45x faster                                               |
| comprehensions             | 21.8 us                                                | 16.2 us: 1.34x faster                                              |
| raytrace                   | 312 ms                                                 | 260 ms: 1.20x faster                                               |
| deltablue                  | 3.72 ms                                                | 3.22 ms: 1.16x faster                                              |
| regex_compile              | 148 ms                                                 | 129 ms: 1.15x faster                                               |
| logging_format             | 7.23 us                                                | 6.33 us: 1.14x faster                                              |
| crypto_pyaes               | 81.9 ms                                                | 71.7 ms: 1.14x faster                                              |
| chaos                      | 67.0 ms                                                | 58.7 ms: 1.14x faster                                              |
| sympy_sum                  | 169 ms                                                 | 149 ms: 1.14x faster                                               |
| logging_simple             | 6.46 us                                                | 5.69 us: 1.13x faster                                              |
| scimark_monte_carlo        | 75.1 ms                                                | 66.6 ms: 1.13x faster                                              |
| deepcopy_reduce            | 3.35 us                                                | 2.99 us: 1.12x faster                                              |
| sympy_str                  | 300 ms                                                 | 273 ms: 1.10x faster                                               |
| sympy_integrate            | 21.4 ms                                                | 19.5 ms: 1.10x faster                                              |
| deepcopy                   | 371 us                                                 | 339 us: 1.10x faster                                               |
| nbody                      | 97.0 ms                                                | 88.6 ms: 1.09x faster                                              |
| deepcopy_memo              | 40.7 us                                                | 37.3 us: 1.09x faster                                              |
| sqlglot_parse              | 1.36 ms                                                | 1.25 ms: 1.09x faster                                              |
| async_tree_none            | 472 ms                                                 | 433 ms: 1.09x faster                                               |
| tomli_loads                | 2.33 sec                                               | 2.14 sec: 1.09x faster                                             |
| pickle_pure_python         | 324 us                                                 | 299 us: 1.08x faster                                               |
| tornado_http               | 103 ms                                                 | 94.8 ms: 1.08x faster                                              |
| mako                       | 11.9 ms                                                | 11.0 ms: 1.08x faster                                              |
| chameleon                  | 7.41 ms                                                | 6.87 ms: 1.08x faster                                              |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 4.69 ms: 1.08x faster                                              |
| scimark_sor                | 129 ms                                                 | 121 ms: 1.07x faster                                               |
| unpickle_pure_python       | 230 us                                                 | 215 us: 1.07x faster                                               |
| unpickle                   | 15.9 us                                                | 14.9 us: 1.07x faster                                              |
| sqlglot_transpile          | 1.68 ms                                                | 1.58 ms: 1.07x faster                                              |
| scimark_fft                | 382 ms                                                 | 360 ms: 1.06x faster                                               |
| generators                 | 31.2 ms                                                | 29.4 ms: 1.06x faster                                              |
| pprint_safe_repr           | 776 ms                                                 | 733 ms: 1.06x faster                                               |
| pathlib                    | 19.3 ms                                                | 18.3 ms: 1.06x faster                                              |
| coroutines                 | 23.2 ms                                                | 21.9 ms: 1.06x faster                                              |
| pyflate                    | 482 ms                                                 | 458 ms: 1.05x faster                                               |
| float                      | 84.7 ms                                                | 80.5 ms: 1.05x faster                                              |
| pprint_pformat             | 1.57 sec                                               | 1.49 sec: 1.05x faster                                             |
| async_generators           | 463 ms                                                 | 441 ms: 1.05x faster                                               |
| docutils                   | 2.77 sec                                               | 2.64 sec: 1.05x faster                                             |
| nqueens                    | 83.3 ms                                                | 79.4 ms: 1.05x faster                                              |
| xml_etree_process          | 61.7 ms                                                | 58.8 ms: 1.05x faster                                              |
| scimark_lu                 | 118 ms                                                 | 113 ms: 1.05x faster                                               |
| spectral_norm              | 115 ms                                                 | 110 ms: 1.05x faster                                               |
| hexiom                     | 6.41 ms                                                | 6.13 ms: 1.05x faster                                              |
| pickle_dict                | 35.5 us                                                | 34.0 us: 1.04x faster                                              |
| 2to3                       | 274 ms                                                 | 263 ms: 1.04x faster                                               |
| mdp                        | 2.63 sec                                               | 2.53 sec: 1.04x faster                                             |
| dulwich_log                | 68.5 ms                                                | 65.9 ms: 1.04x faster                                              |
| sympy_expand               | 478 ms                                                 | 460 ms: 1.04x faster                                               |
| fannkuch                   | 417 ms                                                 | 402 ms: 1.04x faster                                               |
| xml_etree_generate         | 89.2 ms                                                | 86.3 ms: 1.03x faster                                              |
| meteor_contest             | 112 ms                                                 | 109 ms: 1.03x faster                                               |
| sqlglot_normalize          | 110 ms                                                 | 107 ms: 1.03x faster                                               |
| async_tree_memoization     | 578 ms                                                 | 561 ms: 1.03x faster                                               |
| dask                       | 372 ms                                                 | 361 ms: 1.03x faster                                               |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 705 ms: 1.03x faster                                               |
| async_tree_none_tg         | 450 ms                                                 | 438 ms: 1.03x faster                                               |
| json                       | 5.26 ms                                                | 5.14 ms: 1.02x faster                                              |
| go                         | 139 ms                                                 | 137 ms: 1.02x faster                                               |
| xml_etree_iterparse        | 107 ms                                                 | 105 ms: 1.02x faster                                               |
| asyncio_tcp                | 491 ms                                                 | 482 ms: 1.02x faster                                               |
| sqlglot_optimize           | 54.8 ms                                                | 53.9 ms: 1.02x faster                                              |
| regex_effbot               | 3.61 ms                                                | 3.55 ms: 1.02x faster                                              |
| pycparser                  | 1.18 sec                                               | 1.16 sec: 1.01x faster                                             |
| logging_silent             | 104 ns                                                 | 103 ns: 1.01x faster                                               |
| json_loads                 | 28.5 us                                                | 28.1 us: 1.01x faster                                              |
| gc_traversal               | 3.79 ms                                                | 3.74 ms: 1.01x faster                                              |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 716 ms: 1.01x faster                                               |
| bench_thread_pool          | 842 us                                                 | 835 us: 1.01x faster                                               |
| create_gc_cycles           | 1.48 ms                                                | 1.47 ms: 1.00x faster                                              |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.78 sec: 1.00x faster                                             |
| pidigits                   | 187 ms                                                 | 187 ms: 1.00x faster                                               |
| pickle_list                | 5.08 us                                                | 5.11 us: 1.01x slower                                              |
| unpickle_list              | 5.29 us                                                | 5.32 us: 1.01x slower                                              |
| async_tree_io_tg           | 1.18 sec                                               | 1.19 sec: 1.01x slower                                             |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                              |
| asyncio_websockets         | 551 ms                                                 | 556 ms: 1.01x slower                                               |
| unpack_sequence            | 54.0 ns                                                | 55.0 ns: 1.02x slower                                              |
| async_tree_io              | 1.16 sec                                               | 1.18 sec: 1.02x slower                                             |
| richards_super             | 51.5 ms                                                | 53.2 ms: 1.03x slower                                              |
| richards                   | 45.8 ms                                                | 47.4 ms: 1.03x slower                                              |
| regex_dna                  | 212 ms                                                 | 221 ms: 1.04x slower                                               |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                              |
| regex_v8                   | 23.1 ms                                                | 25.4 ms: 1.10x slower                                              |
| telco                      | 7.10 ms                                                | 8.33 ms: 1.17x slower                                              |
| python_startup_no_site     | 6.94 ms                                                | 8.73 ms: 1.26x slower                                              |
| coverage                   | 72.7 ms                                                | 93.9 ms: 1.29x slower                                              |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                       |

Benchmark hidden because not significant (6): async_tree_memoization_tg, sqlite_synth, xml_etree_parse, bench_mp_pool, pickle, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.92x