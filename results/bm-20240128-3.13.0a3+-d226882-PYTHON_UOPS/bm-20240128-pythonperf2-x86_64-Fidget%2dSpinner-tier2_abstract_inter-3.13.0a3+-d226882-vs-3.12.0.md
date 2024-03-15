
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 309 ms: 1.08x slower                                                                   |
| chameleon      | 7.23 ms                                                      | 8.09 ms: 1.12x slower                                                                  |
| docutils       | 2.87 sec                                                     | 2.95 sec: 1.03x slower                                                                 |
| tornado_http   | 121 ms                                                       | 129 ms: 1.06x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 438 ms: 1.03x faster                                                                   |
| async_tree_memoization     | 544 ms                                                       | 549 ms: 1.01x slower                                                                   |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 707 ms: 1.01x slower                                                                   |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                                 |
| async_tree_none_tg         | 431 ms                                                       | 441 ms: 1.02x slower                                                                   |
| async_tree_io              | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                                 |
| async_tree_memoization_tg  | 540 ms                                                       | 555 ms: 1.03x slower                                                                   |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 264 ms: 1.00x faster                                                                   |
| float          | 76.6 ms                                                      | 95.3 ms: 1.24x slower                                                                  |
| nbody          | 88.0 ms                                                      | 114 ms: 1.30x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.17x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 251 ms: 1.05x slower                                                                   |
| regex_v8       | 23.6 ms                                                      | 26.3 ms: 1.11x slower                                                                  |
| regex_compile  | 144 ms                                                       | 169 ms: 1.17x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| unpickle             | 14.8 us                                                      | 14.5 us: 1.02x faster                                                                  |
| pickle_pure_python   | 318 us                                                       | 314 us: 1.01x faster                                                                   |
| pickle               | 10.5 us                                                      | 10.7 us: 1.02x slower                                                                  |
| unpickle_list        | 4.66 us                                                      | 4.75 us: 1.02x slower                                                                  |
| json_loads           | 24.4 us                                                      | 24.9 us: 1.02x slower                                                                  |
| xml_etree_generate   | 86.1 ms                                                      | 89.9 ms: 1.04x slower                                                                  |
| xml_etree_process    | 58.4 ms                                                      | 61.6 ms: 1.06x slower                                                                  |
| json_dumps           | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                                  |
| pickle_dict          | 32.5 us                                                      | 34.6 us: 1.06x slower                                                                  |
| unpickle_pure_python | 210 us                                                       | 229 us: 1.09x slower                                                                   |
| xml_etree_iterparse  | 103 ms                                                       | 112 ms: 1.09x slower                                                                   |
| tomli_loads          | 2.16 sec                                                     | 2.61 sec: 1.21x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                           |

