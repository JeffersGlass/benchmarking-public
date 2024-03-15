# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_superinstructi
- machine: linux-x86_64
- commit hash: c04ea6c
- commit date: 2024-03-01
- overall geometric mean: 1.01x slower \*
- HPT reliability: 70.45%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 280 ms: 1.02x slower                                                             |
| chameleon      | 7.41 ms                                                | 6.99 ms: 1.06x faster                                                            |
| docutils       | 2.77 sec                                               | 2.74 sec: 1.01x faster                                                           |
| tornado_http   | 103 ms                                                 | 96.3 ms: 1.07x faster                                                            |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none           | 472 ms                                                 | 439 ms: 1.08x faster                                                             |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 708 ms: 1.02x faster                                                             |
| async_tree_memoization    | 578 ms                                                 | 567 ms: 1.02x faster                                                             |
| async_tree_none_tg        | 450 ms                                                 | 452 ms: 1.00x slower                                                             |
| async_tree_memoization_tg | 575 ms                                                 | 585 ms: 1.02x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| Geometric mean            | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 82.7 ms: 1.02x faster                                                            |
| nbody          | 97.0 ms                                                | 96.2 ms: 1.01x faster                                                            |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                             |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 153 ms: 1.03x slower                                                             |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                            |
| regex_dna      | 212 ms                                                 | 232 ms: 1.10x slower                                                             |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                             |
| tomli_loads          | 2.33 sec                                               | 2.16 sec: 1.08x faster                                                           |
| unpickle_list        | 5.29 us                                                | 4.93 us: 1.07x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 58.7 ms: 1.05x faster                                                            |
| json_loads           | 28.5 us                                                | 27.3 us: 1.05x faster                                                            |
| pickle_dict          | 35.5 us                                                | 34.1 us: 1.04x faster                                                            |
| xml_etree_generate   | 89.2 ms                                                | 86.8 ms: 1.03x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                             |
| pickle_list          | 5.08 us                                                | 4.97 us: 1.02x faster                                                            |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                            |
| pickle               | 11.6 us                                                | 11.7 us: 1.00x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 245 us: 1.06x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                                     |

