
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 6e55480
- commit date: 2024-01-24
- overall geometric mean: 1.02x slower
- HPT reliability: 99.97%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 286 ms: 1.04x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.33 ms: 1.01x faster                                                            |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| tornado_http   | 103 ms                                                 | 99.2 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 447 ms: 1.06x faster                                                             |
| async_tree_memoization     | 578 ms                                                 | 571 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 717 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 734 ms: 1.01x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 455 ms: 1.01x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 599 ms: 1.04x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                             |
| float          | 84.7 ms                                                | 87.8 ms: 1.04x slower                                                            |
| nbody          | 97.0 ms                                                | 110 ms: 1.13x slower                                                             |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 149 ms: 1.01x slower                                                             |
| regex_effbot   | 3.61 ms                                                | 3.64 ms: 1.01x slower                                                            |
| regex_dna      | 212 ms                                                 | 223 ms: 1.05x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 300 us: 1.08x faster                                                             |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                                            |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                             |
| xml_etree_process    | 61.7 ms                                                | 60.8 ms: 1.02x faster                                                            |
| xml_etree_generate   | 89.2 ms                                                | 88.5 ms: 1.01x faster                                                            |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                            |
| unpickle_list        | 5.29 us                                                | 5.31 us: 1.01x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 235 us: 1.02x slower                                                             |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| pickle_list          | 5.08 us                                                | 5.24 us: 1.03x slower                                                            |
| tomli_loads          | 2.33 sec                                               | 2.47 sec: 1.06x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.3 ms: 1.12x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpack_sequence            | 54.0 ns                                                | 39.0 ns: 1.38x faster                                                            |
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.35x faster                                                             |
| pickle_pure_python         | 324 us                                                 | 300 us: 1.08x faster                                                             |
| unpickle                   | 15.9 us                                                | 14.9 us: 1.07x faster                                                            |
| logging_simple             | 6.46 us                                                | 6.06 us: 1.07x faster                                                            |
| comprehensions             | 21.8 us                                                | 20.5 us: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                             |
| async_tree_none            | 472 ms                                                 | 447 ms: 1.06x faster                                                             |
| deepcopy_reduce            | 3.35 us                                                | 3.17 us: 1.05x faster                                                            |
| logging_format             | 7.23 us                                                | 6.86 us: 1.05x faster                                                            |
| generators                 | 31.2 ms                                                | 29.6 ms: 1.05x faster                                                            |
| raytrace                   | 312 ms                                                 | 297 ms: 1.05x faster                                                             |
| asyncio_tcp                | 491 ms                                                 | 469 ms: 1.05x faster                                                             |
| coroutines                 | 23.2 ms                                                | 22.3 ms: 1.04x faster                                                            |
| sympy_str                  | 300 ms                                                 | 288 ms: 1.04x faster                                                             |
| tornado_http               | 103 ms                                                 | 99.2 ms: 1.03x faster                                                            |
| scimark_sor                | 129 ms                                                 | 125 ms: 1.03x faster                                                             |
| sqlglot_parse              | 1.36 ms                                                | 1.32 ms: 1.03x faster                                                            |
| deepcopy                   | 371 us                                                 | 360 us: 1.03x faster                                                             |
| sympy_integrate            | 21.4 ms                                                | 20.9 ms: 1.03x faster                                                            |
| docutils                   | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| pathlib                    | 19.3 ms                                                | 18.9 ms: 1.02x faster                                                            |
| sqlglot_transpile          | 1.68 ms                                                | 1.65 ms: 1.02x faster                                                            |
| pickle_dict                | 35.5 us                                                | 34.9 us: 1.02x faster                                                            |
| xml_etree_parse            | 159 ms                                                 | 157 ms: 1.02x faster                                                             |
| xml_etree_process          | 61.7 ms                                                | 60.8 ms: 1.02x faster                                                            |
| async_generators           | 463 ms                                                 | 456 ms: 1.02x faster                                                             |
| async_tree_memoization     | 578 ms                                                 | 571 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 717 ms: 1.01x faster                                                             |
| chameleon                  | 7.41 ms                                                | 7.33 ms: 1.01x faster                                                            |
| json                       | 5.26 ms                                                | 5.20 ms: 1.01x faster                                                            |
| dask                       | 372 ms                                                 | 368 ms: 1.01x faster                                                             |
| xml_etree_generate         | 89.2 ms                                                | 88.5 ms: 1.01x faster                                                            |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                                            |
| create_gc_cycles           | 1.48 ms                                                | 1.47 ms: 1.01x faster                                                            |
| dulwich_log                | 68.5 ms                                                | 68.8 ms: 1.00x slower                                                            |
| pidigits                   | 187 ms                                                 | 188 ms: 1.00x slower                                                             |
| regex_compile              | 148 ms                                                 | 149 ms: 1.01x slower                                                             |
| unpickle_list              | 5.29 us                                                | 5.31 us: 1.01x slower                                                            |
| crypto_pyaes               | 81.9 ms                                                | 82.3 ms: 1.01x slower                                                            |
| gc_traversal               | 3.79 ms                                                | 3.82 ms: 1.01x slower                                                            |
| regex_effbot               | 3.61 ms                                                | 3.64 ms: 1.01x slower                                                            |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| scimark_lu                 | 118 ms                                                 | 119 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 734 ms: 1.01x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 455 ms: 1.01x slower                                                             |
| meteor_contest             | 112 ms                                                 | 114 ms: 1.01x slower                                                             |
| sqlite_synth               | 2.83 us                                                | 2.87 us: 1.01x slower                                                            |
| async_tree_io_tg           | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                           |
| sympy_expand               | 478 ms                                                 | 485 ms: 1.01x slower                                                             |
| unpickle_pure_python       | 230 us                                                 | 235 us: 1.02x slower                                                             |
| xml_etree_iterparse        | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| pickle_list                | 5.08 us                                                | 5.24 us: 1.03x slower                                                            |
| sqlglot_normalize          | 110 ms                                                 | 114 ms: 1.03x slower                                                             |
| float                      | 84.7 ms                                                | 87.8 ms: 1.04x slower                                                            |
| 2to3                       | 274 ms                                                 | 286 ms: 1.04x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 599 ms: 1.04x slower                                                             |
| pprint_safe_repr           | 776 ms                                                 | 811 ms: 1.05x slower                                                             |
| fannkuch                   | 417 ms                                                 | 437 ms: 1.05x slower                                                             |
| scimark_monte_carlo        | 75.1 ms                                                | 78.8 ms: 1.05x slower                                                            |
| richards                   | 45.8 ms                                                | 48.2 ms: 1.05x slower                                                            |
| chaos                      | 67.0 ms                                                | 70.5 ms: 1.05x slower                                                            |
| regex_dna                  | 212 ms                                                 | 223 ms: 1.05x slower                                                             |
| sqlglot_optimize           | 54.8 ms                                                | 57.8 ms: 1.05x slower                                                            |
| richards_super             | 51.5 ms                                                | 54.5 ms: 1.06x slower                                                            |
| mdp                        | 2.63 sec                                               | 2.79 sec: 1.06x slower                                                           |
| tomli_loads                | 2.33 sec                                               | 2.47 sec: 1.06x slower                                                           |
| pycparser                  | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                           |
| pprint_pformat             | 1.57 sec                                               | 1.67 sec: 1.06x slower                                                           |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| regex_v8                   | 23.1 ms                                                | 24.7 ms: 1.07x slower                                                            |
| pyflate                    | 482 ms                                                 | 516 ms: 1.07x slower                                                             |
| nqueens                    | 83.3 ms                                                | 90.5 ms: 1.09x slower                                                            |
| scimark_fft                | 382 ms                                                 | 419 ms: 1.10x slower                                                             |
| go                         | 139 ms                                                 | 153 ms: 1.10x slower                                                             |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.57 ms: 1.10x slower                                                            |
| mako                       | 11.9 ms                                                | 13.3 ms: 1.12x slower                                                            |
| nbody                      | 97.0 ms                                                | 110 ms: 1.13x slower                                                             |
| spectral_norm              | 115 ms                                                 | 136 ms: 1.18x slower                                                             |
| deltablue                  | 3.72 ms                                                | 4.42 ms: 1.19x slower                                                            |
| telco                      | 7.10 ms                                                | 8.71 ms: 1.23x slower                                                            |
| hexiom                     | 6.41 ms                                                | 7.97 ms: 1.24x slower                                                            |
| python_startup_no_site     | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                            |
| coverage                   | 72.7 ms                                                | 95.4 ms: 1.31x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (8): deepcopy_memo, bench_mp_pool, bench_thread_pool, asyncio_tcp_ssl, asyncio_websockets, logging_silent, json_loads, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.97% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x