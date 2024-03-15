
# Results vs. 3.12.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: 482aac3
- commit date: 2024-02-08
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 287 ms: 1.05x slower                                                           |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                         |
| tornado_http   | 103 ms                                                 | 99.0 ms: 1.04x faster                                                          |
| Geometric mean | (ref)                                                  | 1.00x faster                                                                   |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 455 ms: 1.04x faster                                                           |
| async_tree_memoization     | 578 ms                                                 | 585 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 738 ms: 1.02x slower                                                           |
| async_tree_none_tg         | 450 ms                                                 | 461 ms: 1.02x slower                                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                         |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 608 ms: 1.06x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                   |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                           |
| float          | 84.7 ms                                                | 101 ms: 1.19x slower                                                           |
| nbody          | 97.0 ms                                                | 129 ms: 1.33x slower                                                           |
| Geometric mean | (ref)                                                  | 1.17x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.63 ms: 1.01x slower                                                          |
| regex_compile  | 148 ms                                                 | 156 ms: 1.05x slower                                                           |
| regex_dna      | 212 ms                                                 | 226 ms: 1.06x slower                                                           |
| regex_v8       | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                          |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                                           |
| unpickle_list        | 5.29 us                                                | 4.98 us: 1.06x faster                                                          |
| pickle_dict          | 35.5 us                                                | 33.8 us: 1.05x faster                                                          |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                                          |
| unpickle             | 15.9 us                                                | 15.4 us: 1.03x faster                                                          |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                           |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                          |
| xml_etree_generate   | 89.2 ms                                                | 90.3 ms: 1.01x slower                                                          |
| pickle               | 11.6 us                                                | 11.8 us: 1.02x slower                                                          |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                                          |
| unpickle_pure_python | 230 us                                                 | 237 us: 1.03x slower                                                           |
| xml_etree_iterparse  | 107 ms                                                 | 113 ms: 1.06x slower                                                           |
| tomli_loads          | 2.33 sec                                               | 2.80 sec: 1.20x slower                                                         |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                   |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                          |
| python_startup_no_site | 6.94 ms                                                | 8.76 ms: 1.26x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 15.2 ms: 1.28x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-482aac3 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 116 us: 1.36x faster                                                           |
| unpack_sequence            | 54.0 ns                                                | 45.0 ns: 1.20x faster                                                          |
| pickle_pure_python         | 324 us                                                 | 301 us: 1.08x faster                                                           |
| logging_simple             | 6.46 us                                                | 6.04 us: 1.07x faster                                                          |
| deepcopy_reduce            | 3.35 us                                                | 3.13 us: 1.07x faster                                                          |
| unpickle_list              | 5.29 us                                                | 4.98 us: 1.06x faster                                                          |
| generators                 | 31.2 ms                                                | 29.5 ms: 1.06x faster                                                          |
| logging_format             | 7.23 us                                                | 6.87 us: 1.05x faster                                                          |
| pickle_dict                | 35.5 us                                                | 33.8 us: 1.05x faster                                                          |
| deepcopy                   | 371 us                                                 | 354 us: 1.05x faster                                                           |
| pathlib                    | 19.3 ms                                                | 18.5 ms: 1.05x faster                                                          |
| scimark_sor                | 129 ms                                                 | 124 ms: 1.04x faster                                                           |
| tornado_http               | 103 ms                                                 | 99.0 ms: 1.04x faster                                                          |
| async_tree_none            | 472 ms                                                 | 455 ms: 1.04x faster                                                           |
| json_loads                 | 28.5 us                                                | 27.7 us: 1.03x faster                                                          |
| unpickle                   | 15.9 us                                                | 15.4 us: 1.03x faster                                                          |
| coroutines                 | 23.2 ms                                                | 22.6 ms: 1.03x faster                                                          |
| gc_traversal               | 3.79 ms                                                | 3.70 ms: 1.03x faster                                                          |
| docutils                   | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 166 ms: 1.02x faster                                                           |
| json                       | 5.26 ms                                                | 5.16 ms: 1.02x faster                                                          |
| async_generators           | 463 ms                                                 | 456 ms: 1.01x faster                                                           |
| xml_etree_parse            | 159 ms                                                 | 157 ms: 1.01x faster                                                           |
| create_gc_cycles           | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                          |
| raytrace                   | 312 ms                                                 | 310 ms: 1.01x faster                                                           |
| deltablue                  | 3.72 ms                                                | 3.69 ms: 1.01x faster                                                          |
| asyncio_tcp                | 491 ms                                                 | 489 ms: 1.00x faster                                                           |
| regex_effbot               | 3.61 ms                                                | 3.63 ms: 1.01x slower                                                          |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                           |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                         |
| sympy_integrate            | 21.4 ms                                                | 21.7 ms: 1.01x slower                                                          |
| sqlglot_transpile          | 1.68 ms                                                | 1.70 ms: 1.01x slower                                                          |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                          |
| async_tree_memoization     | 578 ms                                                 | 585 ms: 1.01x slower                                                           |
| xml_etree_generate         | 89.2 ms                                                | 90.3 ms: 1.01x slower                                                          |
| dulwich_log                | 68.5 ms                                                | 69.5 ms: 1.01x slower                                                          |
| mdp                        | 2.63 sec                                               | 2.67 sec: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 738 ms: 1.02x slower                                                           |
| pickle                     | 11.6 us                                                | 11.8 us: 1.02x slower                                                          |
| sqlite_synth               | 2.83 us                                                | 2.89 us: 1.02x slower                                                          |
| bench_thread_pool          | 842 us                                                 | 858 us: 1.02x slower                                                           |
| pickle_list                | 5.08 us                                                | 5.20 us: 1.02x slower                                                          |
| async_tree_none_tg         | 450 ms                                                 | 461 ms: 1.02x slower                                                           |
| unpickle_pure_python       | 230 us                                                 | 237 us: 1.03x slower                                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                         |
| sympy_expand               | 478 ms                                                 | 495 ms: 1.04x slower                                                           |
| meteor_contest             | 112 ms                                                 | 117 ms: 1.04x slower                                                           |
| pycparser                  | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                         |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                         |
| 2to3                       | 274 ms                                                 | 287 ms: 1.05x slower                                                           |
| regex_compile              | 148 ms                                                 | 156 ms: 1.05x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 608 ms: 1.06x slower                                                           |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                          |
| xml_etree_iterparse        | 107 ms                                                 | 113 ms: 1.06x slower                                                           |
| regex_dna                  | 212 ms                                                 | 226 ms: 1.06x slower                                                           |
| sqlglot_normalize          | 110 ms                                                 | 118 ms: 1.07x slower                                                           |
| comprehensions             | 21.8 us                                                | 23.5 us: 1.08x slower                                                          |
| pprint_safe_repr           | 776 ms                                                 | 842 ms: 1.09x slower                                                           |
| sqlglot_optimize           | 54.8 ms                                                | 59.6 ms: 1.09x slower                                                          |
| regex_v8                   | 23.1 ms                                                | 25.3 ms: 1.09x slower                                                          |
| richards_super             | 51.5 ms                                                | 57.1 ms: 1.11x slower                                                          |
| pprint_pformat             | 1.57 sec                                               | 1.74 sec: 1.11x slower                                                         |
| richards                   | 45.8 ms                                                | 51.0 ms: 1.11x slower                                                          |
| crypto_pyaes               | 81.9 ms                                                | 92.1 ms: 1.12x slower                                                          |
| fannkuch                   | 417 ms                                                 | 476 ms: 1.14x slower                                                           |
| pyflate                    | 482 ms                                                 | 553 ms: 1.15x slower                                                           |
| chaos                      | 67.0 ms                                                | 77.8 ms: 1.16x slower                                                          |
| scimark_monte_carlo        | 75.1 ms                                                | 88.3 ms: 1.18x slower                                                          |
| float                      | 84.7 ms                                                | 101 ms: 1.19x slower                                                           |
| tomli_loads                | 2.33 sec                                               | 2.80 sec: 1.20x slower                                                         |
| telco                      | 7.10 ms                                                | 8.82 ms: 1.24x slower                                                          |
| scimark_fft                | 382 ms                                                 | 475 ms: 1.24x slower                                                           |
| nqueens                    | 83.3 ms                                                | 104 ms: 1.25x slower                                                           |
| python_startup_no_site     | 6.94 ms                                                | 8.76 ms: 1.26x slower                                                          |
| go                         | 139 ms                                                 | 177 ms: 1.27x slower                                                           |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.42 ms: 1.27x slower                                                          |
| mako                       | 11.9 ms                                                | 15.2 ms: 1.28x slower                                                          |
| coverage                   | 72.7 ms                                                | 94.9 ms: 1.31x slower                                                          |
| nbody                      | 97.0 ms                                                | 129 ms: 1.33x slower                                                           |
| spectral_norm              | 115 ms                                                 | 157 ms: 1.37x slower                                                           |
| hexiom                     | 6.41 ms                                                | 9.42 ms: 1.47x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                                   |

Benchmark hidden because not significant (12): dask, sympy_str, chameleon, xml_etree_process, deepcopy_memo, bench_mp_pool, asyncio_websockets, sqlglot_parse, logging_silent, async_tree_cpu_io_mixed, scimark_lu, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.93x