Benchmark hidden because not significant (2): xml_etree_iterparse, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.3 ms: 1.28x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.42x slower                                                                     |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                 | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 158 us                                                 | 110 us: 1.44x faster                                                             |
| comprehensions            | 21.8 us                                                | 18.6 us: 1.17x faster                                                            |
| raytrace                  | 312 ms                                                 | 276 ms: 1.13x faster                                                             |
| logging_format            | 7.23 us                                                | 6.41 us: 1.13x faster                                                            |
| logging_simple            | 6.46 us                                                | 5.86 us: 1.10x faster                                                            |
| crypto_pyaes              | 81.9 ms                                                | 74.7 ms: 1.10x faster                                                            |
| pickle_pure_python        | 324 us                                                 | 299 us: 1.08x faster                                                             |
| scimark_fft               | 382 ms                                                 | 354 ms: 1.08x faster                                                             |
| tomli_loads               | 2.33 sec                                               | 2.16 sec: 1.08x faster                                                           |
| async_tree_none           | 472 ms                                                 | 439 ms: 1.08x faster                                                             |
| unpickle_list             | 5.29 us                                                | 4.93 us: 1.07x faster                                                            |
| deepcopy_reduce           | 3.35 us                                                | 3.12 us: 1.07x faster                                                            |
| deltablue                 | 3.72 ms                                                | 3.46 ms: 1.07x faster                                                            |
| deepcopy                  | 371 us                                                 | 347 us: 1.07x faster                                                             |
| generators                | 31.2 ms                                                | 29.3 ms: 1.07x faster                                                            |
| tornado_http              | 103 ms                                                 | 96.3 ms: 1.07x faster                                                            |
| chameleon                 | 7.41 ms                                                | 6.99 ms: 1.06x faster                                                            |
| sympy_sum                 | 169 ms                                                 | 161 ms: 1.05x faster                                                             |
| xml_etree_process         | 61.7 ms                                                | 58.7 ms: 1.05x faster                                                            |
| coroutines                | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                            |
| sympy_str                 | 300 ms                                                 | 286 ms: 1.05x faster                                                             |
| json_loads                | 28.5 us                                                | 27.3 us: 1.05x faster                                                            |
| deepcopy_memo             | 40.7 us                                                | 39.0 us: 1.04x faster                                                            |
| pickle_dict               | 35.5 us                                                | 34.1 us: 1.04x faster                                                            |
| pathlib                   | 19.3 ms                                                | 18.6 ms: 1.04x faster                                                            |
| logging_silent            | 104 ns                                                 | 101 ns: 1.04x faster                                                             |
| meteor_contest            | 112 ms                                                 | 108 ms: 1.04x faster                                                             |
| sqlglot_parse             | 1.36 ms                                                | 1.31 ms: 1.04x faster                                                            |
| chaos                     | 67.0 ms                                                | 64.8 ms: 1.03x faster                                                            |
| json                      | 5.26 ms                                                | 5.10 ms: 1.03x faster                                                            |
| xml_etree_generate        | 89.2 ms                                                | 86.8 ms: 1.03x faster                                                            |
| async_tree_cpu_io_mixed   | 726 ms                                                 | 708 ms: 1.02x faster                                                             |
| float                     | 84.7 ms                                                | 82.7 ms: 1.02x faster                                                            |
| xml_etree_parse           | 159 ms                                                 | 156 ms: 1.02x faster                                                             |
| sqlglot_transpile         | 1.68 ms                                                | 1.65 ms: 1.02x faster                                                            |
| pickle_list               | 5.08 us                                                | 4.97 us: 1.02x faster                                                            |
| gc_traversal              | 3.79 ms                                                | 3.72 ms: 1.02x faster                                                            |
| async_tree_memoization    | 578 ms                                                 | 567 ms: 1.02x faster                                                             |
| docutils                  | 2.77 sec                                               | 2.74 sec: 1.01x faster                                                           |
| sqlglot_normalize         | 110 ms                                                 | 109 ms: 1.01x faster                                                             |
| nbody                     | 97.0 ms                                                | 96.2 ms: 1.01x faster                                                            |
| sqlite_synth              | 2.83 us                                                | 2.81 us: 1.01x faster                                                            |
| json_dumps                | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                            |
| pidigits                  | 187 ms                                                 | 187 ms: 1.00x faster                                                             |
| asyncio_tcp               | 491 ms                                                 | 492 ms: 1.00x slower                                                             |
| sympy_integrate           | 21.4 ms                                                | 21.5 ms: 1.00x slower                                                            |
| pickle                    | 11.6 us                                                | 11.7 us: 1.00x slower                                                            |
| async_tree_none_tg        | 450 ms                                                 | 452 ms: 1.00x slower                                                             |
| bench_thread_pool         | 842 us                                                 | 849 us: 1.01x slower                                                             |
| asyncio_tcp_ssl           | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| mdp                       | 2.63 sec                                               | 2.66 sec: 1.01x slower                                                           |
| dulwich_log               | 68.5 ms                                                | 69.3 ms: 1.01x slower                                                            |
| scimark_monte_carlo       | 75.1 ms                                                | 76.2 ms: 1.01x slower                                                            |
| sympy_expand              | 478 ms                                                 | 485 ms: 1.01x slower                                                             |
| create_gc_cycles          | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                            |
| async_tree_memoization_tg | 575 ms                                                 | 585 ms: 1.02x slower                                                             |
| 2to3                      | 274 ms                                                 | 280 ms: 1.02x slower                                                             |
| async_tree_io_tg          | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| pycparser                 | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                           |
| async_tree_io             | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| regex_compile             | 148 ms                                                 | 153 ms: 1.03x slower                                                             |
| sqlglot_optimize          | 54.8 ms                                                | 56.7 ms: 1.04x slower                                                            |
| spectral_norm             | 115 ms                                                 | 120 ms: 1.04x slower                                                             |
| pyflate                   | 482 ms                                                 | 509 ms: 1.06x slower                                                             |
| unpickle_pure_python      | 230 us                                                 | 245 us: 1.06x slower                                                             |
| pprint_safe_repr          | 776 ms                                                 | 831 ms: 1.07x slower                                                             |
| richards_super            | 51.5 ms                                                | 56.0 ms: 1.09x slower                                                            |
| regex_v8                  | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                            |
| richards                  | 45.8 ms                                                | 50.1 ms: 1.09x slower                                                            |
| pprint_pformat            | 1.57 sec                                               | 1.72 sec: 1.09x slower                                                           |
| regex_dna                 | 212 ms                                                 | 232 ms: 1.10x slower                                                             |
| nqueens                   | 83.3 ms                                                | 91.4 ms: 1.10x slower                                                            |
| scimark_lu                | 118 ms                                                 | 131 ms: 1.11x slower                                                             |
| go                        | 139 ms                                                 | 156 ms: 1.12x slower                                                             |
| bench_mp_pool             | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                            |
| hexiom                    | 6.41 ms                                                | 7.74 ms: 1.21x slower                                                            |
| telco                     | 7.10 ms                                                | 8.59 ms: 1.21x slower                                                            |
| python_startup            | 9.55 ms                                                | 12.3 ms: 1.28x slower                                                            |
| coverage                  | 72.7 ms                                                | 96.3 ms: 1.32x slower                                                            |
| python_startup_no_site    | 6.94 ms                                                | 10.9 ms: 1.57x slower                                                            |
| unpack_sequence           | 54.0 ns                                                | 126 ns: 2.34x slower                                                             |
| Geometric mean            | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (11): async_tree_cpu_io_mixed_tg, xml_etree_iterparse, mako, async_generators, regex_effbot, asyncio_websockets, fannkuch, scimark_sparse_mat_mult, scimark_sor, unpickle, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 70.45% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.17x