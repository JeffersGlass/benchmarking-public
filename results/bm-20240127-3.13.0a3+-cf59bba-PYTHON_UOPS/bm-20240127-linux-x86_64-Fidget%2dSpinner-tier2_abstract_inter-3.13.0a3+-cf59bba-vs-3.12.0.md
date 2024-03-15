
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.01x slower
- HPT reliability: 99.41%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 283 ms: 1.03x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.16 ms: 1.03x faster                                                            |
| docutils       | 2.77 sec                                               | 2.69 sec: 1.03x faster                                                           |
| tornado_http   | 103 ms                                                 | 98.5 ms: 1.04x faster                                                            |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 448 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                             |
| async_tree_none_tg        | 450 ms                                                 | 456 ms: 1.01x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| async_tree_memoization_tg | 575 ms                                                 | 590 ms: 1.03x slower                                                             |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                             |
| float          | 84.7 ms                                                | 87.7 ms: 1.04x slower                                                            |
| nbody          | 97.0 ms                                                | 113 ms: 1.16x slower                                                             |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.56 ms: 1.01x faster                                                            |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 297 us: 1.09x faster                                                             |
| unpickle_list        | 5.29 us                                                | 4.94 us: 1.07x faster                                                            |
| unpickle             | 15.9 us                                                | 15.0 us: 1.06x faster                                                            |
| pickle_dict          | 35.5 us                                                | 34.8 us: 1.02x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 60.5 ms: 1.02x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.02x faster                                                             |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                                            |
| unpickle_pure_python | 230 us                                                 | 234 us: 1.02x slower                                                             |
| xml_etree_iterparse  | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| pickle_list          | 5.08 us                                                | 5.23 us: 1.03x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (4): tomli_loads, json_dumps, xml_etree_generate, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.79 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.9 ms: 1.09x slower                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 116 us: 1.36x faster                                                             |
| unpack_sequence           | 54.0 ns                                                | 40.7 ns: 1.32x faster                                                            |
| pickle_pure_python        | 324 us                                                 | 297 us: 1.09x faster                                                             |
| unpickle_list             | 5.29 us                                                | 4.94 us: 1.07x faster                                                            |
| logging_format            | 7.23 us                                                | 6.76 us: 1.07x faster                                                            |
| logging_simple            | 6.46 us                                                | 6.06 us: 1.07x faster                                                            |
| raytrace                  | 312 ms                                                 | 294 ms: 1.06x faster                                                             |
| sympy_sum                 | 169 ms                                                 | 159 ms: 1.06x faster                                                             |
| comprehensions            | 21.8 us                                                | 20.6 us: 1.06x faster                                                            |
| unpickle                  | 15.9 us                                                | 15.0 us: 1.06x faster                                                            |
| async_tree_none           | 472 ms                                                 | 448 ms: 1.05x faster                                                             |
| generators                | 31.2 ms                                                | 29.8 ms: 1.05x faster                                                            |
| deepcopy_reduce           | 3.35 us                                                | 3.19 us: 1.05x faster                                                            |
| tornado_http              | 103 ms                                                 | 98.5 ms: 1.04x faster                                                            |
| pathlib                   | 19.3 ms                                                | 18.6 ms: 1.04x faster                                                            |
| chameleon                 | 7.41 ms                                                | 7.16 ms: 1.03x faster                                                            |
| sympy_str                 | 300 ms                                                 | 290 ms: 1.03x faster                                                             |
| sqlglot_parse             | 1.36 ms                                                | 1.32 ms: 1.03x faster                                                            |
| docutils                  | 2.77 sec                                               | 2.69 sec: 1.03x faster                                                           |
| deepcopy                  | 371 us                                                 | 361 us: 1.03x faster                                                             |
| coroutines                | 23.2 ms                                                | 22.7 ms: 1.02x faster                                                            |
| pickle_dict               | 35.5 us                                                | 34.8 us: 1.02x faster                                                            |
| xml_etree_process         | 61.7 ms                                                | 60.5 ms: 1.02x faster                                                            |
| gc_traversal              | 3.79 ms                                                | 3.72 ms: 1.02x faster                                                            |
| sqlglot_transpile         | 1.68 ms                                                | 1.65 ms: 1.02x faster                                                            |
| sympy_integrate           | 21.4 ms                                                | 21.1 ms: 1.02x faster                                                            |
| json                      | 5.26 ms                                                | 5.17 ms: 1.02x faster                                                            |
| xml_etree_parse           | 159 ms                                                 | 157 ms: 1.02x faster                                                             |
| async_generators          | 463 ms                                                 | 456 ms: 1.02x faster                                                             |
| regex_effbot              | 3.61 ms                                                | 3.56 ms: 1.01x faster                                                            |
| scimark_sor               | 129 ms                                                 | 128 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 717 ms: 1.01x faster                                                             |
| dask                      | 372 ms                                                 | 368 ms: 1.01x faster                                                             |
| logging_silent            | 104 ns                                                 | 104 ns: 1.01x faster                                                             |
| mdp                       | 2.63 sec                                               | 2.61 sec: 1.01x faster                                                           |
| json_loads                | 28.5 us                                                | 28.3 us: 1.01x faster                                                            |
| asyncio_tcp               | 491 ms                                                 | 488 ms: 1.01x faster                                                             |
| pidigits                  | 187 ms                                                 | 188 ms: 1.00x slower                                                             |
| crypto_pyaes              | 81.9 ms                                                | 82.2 ms: 1.00x slower                                                            |
| dulwich_log               | 68.5 ms                                                | 68.8 ms: 1.00x slower                                                            |
| deepcopy_memo             | 40.7 us                                                | 40.9 us: 1.01x slower                                                            |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| async_tree_none_tg        | 450 ms                                                 | 456 ms: 1.01x slower                                                             |
| meteor_contest            | 112 ms                                                 | 114 ms: 1.01x slower                                                             |
| scimark_lu                | 118 ms                                                 | 120 ms: 1.02x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| unpickle_pure_python      | 230 us                                                 | 234 us: 1.02x slower                                                             |
| sqlite_synth              | 2.83 us                                                | 2.88 us: 1.02x slower                                                            |
| sympy_expand              | 478 ms                                                 | 487 ms: 1.02x slower                                                             |
| pycparser                 | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| sqlglot_normalize         | 110 ms                                                 | 113 ms: 1.03x slower                                                             |
| async_tree_memoization_tg | 575 ms                                                 | 590 ms: 1.03x slower                                                             |
| xml_etree_iterparse       | 107 ms                                                 | 110 ms: 1.03x slower                                                             |
| pickle_list               | 5.08 us                                                | 5.23 us: 1.03x slower                                                            |
| fannkuch                  | 417 ms                                                 | 429 ms: 1.03x slower                                                             |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| 2to3                      | 274 ms                                                 | 283 ms: 1.03x slower                                                             |
| scimark_monte_carlo       | 75.1 ms                                                | 77.5 ms: 1.03x slower                                                            |
| float                     | 84.7 ms                                                | 87.7 ms: 1.04x slower                                                            |
| pprint_safe_repr          | 776 ms                                                 | 806 ms: 1.04x slower                                                             |
| regex_dna                 | 212 ms                                                 | 222 ms: 1.05x slower                                                             |
| chaos                     | 67.0 ms                                                | 70.2 ms: 1.05x slower                                                            |
| sqlglot_optimize          | 54.8 ms                                                | 57.6 ms: 1.05x slower                                                            |
| pyflate                   | 482 ms                                                 | 508 ms: 1.05x slower                                                             |
| pprint_pformat            | 1.57 sec                                               | 1.66 sec: 1.06x slower                                                           |
| python_startup            | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| richards                  | 45.8 ms                                                | 48.9 ms: 1.07x slower                                                            |
| richards_super            | 51.5 ms                                                | 55.3 ms: 1.07x slower                                                            |
| regex_v8                  | 23.1 ms                                                | 24.9 ms: 1.08x slower                                                            |
| scimark_fft               | 382 ms                                                 | 414 ms: 1.08x slower                                                             |
| mako                      | 11.9 ms                                                | 12.9 ms: 1.09x slower                                                            |
| scimark_sparse_mat_mult   | 5.06 ms                                                | 5.50 ms: 1.09x slower                                                            |
| nqueens                   | 83.3 ms                                                | 92.2 ms: 1.11x slower                                                            |
| go                        | 139 ms                                                 | 155 ms: 1.11x slower                                                             |
| spectral_norm             | 115 ms                                                 | 132 ms: 1.15x slower                                                             |
| nbody                     | 97.0 ms                                                | 113 ms: 1.16x slower                                                             |
| deltablue                 | 3.72 ms                                                | 4.41 ms: 1.19x slower                                                            |
| telco                     | 7.10 ms                                                | 8.62 ms: 1.21x slower                                                            |
| hexiom                    | 6.41 ms                                                | 8.01 ms: 1.25x slower                                                            |
| python_startup_no_site    | 6.94 ms                                                | 8.79 ms: 1.27x slower                                                            |
| coverage                  | 72.7 ms                                                | 93.5 ms: 1.29x slower                                                            |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (12): async_tree_memoization, tomli_loads, regex_compile, json_dumps, xml_etree_generate, bench_mp_pool, bench_thread_pool, create_gc_cycles, asyncio_websockets, pickle, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.41% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.95x