Benchmark hidden because not significant (2): pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                                  |
| python_startup_no_site | 8.64 ms                                                      | 11.2 ms: 1.29x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.19x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 13.6 ms: 1.36x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| unpack_sequence            | 53.2 ns                                                      | 42.2 ns: 1.26x faster                                                                  |
| typing_runtime_protocols   | 152 us                                                       | 127 us: 1.19x faster                                                                   |
| generators                 | 37.4 ms                                                      | 34.2 ms: 1.09x faster                                                                  |
| async_generators           | 390 ms                                                       | 375 ms: 1.04x faster                                                                   |
| logging_format             | 7.48 us                                                      | 7.20 us: 1.04x faster                                                                  |
| coroutines                 | 23.0 ms                                                      | 22.2 ms: 1.04x faster                                                                  |
| async_tree_none            | 452 ms                                                       | 438 ms: 1.03x faster                                                                   |
| unpickle                   | 14.8 us                                                      | 14.5 us: 1.02x faster                                                                  |
| asyncio_websockets         | 387 ms                                                       | 380 ms: 1.02x faster                                                                   |
| pickle_pure_python         | 318 us                                                       | 314 us: 1.01x faster                                                                   |
| logging_simple             | 6.71 us                                                      | 6.65 us: 1.01x faster                                                                  |
| asyncio_tcp                | 378 ms                                                       | 377 ms: 1.00x faster                                                                   |
| pidigits                   | 265 ms                                                       | 264 ms: 1.00x faster                                                                   |
| async_tree_memoization     | 544 ms                                                       | 549 ms: 1.01x slower                                                                   |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                                  |
| sqlite_synth               | 2.77 us                                                      | 2.81 us: 1.01x slower                                                                  |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 707 ms: 1.01x slower                                                                   |
| mdp                        | 2.57 sec                                                     | 2.61 sec: 1.01x slower                                                                 |
| pickle                     | 10.5 us                                                      | 10.7 us: 1.02x slower                                                                  |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                                 |
| crypto_pyaes               | 80.3 ms                                                      | 81.8 ms: 1.02x slower                                                                  |
| unpickle_list              | 4.66 us                                                      | 4.75 us: 1.02x slower                                                                  |
| deepcopy_reduce            | 3.37 us                                                      | 3.44 us: 1.02x slower                                                                  |
| create_gc_cycles           | 1.59 ms                                                      | 1.62 ms: 1.02x slower                                                                  |
| async_tree_none_tg         | 431 ms                                                       | 441 ms: 1.02x slower                                                                   |
| json_loads                 | 24.4 us                                                      | 24.9 us: 1.02x slower                                                                  |
| gc_traversal               | 3.48 ms                                                      | 3.56 ms: 1.02x slower                                                                  |
| async_tree_io              | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                                 |
| async_tree_memoization_tg  | 540 ms                                                       | 555 ms: 1.03x slower                                                                   |
| docutils                   | 2.87 sec                                                     | 2.95 sec: 1.03x slower                                                                 |
| bench_thread_pool          | 950 us                                                       | 985 us: 1.04x slower                                                                   |
| json                       | 5.12 ms                                                      | 5.31 ms: 1.04x slower                                                                  |
| sqlglot_parse              | 1.38 ms                                                      | 1.44 ms: 1.04x slower                                                                  |
| xml_etree_generate         | 86.1 ms                                                      | 89.9 ms: 1.04x slower                                                                  |
| sqlglot_transpile          | 1.78 ms                                                      | 1.85 ms: 1.04x slower                                                                  |
| sympy_integrate            | 23.9 ms                                                      | 25.0 ms: 1.05x slower                                                                  |
| sympy_sum                  | 162 ms                                                       | 170 ms: 1.05x slower                                                                   |
| dask                       | 392 ms                                                       | 413 ms: 1.05x slower                                                                   |
| regex_dna                  | 239 ms                                                       | 251 ms: 1.05x slower                                                                   |
| sqlglot_normalize          | 116 ms                                                       | 122 ms: 1.05x slower                                                                   |
| xml_etree_process          | 58.4 ms                                                      | 61.6 ms: 1.06x slower                                                                  |
| comprehensions             | 21.9 us                                                      | 23.1 us: 1.06x slower                                                                  |
| json_dumps                 | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                                  |
| deepcopy                   | 368 us                                                       | 391 us: 1.06x slower                                                                   |
| tornado_http               | 121 ms                                                       | 129 ms: 1.06x slower                                                                   |
| pickle_dict                | 32.5 us                                                      | 34.6 us: 1.06x slower                                                                  |
| logging_silent             | 94.4 ns                                                      | 100 ns: 1.06x slower                                                                   |
| meteor_contest             | 128 ms                                                       | 137 ms: 1.07x slower                                                                   |
| scimark_lu                 | 98.8 ms                                                      | 106 ms: 1.07x slower                                                                   |
| sympy_str                  | 302 ms                                                       | 325 ms: 1.07x slower                                                                   |
| mypy2                      | 830 ms                                                       | 898 ms: 1.08x slower                                                                   |
| 2to3                       | 285 ms                                                       | 309 ms: 1.08x slower                                                                   |
| unpickle_pure_python       | 210 us                                                       | 229 us: 1.09x slower                                                                   |
| xml_etree_iterparse        | 103 ms                                                       | 112 ms: 1.09x slower                                                                   |
| pycparser                  | 1.23 sec                                                     | 1.35 sec: 1.09x slower                                                                 |
| python_startup             | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                                  |
| sqlglot_optimize           | 57.5 ms                                                      | 63.4 ms: 1.10x slower                                                                  |
| regex_v8                   | 23.6 ms                                                      | 26.3 ms: 1.11x slower                                                                  |
| pprint_safe_repr           | 807 ms                                                       | 901 ms: 1.12x slower                                                                   |
| pprint_pformat             | 1.65 sec                                                     | 1.85 sec: 1.12x slower                                                                 |
| chameleon                  | 7.23 ms                                                      | 8.09 ms: 1.12x slower                                                                  |
| deepcopy_memo              | 36.8 us                                                      | 41.3 us: 1.12x slower                                                                  |
| dulwich_log                | 65.4 ms                                                      | 73.5 ms: 1.13x slower                                                                  |
| sympy_expand               | 484 ms                                                       | 547 ms: 1.13x slower                                                                   |
| nqueens                    | 89.9 ms                                                      | 104 ms: 1.15x slower                                                                   |
| chaos                      | 64.0 ms                                                      | 73.8 ms: 1.15x slower                                                                  |
| richards_super             | 51.3 ms                                                      | 59.4 ms: 1.16x slower                                                                  |
| richards                   | 45.7 ms                                                      | 53.5 ms: 1.17x slower                                                                  |
| regex_compile              | 144 ms                                                       | 169 ms: 1.17x slower                                                                   |
| go                         | 150 ms                                                       | 177 ms: 1.18x slower                                                                   |
| scimark_monte_carlo        | 69.0 ms                                                      | 81.9 ms: 1.19x slower                                                                  |
| telco                      | 6.96 ms                                                      | 8.27 ms: 1.19x slower                                                                  |
| coverage                   | 66.7 ms                                                      | 79.3 ms: 1.19x slower                                                                  |
| tomli_loads                | 2.16 sec                                                     | 2.61 sec: 1.21x slower                                                                 |
| float                      | 76.6 ms                                                      | 95.3 ms: 1.24x slower                                                                  |
| fannkuch                   | 350 ms                                                       | 446 ms: 1.28x slower                                                                   |
| pyflate                    | 439 ms                                                       | 561 ms: 1.28x slower                                                                   |
| python_startup_no_site     | 8.64 ms                                                      | 11.2 ms: 1.29x slower                                                                  |
| nbody                      | 88.0 ms                                                      | 114 ms: 1.30x slower                                                                   |
| scimark_fft                | 301 ms                                                       | 396 ms: 1.32x slower                                                                   |
| mako                       | 10.0 ms                                                      | 13.6 ms: 1.36x slower                                                                  |
| scimark_sor                | 109 ms                                                       | 148 ms: 1.36x slower                                                                   |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.10 ms: 1.45x slower                                                                  |
| hexiom                     | 5.96 ms                                                      | 8.91 ms: 1.50x slower                                                                  |
| deltablue                  | 3.24 ms                                                      | 4.88 ms: 1.51x slower                                                                  |
| spectral_norm              | 91.6 ms                                                      | 144 ms: 1.57x slower                                                                   |
| Geometric mean             | (ref)                                                        | 1.08x slower                                                                           |

Benchmark hidden because not significant (7): asyncio_tcp_ssl, regex_effbot, raytrace, pickle_list, bench_mp_pool, xml_etree_parse, async_tree_cpu_io_mixed
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.88x