
# Results vs. 3.12.0

- fork: faster-cpython
- ref: watched_dict_stats
- machine: linux-x86_64
- commit hash: fe6f94a
- commit date: 2024-02-08
- overall geometric mean: 1.06x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 288 ms: 1.05x slower                                                           |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                         |
| tornado_http   | 103 ms                                                 | 99.4 ms: 1.03x faster                                                          |
| Geometric mean | (ref)                                                  | 1.00x faster                                                                   |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 457 ms: 1.03x faster                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 735 ms: 1.01x slower                                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                         |
| async_tree_none_tg         | 450 ms                                                 | 462 ms: 1.03x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 598 ms: 1.04x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                   |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                           |
| float          | 84.7 ms                                                | 105 ms: 1.24x slower                                                           |
| nbody          | 97.0 ms                                                | 141 ms: 1.45x slower                                                           |
| Geometric mean | (ref)                                                  | 1.22x slower                                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.70 ms: 1.02x slower                                                          |
| regex_v8       | 23.1 ms                                                | 24.4 ms: 1.06x slower                                                          |
| regex_compile  | 148 ms                                                 | 157 ms: 1.06x slower                                                           |
| regex_dna      | 212 ms                                                 | 225 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 301 us: 1.08x faster                                                           |
| unpickle             | 15.9 us                                                | 15.2 us: 1.04x faster                                                          |
| json_loads           | 28.5 us                                                | 27.8 us: 1.03x faster                                                          |
| unpickle_list        | 5.29 us                                                | 5.17 us: 1.02x faster                                                          |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                           |
| pickle_dict          | 35.5 us                                                | 35.3 us: 1.01x faster                                                          |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                          |
| pickle               | 11.6 us                                                | 11.9 us: 1.02x slower                                                          |
| xml_etree_generate   | 89.2 ms                                                | 91.3 ms: 1.02x slower                                                          |
| pickle_list          | 5.08 us                                                | 5.24 us: 1.03x slower                                                          |
| unpickle_pure_python | 230 us                                                 | 240 us: 1.04x slower                                                           |
| xml_etree_iterparse  | 107 ms                                                 | 115 ms: 1.08x slower                                                           |
| tomli_loads          | 2.33 sec                                               | 2.84 sec: 1.22x slower                                                         |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                                   |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                          |
| python_startup_no_site | 6.94 ms                                                | 8.81 ms: 1.27x slower                                                          |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 15.4 ms: 1.30x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240208-linux-x86_64-faster%2dcpython-watched_dict_stats-3.13.0a3+-fe6f94a |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 119 us: 1.33x faster                                                           |
| pickle_pure_python         | 324 us                                                 | 301 us: 1.08x faster                                                           |
| deepcopy_reduce            | 3.35 us                                                | 3.12 us: 1.07x faster                                                          |
| logging_simple             | 6.46 us                                                | 6.10 us: 1.06x faster                                                          |
| generators                 | 31.2 ms                                                | 29.6 ms: 1.06x faster                                                          |
| logging_format             | 7.23 us                                                | 6.94 us: 1.04x faster                                                          |
| deepcopy                   | 371 us                                                 | 356 us: 1.04x faster                                                           |
| scimark_sor                | 129 ms                                                 | 124 ms: 1.04x faster                                                           |
| unpickle                   | 15.9 us                                                | 15.2 us: 1.04x faster                                                          |
| pathlib                    | 19.3 ms                                                | 18.7 ms: 1.03x faster                                                          |
| tornado_http               | 103 ms                                                 | 99.4 ms: 1.03x faster                                                          |
| async_tree_none            | 472 ms                                                 | 457 ms: 1.03x faster                                                           |
| gc_traversal               | 3.79 ms                                                | 3.70 ms: 1.03x faster                                                          |
| json_loads                 | 28.5 us                                                | 27.8 us: 1.03x faster                                                          |
| sympy_sum                  | 169 ms                                                 | 165 ms: 1.03x faster                                                           |
| deltablue                  | 3.72 ms                                                | 3.63 ms: 1.02x faster                                                          |
| unpickle_list              | 5.29 us                                                | 5.17 us: 1.02x faster                                                          |
| json                       | 5.26 ms                                                | 5.15 ms: 1.02x faster                                                          |
| docutils                   | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                         |
| async_generators           | 463 ms                                                 | 456 ms: 1.02x faster                                                           |
| coroutines                 | 23.2 ms                                                | 22.9 ms: 1.01x faster                                                          |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                           |
| pickle_dict                | 35.5 us                                                | 35.3 us: 1.01x faster                                                          |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                           |
| sqlglot_transpile          | 1.68 ms                                                | 1.70 ms: 1.01x slower                                                          |
| deepcopy_memo              | 40.7 us                                                | 41.2 us: 1.01x slower                                                          |
| unpack_sequence            | 54.0 ns                                                | 54.6 ns: 1.01x slower                                                          |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.81 sec: 1.01x slower                                                         |
| dulwich_log                | 68.5 ms                                                | 69.3 ms: 1.01x slower                                                          |
| scimark_lu                 | 118 ms                                                 | 119 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 735 ms: 1.01x slower                                                           |
| logging_silent             | 104 ns                                                 | 106 ns: 1.01x slower                                                           |
| sympy_integrate            | 21.4 ms                                                | 21.7 ms: 1.01x slower                                                          |
| bench_thread_pool          | 842 us                                                 | 855 us: 1.02x slower                                                           |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                          |
| sqlite_synth               | 2.83 us                                                | 2.90 us: 1.02x slower                                                          |
| pickle                     | 11.6 us                                                | 11.9 us: 1.02x slower                                                          |
| xml_etree_generate         | 89.2 ms                                                | 91.3 ms: 1.02x slower                                                          |
| regex_effbot               | 3.61 ms                                                | 3.70 ms: 1.02x slower                                                          |
| async_tree_io_tg           | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                         |
| async_tree_none_tg         | 450 ms                                                 | 462 ms: 1.03x slower                                                           |
| pickle_list                | 5.08 us                                                | 5.24 us: 1.03x slower                                                          |
| sympy_expand               | 478 ms                                                 | 495 ms: 1.03x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                         |
| async_tree_memoization_tg  | 575 ms                                                 | 598 ms: 1.04x slower                                                           |
| pycparser                  | 1.18 sec                                               | 1.23 sec: 1.04x slower                                                         |
| unpickle_pure_python       | 230 us                                                 | 240 us: 1.04x slower                                                           |
| meteor_contest             | 112 ms                                                 | 118 ms: 1.05x slower                                                           |
| 2to3                       | 274 ms                                                 | 288 ms: 1.05x slower                                                           |
| regex_v8                   | 23.1 ms                                                | 24.4 ms: 1.06x slower                                                          |
| sqlglot_normalize          | 110 ms                                                 | 117 ms: 1.06x slower                                                           |
| regex_compile              | 148 ms                                                 | 157 ms: 1.06x slower                                                           |
| regex_dna                  | 212 ms                                                 | 225 ms: 1.06x slower                                                           |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                          |
| pprint_safe_repr           | 776 ms                                                 | 834 ms: 1.07x slower                                                           |
| mdp                        | 2.63 sec                                               | 2.83 sec: 1.08x slower                                                         |
| xml_etree_iterparse        | 107 ms                                                 | 115 ms: 1.08x slower                                                           |
| sqlglot_optimize           | 54.8 ms                                                | 59.0 ms: 1.08x slower                                                          |
| richards                   | 45.8 ms                                                | 50.2 ms: 1.09x slower                                                          |
| comprehensions             | 21.8 us                                                | 23.9 us: 1.10x slower                                                          |
| richards_super             | 51.5 ms                                                | 56.8 ms: 1.10x slower                                                          |
| pprint_pformat             | 1.57 sec                                               | 1.75 sec: 1.11x slower                                                         |
| crypto_pyaes               | 81.9 ms                                                | 93.8 ms: 1.15x slower                                                          |
| fannkuch                   | 417 ms                                                 | 490 ms: 1.17x slower                                                           |
| pyflate                    | 482 ms                                                 | 573 ms: 1.19x slower                                                           |
| chaos                      | 67.0 ms                                                | 79.8 ms: 1.19x slower                                                          |
| scimark_monte_carlo        | 75.1 ms                                                | 89.8 ms: 1.20x slower                                                          |
| tomli_loads                | 2.33 sec                                               | 2.84 sec: 1.22x slower                                                         |
| float                      | 84.7 ms                                                | 105 ms: 1.24x slower                                                           |
| nqueens                    | 83.3 ms                                                | 104 ms: 1.25x slower                                                           |
| telco                      | 7.10 ms                                                | 8.95 ms: 1.26x slower                                                          |
| go                         | 139 ms                                                 | 177 ms: 1.27x slower                                                           |
| python_startup_no_site     | 6.94 ms                                                | 8.81 ms: 1.27x slower                                                          |
| mako                       | 11.9 ms                                                | 15.4 ms: 1.30x slower                                                          |
| scimark_fft                | 382 ms                                                 | 496 ms: 1.30x slower                                                           |
| coverage                   | 72.7 ms                                                | 94.7 ms: 1.30x slower                                                          |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.74 ms: 1.33x slower                                                          |
| nbody                      | 97.0 ms                                                | 141 ms: 1.45x slower                                                           |
| spectral_norm              | 115 ms                                                 | 167 ms: 1.45x slower                                                           |
| hexiom                     | 6.41 ms                                                | 9.60 ms: 1.50x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.06x slower                                                                   |

Benchmark hidden because not significant (13): dask, chameleon, create_gc_cycles, raytrace, asyncio_tcp, sympy_str, bench_mp_pool, xml_etree_process, asyncio_websockets, async_tree_cpu_io_mixed, sqlglot_parse, async_tree_memoization, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.93x