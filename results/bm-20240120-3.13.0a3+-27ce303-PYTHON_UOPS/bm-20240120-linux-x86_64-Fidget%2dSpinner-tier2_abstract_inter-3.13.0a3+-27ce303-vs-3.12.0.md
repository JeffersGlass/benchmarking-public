
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.03x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.19x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 287 ms: 1.05x slower                                                             |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                           |
| tornado_http   | 103 ms                                                 | 97.5 ms: 1.05x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 449 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 736 ms: 1.01x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 460 ms: 1.02x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                             |
| float          | 84.7 ms                                                | 89.4 ms: 1.06x slower                                                            |
| nbody          | 97.0 ms                                                | 119 ms: 1.23x slower                                                             |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                            |
| regex_compile  | 148 ms                                                 | 150 ms: 1.01x slower                                                             |
| regex_dna      | 212 ms                                                 | 227 ms: 1.07x slower                                                             |
| regex_v8       | 23.1 ms                                                | 25.9 ms: 1.12x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 305 us: 1.06x faster                                                             |
| unpickle_list        | 5.29 us                                                | 5.01 us: 1.05x faster                                                            |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                                            |
| pickle_dict          | 35.5 us                                                | 34.8 us: 1.02x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                             |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 61.2 ms: 1.01x faster                                                            |
| xml_etree_generate   | 89.2 ms                                                | 89.6 ms: 1.01x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                             |
| pickle               | 11.6 us                                                | 11.9 us: 1.03x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.25 us: 1.03x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 238 us: 1.04x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.77 ms: 1.26x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.7 ms: 1.15x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 120 us: 1.32x faster                                                             |
| logging_simple             | 6.46 us                                                | 5.96 us: 1.08x faster                                                            |
| logging_format             | 7.23 us                                                | 6.77 us: 1.07x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 305 us: 1.06x faster                                                             |
| pathlib                    | 19.3 ms                                                | 18.3 ms: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                             |
| unpickle_list              | 5.29 us                                                | 5.01 us: 1.05x faster                                                            |
| deepcopy_reduce            | 3.35 us                                                | 3.17 us: 1.05x faster                                                            |
| raytrace                   | 312 ms                                                 | 296 ms: 1.05x faster                                                             |
| tornado_http               | 103 ms                                                 | 97.5 ms: 1.05x faster                                                            |
| async_tree_none            | 472 ms                                                 | 449 ms: 1.05x faster                                                             |
| generators                 | 31.2 ms                                                | 29.7 ms: 1.05x faster                                                            |
| coroutines                 | 23.2 ms                                                | 22.2 ms: 1.05x faster                                                            |
| unpickle                   | 15.9 us                                                | 15.3 us: 1.04x faster                                                            |
| comprehensions             | 21.8 us                                                | 21.1 us: 1.03x faster                                                            |
| deepcopy                   | 371 us                                                 | 361 us: 1.03x faster                                                             |
| sympy_str                  | 300 ms                                                 | 292 ms: 1.02x faster                                                             |
| sympy_integrate            | 21.4 ms                                                | 20.9 ms: 1.02x faster                                                            |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                            |
| pickle_dict                | 35.5 us                                                | 34.8 us: 1.02x faster                                                            |
| docutils                   | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                           |
| json                       | 5.26 ms                                                | 5.17 ms: 1.02x faster                                                            |
| xml_etree_parse            | 159 ms                                                 | 157 ms: 1.02x faster                                                             |
| json_loads                 | 28.5 us                                                | 28.1 us: 1.01x faster                                                            |
| xml_etree_process          | 61.7 ms                                                | 61.2 ms: 1.01x faster                                                            |
| sqlglot_transpile          | 1.68 ms                                                | 1.67 ms: 1.01x faster                                                            |
| async_generators           | 463 ms                                                 | 459 ms: 1.01x faster                                                             |
| create_gc_cycles           | 1.48 ms                                                | 1.46 ms: 1.01x faster                                                            |
| logging_silent             | 104 ns                                                 | 105 ns: 1.00x slower                                                             |
| pidigits                   | 187 ms                                                 | 188 ms: 1.00x slower                                                             |
| xml_etree_generate         | 89.2 ms                                                | 89.6 ms: 1.01x slower                                                            |
| sqlite_synth               | 2.83 us                                                | 2.86 us: 1.01x slower                                                            |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| bench_thread_pool          | 842 us                                                 | 850 us: 1.01x slower                                                             |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| meteor_contest             | 112 ms                                                 | 114 ms: 1.01x slower                                                             |
| deepcopy_memo              | 40.7 us                                                | 41.2 us: 1.01x slower                                                            |
| regex_effbot               | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                            |
| regex_compile              | 148 ms                                                 | 150 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 736 ms: 1.01x slower                                                             |
| asyncio_tcp                | 491 ms                                                 | 500 ms: 1.02x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 460 ms: 1.02x slower                                                             |
| xml_etree_iterparse        | 107 ms                                                 | 109 ms: 1.02x slower                                                             |
| pycparser                  | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                           |
| crypto_pyaes               | 81.9 ms                                                | 84.0 ms: 1.03x slower                                                            |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                           |
| sympy_expand               | 478 ms                                                 | 492 ms: 1.03x slower                                                             |
| pickle                     | 11.6 us                                                | 11.9 us: 1.03x slower                                                            |
| pickle_list                | 5.08 us                                                | 5.25 us: 1.03x slower                                                            |
| unpickle_pure_python       | 230 us                                                 | 238 us: 1.04x slower                                                             |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| scimark_sor                | 129 ms                                                 | 134 ms: 1.04x slower                                                             |
| pprint_safe_repr           | 776 ms                                                 | 810 ms: 1.04x slower                                                             |
| 2to3                       | 274 ms                                                 | 287 ms: 1.05x slower                                                             |
| sqlglot_normalize          | 110 ms                                                 | 116 ms: 1.05x slower                                                             |
| gc_traversal               | 3.79 ms                                                | 3.98 ms: 1.05x slower                                                            |
| unpack_sequence            | 54.0 ns                                                | 56.7 ns: 1.05x slower                                                            |
| float                      | 84.7 ms                                                | 89.4 ms: 1.06x slower                                                            |
| richards                   | 45.8 ms                                                | 48.4 ms: 1.06x slower                                                            |
| richards_super             | 51.5 ms                                                | 54.5 ms: 1.06x slower                                                            |
| scimark_monte_carlo        | 75.1 ms                                                | 79.5 ms: 1.06x slower                                                            |
| fannkuch                   | 417 ms                                                 | 442 ms: 1.06x slower                                                             |
| python_startup             | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| chaos                      | 67.0 ms                                                | 71.3 ms: 1.06x slower                                                            |
| sqlglot_optimize           | 54.8 ms                                                | 58.4 ms: 1.07x slower                                                            |
| regex_dna                  | 212 ms                                                 | 227 ms: 1.07x slower                                                             |
| mdp                        | 2.63 sec                                               | 2.83 sec: 1.08x slower                                                           |
| pprint_pformat             | 1.57 sec                                               | 1.69 sec: 1.08x slower                                                           |
| pyflate                    | 482 ms                                                 | 522 ms: 1.08x slower                                                             |
| scimark_fft                | 382 ms                                                 | 422 ms: 1.11x slower                                                             |
| regex_v8                   | 23.1 ms                                                | 25.9 ms: 1.12x slower                                                            |
| nqueens                    | 83.3 ms                                                | 93.8 ms: 1.13x slower                                                            |
| go                         | 139 ms                                                 | 157 ms: 1.13x slower                                                             |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.72 ms: 1.13x slower                                                            |
| mako                       | 11.9 ms                                                | 13.7 ms: 1.15x slower                                                            |
| spectral_norm              | 115 ms                                                 | 138 ms: 1.20x slower                                                             |
| nbody                      | 97.0 ms                                                | 119 ms: 1.23x slower                                                             |
| deltablue                  | 3.72 ms                                                | 4.59 ms: 1.24x slower                                                            |
| telco                      | 7.10 ms                                                | 8.82 ms: 1.24x slower                                                            |
| python_startup_no_site     | 6.94 ms                                                | 8.77 ms: 1.26x slower                                                            |
| hexiom                     | 6.41 ms                                                | 8.15 ms: 1.27x slower                                                            |
| coverage                   | 72.7 ms                                                | 95.2 ms: 1.31x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (11): async_tree_cpu_io_mixed, dask, tomli_loads, chameleon, asyncio_websockets, async_tree_memoization, bench_mp_pool, dulwich_log, async_tree_memoization_tg, scimark_lu, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.19x