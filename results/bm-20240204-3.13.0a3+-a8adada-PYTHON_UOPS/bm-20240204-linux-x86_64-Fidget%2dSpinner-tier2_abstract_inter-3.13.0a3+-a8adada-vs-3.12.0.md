
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: a8adada
- commit date: 2024-02-04
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.98%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 282 ms: 1.03x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.27 ms: 1.02x faster                                                            |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| tornado_http   | 103 ms                                                 | 98.4 ms: 1.04x faster                                                            |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 452 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 737 ms: 1.02x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 603 ms: 1.05x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                             |
| float          | 84.7 ms                                                | 92.0 ms: 1.09x slower                                                            |
| nbody          | 97.0 ms                                                | 119 ms: 1.23x slower                                                             |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.66 ms: 1.01x slower                                                            |
| regex_dna      | 212 ms                                                 | 221 ms: 1.04x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.2 ms: 1.05x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                             |
| unpickle_list        | 5.29 us                                                | 4.96 us: 1.07x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 60.4 ms: 1.02x faster                                                            |
| pickle_dict          | 35.5 us                                                | 35.1 us: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| xml_etree_generate   | 89.2 ms                                                | 88.9 ms: 1.00x faster                                                            |
| json_loads           | 28.5 us                                                | 28.7 us: 1.01x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.12 us: 1.01x slower                                                            |
| tomli_loads          | 2.33 sec                                               | 2.35 sec: 1.01x slower                                                           |
| unpickle_pure_python | 230 us                                                 | 234 us: 1.02x slower                                                             |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.03x slower                                                             |
| unpickle             | 15.9 us                                                | 16.5 us: 1.04x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.6 ms: 1.14x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 114 us: 1.38x faster                                                             |
| unpack_sequence            | 54.0 ns                                                | 39.2 ns: 1.38x faster                                                            |
| logging_simple             | 6.46 us                                                | 5.85 us: 1.10x faster                                                            |
| logging_format             | 7.23 us                                                | 6.67 us: 1.08x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 299 us: 1.08x faster                                                             |
| unpickle_list              | 5.29 us                                                | 4.96 us: 1.07x faster                                                            |
| comprehensions             | 21.8 us                                                | 20.5 us: 1.06x faster                                                            |
| coroutines                 | 23.2 ms                                                | 21.9 ms: 1.06x faster                                                            |
| deepcopy_reduce            | 3.35 us                                                | 3.16 us: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                             |
| deltablue                  | 3.72 ms                                                | 3.52 ms: 1.06x faster                                                            |
| raytrace                   | 312 ms                                                 | 296 ms: 1.05x faster                                                             |
| logging_silent             | 104 ns                                                 | 99.1 ns: 1.05x faster                                                            |
| generators                 | 31.2 ms                                                | 29.6 ms: 1.05x faster                                                            |
| scimark_sor                | 129 ms                                                 | 123 ms: 1.05x faster                                                             |
| async_tree_none            | 472 ms                                                 | 452 ms: 1.04x faster                                                             |
| tornado_http               | 103 ms                                                 | 98.4 ms: 1.04x faster                                                            |
| sympy_str                  | 300 ms                                                 | 289 ms: 1.04x faster                                                             |
| pathlib                    | 19.3 ms                                                | 18.7 ms: 1.04x faster                                                            |
| sympy_integrate            | 21.4 ms                                                | 20.7 ms: 1.04x faster                                                            |
| deepcopy                   | 371 us                                                 | 359 us: 1.03x faster                                                             |
| docutils                   | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.03x faster                                                            |
| xml_etree_process          | 61.7 ms                                                | 60.4 ms: 1.02x faster                                                            |
| chameleon                  | 7.41 ms                                                | 7.27 ms: 1.02x faster                                                            |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.02x faster                                                            |
| async_generators           | 463 ms                                                 | 456 ms: 1.01x faster                                                             |
| deepcopy_memo              | 40.7 us                                                | 40.2 us: 1.01x faster                                                            |
| pickle_dict                | 35.5 us                                                | 35.1 us: 1.01x faster                                                            |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| scimark_lu                 | 118 ms                                                 | 117 ms: 1.01x faster                                                             |
| xml_etree_generate         | 89.2 ms                                                | 88.9 ms: 1.00x faster                                                            |
| dulwich_log                | 68.5 ms                                                | 68.6 ms: 1.00x slower                                                            |
| pidigits                   | 187 ms                                                 | 188 ms: 1.00x slower                                                             |
| sqlite_synth               | 2.83 us                                                | 2.85 us: 1.01x slower                                                            |
| json_loads                 | 28.5 us                                                | 28.7 us: 1.01x slower                                                            |
| pickle_list                | 5.08 us                                                | 5.12 us: 1.01x slower                                                            |
| create_gc_cycles           | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                            |
| tomli_loads                | 2.33 sec                                               | 2.35 sec: 1.01x slower                                                           |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| asyncio_tcp                | 491 ms                                                 | 496 ms: 1.01x slower                                                             |
| regex_effbot               | 3.61 ms                                                | 3.66 ms: 1.01x slower                                                            |
| meteor_contest             | 112 ms                                                 | 114 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 737 ms: 1.02x slower                                                             |
| sympy_expand               | 478 ms                                                 | 486 ms: 1.02x slower                                                             |
| unpickle_pure_python       | 230 us                                                 | 234 us: 1.02x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 459 ms: 1.02x slower                                                             |
| pycparser                  | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                            |
| xml_etree_iterparse        | 107 ms                                                 | 109 ms: 1.03x slower                                                             |
| crypto_pyaes               | 81.9 ms                                                | 84.0 ms: 1.03x slower                                                            |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                           |
| 2to3                       | 274 ms                                                 | 282 ms: 1.03x slower                                                             |
| pprint_safe_repr           | 776 ms                                                 | 799 ms: 1.03x slower                                                             |
| sqlglot_normalize          | 110 ms                                                 | 114 ms: 1.03x slower                                                             |
| gc_traversal               | 3.79 ms                                                | 3.93 ms: 1.04x slower                                                            |
| unpickle                   | 15.9 us                                                | 16.5 us: 1.04x slower                                                            |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| richards_super             | 51.5 ms                                                | 53.7 ms: 1.04x slower                                                            |
| regex_dna                  | 212 ms                                                 | 221 ms: 1.04x slower                                                             |
| sqlglot_optimize           | 54.8 ms                                                | 57.4 ms: 1.05x slower                                                            |
| richards                   | 45.8 ms                                                | 48.0 ms: 1.05x slower                                                            |
| regex_v8                   | 23.1 ms                                                | 24.2 ms: 1.05x slower                                                            |
| async_tree_memoization_tg  | 575 ms                                                 | 603 ms: 1.05x slower                                                             |
| pyflate                    | 482 ms                                                 | 509 ms: 1.05x slower                                                             |
| pprint_pformat             | 1.57 sec                                               | 1.67 sec: 1.06x slower                                                           |
| scimark_monte_carlo        | 75.1 ms                                                | 79.8 ms: 1.06x slower                                                            |
| mdp                        | 2.63 sec                                               | 2.80 sec: 1.06x slower                                                           |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| chaos                      | 67.0 ms                                                | 71.6 ms: 1.07x slower                                                            |
| fannkuch                   | 417 ms                                                 | 448 ms: 1.07x slower                                                             |
| float                      | 84.7 ms                                                | 92.0 ms: 1.09x slower                                                            |
| scimark_fft                | 382 ms                                                 | 416 ms: 1.09x slower                                                             |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.63 ms: 1.11x slower                                                            |
| nqueens                    | 83.3 ms                                                | 92.8 ms: 1.11x slower                                                            |
| mako                       | 11.9 ms                                                | 13.6 ms: 1.14x slower                                                            |
| spectral_norm              | 115 ms                                                 | 135 ms: 1.18x slower                                                             |
| nbody                      | 97.0 ms                                                | 119 ms: 1.23x slower                                                             |
| telco                      | 7.10 ms                                                | 8.75 ms: 1.23x slower                                                            |
| go                         | 139 ms                                                 | 177 ms: 1.27x slower                                                             |
| python_startup_no_site     | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                            |
| hexiom                     | 6.41 ms                                                | 8.34 ms: 1.30x slower                                                            |
| coverage                   | 72.7 ms                                                | 95.1 ms: 1.31x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (10): dask, pickle, json, bench_mp_pool, asyncio_websockets, async_tree_memoization, bench_thread_pool, async_tree_cpu_io_mixed, regex_compile, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.98% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.94x