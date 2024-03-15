
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 289 ms: 1.05x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.52 ms: 1.02x slower                                                            |
| docutils       | 2.77 sec                                               | 2.74 sec: 1.01x faster                                                           |
| tornado_http   | 103 ms                                                 | 101 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 450 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 734 ms: 1.01x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 462 ms: 1.03x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 609 ms: 1.06x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 101 ms: 1.19x slower                                                             |
| nbody          | 97.0 ms                                                | 135 ms: 1.40x slower                                                             |
| Geometric mean | (ref)                                                  | 1.19x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.54 ms: 1.02x faster                                                            |
| regex_dna      | 212 ms                                                 | 220 ms: 1.04x slower                                                             |
| regex_compile  | 148 ms                                                 | 156 ms: 1.05x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.5 ms: 1.06x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 300 us: 1.08x faster                                                             |
| unpickle             | 15.9 us                                                | 15.1 us: 1.05x faster                                                            |
| unpickle_list        | 5.29 us                                                | 5.06 us: 1.05x faster                                                            |
| pickle_dict          | 35.5 us                                                | 34.2 us: 1.04x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 61.5 ms: 1.00x faster                                                            |
| xml_etree_generate   | 89.2 ms                                                | 90.0 ms: 1.01x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.15 us: 1.01x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 240 us: 1.04x slower                                                             |
| xml_etree_iterparse  | 107 ms                                                 | 115 ms: 1.08x slower                                                             |
| tomli_loads          | 2.33 sec                                               | 2.74 sec: 1.17x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 14.8 ms: 1.24x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 121 us: 1.31x faster                                                             |
| unpack_sequence            | 54.0 ns                                                | 47.8 ns: 1.13x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 300 us: 1.08x faster                                                             |
| deepcopy_reduce            | 3.35 us                                                | 3.13 us: 1.07x faster                                                            |
| logging_simple             | 6.46 us                                                | 6.08 us: 1.06x faster                                                            |
| logging_format             | 7.23 us                                                | 6.87 us: 1.05x faster                                                            |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                            |
| async_tree_none            | 472 ms                                                 | 450 ms: 1.05x faster                                                             |
| unpickle                   | 15.9 us                                                | 15.1 us: 1.05x faster                                                            |
| unpickle_list              | 5.29 us                                                | 5.06 us: 1.05x faster                                                            |
| generators                 | 31.2 ms                                                | 29.9 ms: 1.04x faster                                                            |
| gc_traversal               | 3.79 ms                                                | 3.65 ms: 1.04x faster                                                            |
| deepcopy                   | 371 us                                                 | 357 us: 1.04x faster                                                             |
| pickle_dict                | 35.5 us                                                | 34.2 us: 1.04x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 164 ms: 1.03x faster                                                             |
| regex_effbot               | 3.61 ms                                                | 3.54 ms: 1.02x faster                                                            |
| json                       | 5.26 ms                                                | 5.18 ms: 1.02x faster                                                            |
| docutils                   | 2.77 sec                                               | 2.74 sec: 1.01x faster                                                           |
| tornado_http               | 103 ms                                                 | 101 ms: 1.01x faster                                                             |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| async_generators           | 463 ms                                                 | 460 ms: 1.01x faster                                                             |
| sqlglot_parse              | 1.36 ms                                                | 1.35 ms: 1.01x faster                                                            |
| create_gc_cycles           | 1.48 ms                                                | 1.47 ms: 1.00x faster                                                            |
| xml_etree_process          | 61.7 ms                                                | 61.5 ms: 1.00x faster                                                            |
| deepcopy_memo              | 40.7 us                                                | 41.0 us: 1.01x slower                                                            |
| sympy_integrate            | 21.4 ms                                                | 21.6 ms: 1.01x slower                                                            |
| scimark_sor                | 129 ms                                                 | 130 ms: 1.01x slower                                                             |
| xml_etree_generate         | 89.2 ms                                                | 90.0 ms: 1.01x slower                                                            |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| dulwich_log                | 68.5 ms                                                | 69.2 ms: 1.01x slower                                                            |
| sympy_str                  | 300 ms                                                 | 303 ms: 1.01x slower                                                             |
| logging_silent             | 104 ns                                                 | 106 ns: 1.01x slower                                                             |
| mdp                        | 2.63 sec                                               | 2.66 sec: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 734 ms: 1.01x slower                                                             |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| pickle_list                | 5.08 us                                                | 5.15 us: 1.01x slower                                                            |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.81 sec: 1.01x slower                                                           |
| chameleon                  | 7.41 ms                                                | 7.52 ms: 1.02x slower                                                            |
| bench_thread_pool          | 842 us                                                 | 855 us: 1.02x slower                                                             |
| asyncio_tcp                | 491 ms                                                 | 500 ms: 1.02x slower                                                             |
| scimark_lu                 | 118 ms                                                 | 121 ms: 1.02x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 462 ms: 1.03x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                           |
| sqlite_synth               | 2.83 us                                                | 2.92 us: 1.03x slower                                                            |
| regex_dna                  | 212 ms                                                 | 220 ms: 1.04x slower                                                             |
| async_tree_io              | 1.16 sec                                               | 1.20 sec: 1.04x slower                                                           |
| unpickle_pure_python       | 230 us                                                 | 240 us: 1.04x slower                                                             |
| sqlglot_normalize          | 110 ms                                                 | 116 ms: 1.05x slower                                                             |
| meteor_contest             | 112 ms                                                 | 118 ms: 1.05x slower                                                             |
| 2to3                       | 274 ms                                                 | 289 ms: 1.05x slower                                                             |
| regex_compile              | 148 ms                                                 | 156 ms: 1.05x slower                                                             |
| sympy_expand               | 478 ms                                                 | 504 ms: 1.05x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 609 ms: 1.06x slower                                                             |
| regex_v8                   | 23.1 ms                                                | 24.5 ms: 1.06x slower                                                            |
| comprehensions             | 21.8 us                                                | 23.1 us: 1.06x slower                                                            |
| pycparser                  | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                           |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| sqlglot_optimize           | 54.8 ms                                                | 59.0 ms: 1.08x slower                                                            |
| xml_etree_iterparse        | 107 ms                                                 | 115 ms: 1.08x slower                                                             |
| pprint_safe_repr           | 776 ms                                                 | 842 ms: 1.09x slower                                                             |
| crypto_pyaes               | 81.9 ms                                                | 90.4 ms: 1.10x slower                                                            |
| richards                   | 45.8 ms                                                | 50.6 ms: 1.10x slower                                                            |
| richards_super             | 51.5 ms                                                | 57.0 ms: 1.11x slower                                                            |
| pprint_pformat             | 1.57 sec                                               | 1.75 sec: 1.12x slower                                                           |
| pyflate                    | 482 ms                                                 | 540 ms: 1.12x slower                                                             |
| fannkuch                   | 417 ms                                                 | 468 ms: 1.12x slower                                                             |
| go                         | 139 ms                                                 | 160 ms: 1.15x slower                                                             |
| chaos                      | 67.0 ms                                                | 76.8 ms: 1.15x slower                                                            |
| scimark_monte_carlo        | 75.1 ms                                                | 86.3 ms: 1.15x slower                                                            |
| tomli_loads                | 2.33 sec                                               | 2.74 sec: 1.17x slower                                                           |
| nqueens                    | 83.3 ms                                                | 98.6 ms: 1.18x slower                                                            |
| float                      | 84.7 ms                                                | 101 ms: 1.19x slower                                                             |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.06 ms: 1.20x slower                                                            |
| scimark_fft                | 382 ms                                                 | 459 ms: 1.20x slower                                                             |
| telco                      | 7.10 ms                                                | 8.66 ms: 1.22x slower                                                            |
| mako                       | 11.9 ms                                                | 14.8 ms: 1.24x slower                                                            |
| spectral_norm              | 115 ms                                                 | 145 ms: 1.27x slower                                                             |
| python_startup_no_site     | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                            |
| coverage                   | 72.7 ms                                                | 95.1 ms: 1.31x slower                                                            |
| deltablue                  | 3.72 ms                                                | 5.18 ms: 1.39x slower                                                            |
| nbody                      | 97.0 ms                                                | 135 ms: 1.40x slower                                                             |
| hexiom                     | 6.41 ms                                                | 9.23 ms: 1.44x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                                     |

Benchmark hidden because not significant (10): coroutines, dask, async_tree_cpu_io_mixed, bench_mp_pool, raytrace, sqlglot_transpile, asyncio_websockets, pickle, async_tree_memoization, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.94x