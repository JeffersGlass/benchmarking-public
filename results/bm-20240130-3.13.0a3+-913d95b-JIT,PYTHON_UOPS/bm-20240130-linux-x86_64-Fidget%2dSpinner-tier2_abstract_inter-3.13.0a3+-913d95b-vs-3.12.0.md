
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.00x slower
- HPT reliability: 95.35%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 280 ms: 1.02x slower                                                             |
| chameleon      | 7.41 ms                                                | 6.96 ms: 1.07x faster                                                            |
| docutils       | 2.77 sec                                               | 2.68 sec: 1.03x faster                                                           |
| tornado_http   | 103 ms                                                 | 97.9 ms: 1.05x faster                                                            |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 442 ms: 1.07x faster                                                             |
| async_tree_memoization  | 578 ms                                                 | 570 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed | 726 ms                                                 | 717 ms: 1.01x faster                                                             |
| async_tree_none_tg      | 450 ms                                                 | 453 ms: 1.01x slower                                                             |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| async_tree_io           | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| Geometric mean          | (ref)                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 86.6 ms: 1.02x slower                                                            |
| nbody          | 97.0 ms                                                | 99.8 ms: 1.03x slower                                                            |
| Geometric mean | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 143 ms: 1.04x faster                                                             |
| regex_effbot   | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                            |
| regex_dna      | 212 ms                                                 | 222 ms: 1.05x slower                                                             |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 300 us: 1.08x faster                                                             |
| unpickle             | 15.9 us                                                | 14.7 us: 1.08x faster                                                            |
| tomli_loads          | 2.33 sec                                               | 2.22 sec: 1.05x faster                                                           |
| xml_etree_process    | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                            |
| xml_etree_generate   | 89.2 ms                                                | 87.7 ms: 1.02x faster                                                            |
| pickle_dict          | 35.5 us                                                | 35.0 us: 1.01x faster                                                            |
| unpickle_list        | 5.29 us                                                | 5.22 us: 1.01x faster                                                            |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| unpickle_pure_python | 230 us                                                 | 229 us: 1.00x faster                                                             |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (2): pickle, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.3 ms: 1.08x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.93 ms: 1.29x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.18x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.5 ms: 1.05x slower                                                            |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 111 us: 1.42x faster                                                             |
| unpack_sequence          | 54.0 ns                                                | 43.2 ns: 1.25x faster                                                            |
| logging_format           | 7.23 us                                                | 6.40 us: 1.13x faster                                                            |
| comprehensions           | 21.8 us                                                | 19.4 us: 1.12x faster                                                            |
| raytrace                 | 312 ms                                                 | 281 ms: 1.11x faster                                                             |
| logging_simple           | 6.46 us                                                | 5.86 us: 1.10x faster                                                            |
| deepcopy_reduce          | 3.35 us                                                | 3.08 us: 1.09x faster                                                            |
| pickle_pure_python       | 324 us                                                 | 300 us: 1.08x faster                                                             |
| unpickle                 | 15.9 us                                                | 14.7 us: 1.08x faster                                                            |
| async_tree_none          | 472 ms                                                 | 442 ms: 1.07x faster                                                             |
| chameleon                | 7.41 ms                                                | 6.96 ms: 1.07x faster                                                            |
| pathlib                  | 19.3 ms                                                | 18.2 ms: 1.07x faster                                                            |
| deepcopy                 | 371 us                                                 | 349 us: 1.06x faster                                                             |
| sqlglot_parse            | 1.36 ms                                                | 1.29 ms: 1.06x faster                                                            |
| tomli_loads              | 2.33 sec                                               | 2.22 sec: 1.05x faster                                                           |
| deepcopy_memo            | 40.7 us                                                | 38.8 us: 1.05x faster                                                            |
| generators               | 31.2 ms                                                | 29.7 ms: 1.05x faster                                                            |
| tornado_http             | 103 ms                                                 | 97.9 ms: 1.05x faster                                                            |
| sympy_sum                | 169 ms                                                 | 162 ms: 1.04x faster                                                             |
| scimark_lu               | 118 ms                                                 | 113 ms: 1.04x faster                                                             |
| xml_etree_process        | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                            |
| sqlglot_transpile        | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                            |
| regex_compile            | 148 ms                                                 | 143 ms: 1.04x faster                                                             |
| scimark_sor              | 129 ms                                                 | 125 ms: 1.04x faster                                                             |
| docutils                 | 2.77 sec                                               | 2.68 sec: 1.03x faster                                                           |
| sympy_str                | 300 ms                                                 | 291 ms: 1.03x faster                                                             |
| scimark_fft              | 382 ms                                                 | 372 ms: 1.03x faster                                                             |
| logging_silent           | 104 ns                                                 | 102 ns: 1.02x faster                                                             |
| dask                     | 372 ms                                                 | 366 ms: 1.02x faster                                                             |
| xml_etree_generate       | 89.2 ms                                                | 87.7 ms: 1.02x faster                                                            |
| json                     | 5.26 ms                                                | 5.19 ms: 1.01x faster                                                            |
| pickle_dict              | 35.5 us                                                | 35.0 us: 1.01x faster                                                            |
| async_tree_memoization   | 578 ms                                                 | 570 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 717 ms: 1.01x faster                                                             |
| unpickle_list            | 5.29 us                                                | 5.22 us: 1.01x faster                                                            |
| json_loads               | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| pycparser                | 1.18 sec                                               | 1.17 sec: 1.01x faster                                                           |
| xml_etree_parse          | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| sympy_integrate          | 21.4 ms                                                | 21.3 ms: 1.01x faster                                                            |
| unpickle_pure_python     | 230 us                                                 | 229 us: 1.00x faster                                                             |
| bench_thread_pool        | 842 us                                                 | 839 us: 1.00x faster                                                             |
| meteor_contest           | 112 ms                                                 | 112 ms: 1.00x faster                                                             |
| pidigits                 | 187 ms                                                 | 188 ms: 1.01x slower                                                             |
| sqlglot_normalize        | 110 ms                                                 | 111 ms: 1.01x slower                                                             |
| asyncio_websockets       | 551 ms                                                 | 555 ms: 1.01x slower                                                             |
| async_tree_none_tg       | 450 ms                                                 | 453 ms: 1.01x slower                                                             |
| asyncio_tcp              | 491 ms                                                 | 495 ms: 1.01x slower                                                             |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.81 sec: 1.01x slower                                                           |
| scimark_monte_carlo      | 75.1 ms                                                | 76.2 ms: 1.01x slower                                                            |
| sympy_expand             | 478 ms                                                 | 485 ms: 1.02x slower                                                             |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                            |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| richards                 | 45.8 ms                                                | 46.6 ms: 1.02x slower                                                            |
| regex_effbot             | 3.61 ms                                                | 3.67 ms: 1.02x slower                                                            |
| 2to3                     | 274 ms                                                 | 280 ms: 1.02x slower                                                             |
| gc_traversal             | 3.79 ms                                                | 3.87 ms: 1.02x slower                                                            |
| float                    | 84.7 ms                                                | 86.6 ms: 1.02x slower                                                            |
| pickle_list              | 5.08 us                                                | 5.20 us: 1.02x slower                                                            |
| xml_etree_iterparse      | 107 ms                                                 | 109 ms: 1.02x slower                                                             |
| richards_super           | 51.5 ms                                                | 52.9 ms: 1.03x slower                                                            |
| async_tree_io            | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| fannkuch                 | 417 ms                                                 | 428 ms: 1.03x slower                                                             |
| nbody                    | 97.0 ms                                                | 99.8 ms: 1.03x slower                                                            |
| sqlglot_optimize         | 54.8 ms                                                | 56.5 ms: 1.03x slower                                                            |
| chaos                    | 67.0 ms                                                | 69.5 ms: 1.04x slower                                                            |
| mdp                      | 2.63 sec                                               | 2.74 sec: 1.04x slower                                                           |
| pprint_safe_repr         | 776 ms                                                 | 809 ms: 1.04x slower                                                             |
| regex_dna                | 212 ms                                                 | 222 ms: 1.05x slower                                                             |
| mako                     | 11.9 ms                                                | 12.5 ms: 1.05x slower                                                            |
| pyflate                  | 482 ms                                                 | 515 ms: 1.07x slower                                                             |
| python_startup           | 9.55 ms                                                | 10.3 ms: 1.08x slower                                                            |
| deltablue                | 3.72 ms                                                | 4.01 ms: 1.08x slower                                                            |
| nqueens                  | 83.3 ms                                                | 90.0 ms: 1.08x slower                                                            |
| regex_v8                 | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                            |
| go                       | 139 ms                                                 | 152 ms: 1.09x slower                                                             |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.57 ms: 1.10x slower                                                            |
| pprint_pformat           | 1.57 sec                                               | 1.73 sec: 1.10x slower                                                           |
| spectral_norm            | 115 ms                                                 | 135 ms: 1.17x slower                                                             |
| telco                    | 7.10 ms                                                | 8.43 ms: 1.19x slower                                                            |
| python_startup_no_site   | 6.94 ms                                                | 8.93 ms: 1.29x slower                                                            |
| coverage                 | 72.7 ms                                                | 94.6 ms: 1.30x slower                                                            |
| hexiom                   | 6.41 ms                                                | 8.65 ms: 1.35x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (11): crypto_pyaes, sqlite_synth, async_tree_cpu_io_mixed_tg, coroutines, bench_mp_pool, dulwich_log, pickle, async_generators, json_dumps, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 95.35% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x