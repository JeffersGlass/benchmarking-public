
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 7de4b37
- commit date: 2024-01-26
- overall geometric mean: 1.03x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 285 ms: 1.04x slower                                                             |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.02x faster                                                           |
| tornado_http   | 103 ms                                                 | 98.8 ms: 1.04x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 451 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 739 ms: 1.02x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 460 ms: 1.02x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 594 ms: 1.03x slower                                                             |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 92.9 ms: 1.10x slower                                                            |
| nbody          | 97.0 ms                                                | 125 ms: 1.29x slower                                                             |
| Geometric mean | (ref)                                                  | 1.13x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.66 ms: 1.01x slower                                                            |
| regex_compile  | 148 ms                                                 | 152 ms: 1.03x slower                                                             |
| regex_dna      | 212 ms                                                 | 228 ms: 1.08x slower                                                             |
| regex_v8       | 23.1 ms                                                | 25.9 ms: 1.12x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 303 us: 1.07x faster                                                             |
| unpickle             | 15.9 us                                                | 15.2 us: 1.04x faster                                                            |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| pickle_dict          | 35.5 us                                                | 35.2 us: 1.01x faster                                                            |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 159 ms: 1.01x faster                                                             |
| xml_etree_process    | 61.7 ms                                                | 61.4 ms: 1.01x faster                                                            |
| xml_etree_generate   | 89.2 ms                                                | 89.7 ms: 1.01x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.19 us: 1.02x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 236 us: 1.03x slower                                                             |
| unpickle_list        | 5.29 us                                                | 5.52 us: 1.04x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 112 ms: 1.05x slower                                                             |
| tomli_loads          | 2.33 sec                                               | 2.56 sec: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.9 ms: 1.17x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 117 us: 1.34x faster                                                             |
| unpack_sequence            | 54.0 ns                                                | 40.6 ns: 1.33x faster                                                            |
| deepcopy_reduce            | 3.35 us                                                | 3.10 us: 1.08x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 303 us: 1.07x faster                                                             |
| logging_simple             | 6.46 us                                                | 6.08 us: 1.06x faster                                                            |
| logging_format             | 7.23 us                                                | 6.84 us: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                             |
| coroutines                 | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                            |
| async_tree_none            | 472 ms                                                 | 451 ms: 1.04x faster                                                             |
| unpickle                   | 15.9 us                                                | 15.2 us: 1.04x faster                                                            |
| raytrace                   | 312 ms                                                 | 299 ms: 1.04x faster                                                             |
| generators                 | 31.2 ms                                                | 30.0 ms: 1.04x faster                                                            |
| tornado_http               | 103 ms                                                 | 98.8 ms: 1.04x faster                                                            |
| pathlib                    | 19.3 ms                                                | 18.7 ms: 1.04x faster                                                            |
| deepcopy                   | 371 us                                                 | 359 us: 1.03x faster                                                             |
| sympy_str                  | 300 ms                                                 | 292 ms: 1.03x faster                                                             |
| docutils                   | 2.77 sec                                               | 2.70 sec: 1.02x faster                                                           |
| sqlglot_parse              | 1.36 ms                                                | 1.33 ms: 1.02x faster                                                            |
| scimark_lu                 | 118 ms                                                 | 115 ms: 1.02x faster                                                             |
| sqlglot_transpile          | 1.68 ms                                                | 1.66 ms: 1.01x faster                                                            |
| comprehensions             | 21.8 us                                                | 21.5 us: 1.01x faster                                                            |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| sympy_integrate            | 21.4 ms                                                | 21.2 ms: 1.01x faster                                                            |
| dask                       | 372 ms                                                 | 368 ms: 1.01x faster                                                             |
| pickle_dict                | 35.5 us                                                | 35.2 us: 1.01x faster                                                            |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                                            |
| async_generators           | 463 ms                                                 | 460 ms: 1.01x faster                                                             |
| xml_etree_parse            | 159 ms                                                 | 159 ms: 1.01x faster                                                             |
| xml_etree_process          | 61.7 ms                                                | 61.4 ms: 1.01x faster                                                            |
| asyncio_websockets         | 551 ms                                                 | 554 ms: 1.00x slower                                                             |
| deepcopy_memo              | 40.7 us                                                | 40.9 us: 1.00x slower                                                            |
| bench_thread_pool          | 842 us                                                 | 847 us: 1.01x slower                                                             |
| scimark_sor                | 129 ms                                                 | 130 ms: 1.01x slower                                                             |
| xml_etree_generate         | 89.2 ms                                                | 89.7 ms: 1.01x slower                                                            |
| sqlite_synth               | 2.83 us                                                | 2.85 us: 1.01x slower                                                            |
| create_gc_cycles           | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                            |
| gc_traversal               | 3.79 ms                                                | 3.82 ms: 1.01x slower                                                            |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                           |
| dulwich_log                | 68.5 ms                                                | 69.1 ms: 1.01x slower                                                            |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| regex_effbot               | 3.61 ms                                                | 3.66 ms: 1.01x slower                                                            |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 739 ms: 1.02x slower                                                             |
| sympy_expand               | 478 ms                                                 | 487 ms: 1.02x slower                                                             |
| pickle_list                | 5.08 us                                                | 5.19 us: 1.02x slower                                                            |
| async_tree_none_tg         | 450 ms                                                 | 460 ms: 1.02x slower                                                             |
| pycparser                  | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                           |
| regex_compile              | 148 ms                                                 | 152 ms: 1.03x slower                                                             |
| meteor_contest             | 112 ms                                                 | 115 ms: 1.03x slower                                                             |
| unpickle_pure_python       | 230 us                                                 | 236 us: 1.03x slower                                                             |
| sqlglot_normalize          | 110 ms                                                 | 113 ms: 1.03x slower                                                             |
| logging_silent             | 104 ns                                                 | 107 ns: 1.03x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 594 ms: 1.03x slower                                                             |
| crypto_pyaes               | 81.9 ms                                                | 84.9 ms: 1.04x slower                                                            |
| 2to3                       | 274 ms                                                 | 285 ms: 1.04x slower                                                             |
| async_tree_io              | 1.16 sec                                               | 1.21 sec: 1.04x slower                                                           |
| unpickle_list              | 5.29 us                                                | 5.52 us: 1.04x slower                                                            |
| xml_etree_iterparse        | 107 ms                                                 | 112 ms: 1.05x slower                                                             |
| pprint_safe_repr           | 776 ms                                                 | 814 ms: 1.05x slower                                                             |
| scimark_monte_carlo        | 75.1 ms                                                | 79.0 ms: 1.05x slower                                                            |
| richards                   | 45.8 ms                                                | 48.4 ms: 1.06x slower                                                            |
| sqlglot_optimize           | 54.8 ms                                                | 57.9 ms: 1.06x slower                                                            |
| richards_super             | 51.5 ms                                                | 54.7 ms: 1.06x slower                                                            |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| regex_dna                  | 212 ms                                                 | 228 ms: 1.08x slower                                                             |
| pprint_pformat             | 1.57 sec                                               | 1.70 sec: 1.08x slower                                                           |
| fannkuch                   | 417 ms                                                 | 451 ms: 1.08x slower                                                             |
| chaos                      | 67.0 ms                                                | 72.7 ms: 1.09x slower                                                            |
| float                      | 84.7 ms                                                | 92.9 ms: 1.10x slower                                                            |
| tomli_loads                | 2.33 sec                                               | 2.56 sec: 1.10x slower                                                           |
| go                         | 139 ms                                                 | 156 ms: 1.12x slower                                                             |
| regex_v8                   | 23.1 ms                                                | 25.9 ms: 1.12x slower                                                            |
| nqueens                    | 83.3 ms                                                | 94.1 ms: 1.13x slower                                                            |
| scimark_fft                | 382 ms                                                 | 432 ms: 1.13x slower                                                             |
| pyflate                    | 482 ms                                                 | 546 ms: 1.13x slower                                                             |
| mako                       | 11.9 ms                                                | 13.9 ms: 1.17x slower                                                            |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.98 ms: 1.18x slower                                                            |
| telco                      | 7.10 ms                                                | 8.56 ms: 1.21x slower                                                            |
| spectral_norm              | 115 ms                                                 | 143 ms: 1.25x slower                                                             |
| deltablue                  | 3.72 ms                                                | 4.65 ms: 1.25x slower                                                            |
| python_startup_no_site     | 6.94 ms                                                | 8.82 ms: 1.27x slower                                                            |
| nbody                      | 97.0 ms                                                | 125 ms: 1.29x slower                                                             |
| coverage                   | 72.7 ms                                                | 95.0 ms: 1.31x slower                                                            |
| hexiom                     | 6.41 ms                                                | 8.49 ms: 1.32x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (8): json, chameleon, async_tree_cpu_io_mixed, asyncio_tcp, bench_mp_pool, mdp, async_tree_memoization, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.94x