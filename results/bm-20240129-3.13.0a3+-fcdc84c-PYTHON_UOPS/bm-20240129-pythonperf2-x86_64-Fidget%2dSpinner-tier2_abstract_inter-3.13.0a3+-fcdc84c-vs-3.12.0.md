
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 309 ms: 1.08x slower                                                                   |
| chameleon      | 7.23 ms                                                      | 8.13 ms: 1.12x slower                                                                  |
| docutils       | 2.87 sec                                                     | 2.93 sec: 1.02x slower                                                                 |
| tornado_http   | 121 ms                                                       | 126 ms: 1.04x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 440 ms: 1.03x faster                                                                   |
| async_tree_memoization     | 544 ms                                                       | 550 ms: 1.01x slower                                                                   |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 705 ms: 1.01x slower                                                                   |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 709 ms: 1.02x slower                                                                   |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                                 |
| async_tree_none_tg         | 431 ms                                                       | 440 ms: 1.02x slower                                                                   |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                                 |
| async_tree_memoization_tg  | 540 ms                                                       | 563 ms: 1.04x slower                                                                   |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 264 ms: 1.00x faster                                                                   |
| float          | 76.6 ms                                                      | 94.5 ms: 1.23x slower                                                                  |
| nbody          | 88.0 ms                                                      | 111 ms: 1.26x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.16x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.42 ms: 1.04x faster                                                                  |
| regex_dna      | 239 ms                                                       | 236 ms: 1.01x faster                                                                   |
| regex_v8       | 23.6 ms                                                      | 25.8 ms: 1.09x slower                                                                  |
| regex_compile  | 144 ms                                                       | 168 ms: 1.17x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 312 us: 1.02x faster                                                                   |
| pickle_list          | 4.43 us                                                      | 4.40 us: 1.01x faster                                                                  |
| pickle               | 10.5 us                                                      | 10.5 us: 1.01x faster                                                                  |
| pickle_dict          | 32.5 us                                                      | 32.4 us: 1.00x faster                                                                  |
| unpickle             | 14.8 us                                                      | 14.9 us: 1.01x slower                                                                  |
| json_loads           | 24.4 us                                                      | 24.5 us: 1.01x slower                                                                  |
| unpickle_list        | 4.66 us                                                      | 4.76 us: 1.02x slower                                                                  |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                                   |
| xml_etree_generate   | 86.1 ms                                                      | 90.1 ms: 1.05x slower                                                                  |
| xml_etree_process    | 58.4 ms                                                      | 61.2 ms: 1.05x slower                                                                  |
| json_dumps           | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                                  |
| unpickle_pure_python | 210 us                                                       | 229 us: 1.09x slower                                                                   |
| xml_etree_iterparse  | 103 ms                                                       | 113 ms: 1.10x slower                                                                   |
| tomli_loads          | 2.16 sec                                                     | 2.58 sec: 1.19x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                                  |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 14.0 ms: 1.40x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| unpack_sequence            | 53.2 ns                                                      | 43.3 ns: 1.23x faster                                                                  |
| typing_runtime_protocols   | 152 us                                                       | 129 us: 1.18x faster                                                                   |
| generators                 | 37.4 ms                                                      | 34.1 ms: 1.10x faster                                                                  |
| regex_effbot               | 3.57 ms                                                      | 3.42 ms: 1.04x faster                                                                  |
| async_generators           | 390 ms                                                       | 379 ms: 1.03x faster                                                                   |
| logging_format             | 7.48 us                                                      | 7.28 us: 1.03x faster                                                                  |
| async_tree_none            | 452 ms                                                       | 440 ms: 1.03x faster                                                                   |
| coroutines                 | 23.0 ms                                                      | 22.5 ms: 1.02x faster                                                                  |
| pickle_pure_python         | 318 us                                                       | 312 us: 1.02x faster                                                                   |
| asyncio_tcp                | 378 ms                                                       | 373 ms: 1.01x faster                                                                   |
| regex_dna                  | 239 ms                                                       | 236 ms: 1.01x faster                                                                   |
| asyncio_websockets         | 387 ms                                                       | 384 ms: 1.01x faster                                                                   |
| pickle_list                | 4.43 us                                                      | 4.40 us: 1.01x faster                                                                  |
| pickle                     | 10.5 us                                                      | 10.5 us: 1.01x faster                                                                  |
| pickle_dict                | 32.5 us                                                      | 32.4 us: 1.00x faster                                                                  |
| pidigits                   | 265 ms                                                       | 264 ms: 1.00x faster                                                                   |
| unpickle                   | 14.8 us                                                      | 14.9 us: 1.01x slower                                                                  |
| json_loads                 | 24.4 us                                                      | 24.5 us: 1.01x slower                                                                  |
| async_tree_memoization     | 544 ms                                                       | 550 ms: 1.01x slower                                                                   |
| deepcopy_reduce            | 3.37 us                                                      | 3.41 us: 1.01x slower                                                                  |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 705 ms: 1.01x slower                                                                   |
| gc_traversal               | 3.48 ms                                                      | 3.53 ms: 1.01x slower                                                                  |
| sqlite_synth               | 2.77 us                                                      | 2.82 us: 1.02x slower                                                                  |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 709 ms: 1.02x slower                                                                   |
| json                       | 5.12 ms                                                      | 5.20 ms: 1.02x slower                                                                  |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                                 |
| pathlib                    | 18.9 ms                                                      | 19.2 ms: 1.02x slower                                                                  |
| bench_thread_pool          | 950 us                                                       | 971 us: 1.02x slower                                                                   |
| unpickle_list              | 4.66 us                                                      | 4.76 us: 1.02x slower                                                                  |
| async_tree_none_tg         | 431 ms                                                       | 440 ms: 1.02x slower                                                                   |
| docutils                   | 2.87 sec                                                     | 2.93 sec: 1.02x slower                                                                 |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                                   |
| crypto_pyaes               | 80.3 ms                                                      | 82.5 ms: 1.03x slower                                                                  |
| sympy_integrate            | 23.9 ms                                                      | 24.7 ms: 1.03x slower                                                                  |
| sqlglot_parse              | 1.38 ms                                                      | 1.42 ms: 1.03x slower                                                                  |
| sympy_sum                  | 162 ms                                                       | 167 ms: 1.03x slower                                                                   |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                                 |
| sqlglot_transpile          | 1.78 ms                                                      | 1.84 ms: 1.03x slower                                                                  |
| mdp                        | 2.57 sec                                                     | 2.66 sec: 1.03x slower                                                                 |
| dask                       | 392 ms                                                       | 408 ms: 1.04x slower                                                                   |
| tornado_http               | 121 ms                                                       | 126 ms: 1.04x slower                                                                   |
| async_tree_memoization_tg  | 540 ms                                                       | 563 ms: 1.04x slower                                                                   |
| deepcopy                   | 368 us                                                       | 384 us: 1.04x slower                                                                   |
| xml_etree_generate         | 86.1 ms                                                      | 90.1 ms: 1.05x slower                                                                  |
| xml_etree_process          | 58.4 ms                                                      | 61.2 ms: 1.05x slower                                                                  |
| scimark_lu                 | 98.8 ms                                                      | 104 ms: 1.05x slower                                                                   |
| logging_silent             | 94.4 ns                                                      | 99.5 ns: 1.05x slower                                                                  |
| json_dumps                 | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                                  |
| sympy_str                  | 302 ms                                                       | 319 ms: 1.06x slower                                                                   |
| comprehensions             | 21.9 us                                                      | 23.2 us: 1.06x slower                                                                  |
| sqlglot_normalize          | 116 ms                                                       | 123 ms: 1.06x slower                                                                   |
| meteor_contest             | 128 ms                                                       | 136 ms: 1.06x slower                                                                   |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.08x slower                                                                 |
| 2to3                       | 285 ms                                                       | 309 ms: 1.08x slower                                                                   |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                                  |
| regex_v8                   | 23.6 ms                                                      | 25.8 ms: 1.09x slower                                                                  |
| unpickle_pure_python       | 210 us                                                       | 229 us: 1.09x slower                                                                   |
| dulwich_log                | 65.4 ms                                                      | 71.7 ms: 1.10x slower                                                                  |
| xml_etree_iterparse        | 103 ms                                                       | 113 ms: 1.10x slower                                                                   |
| sqlglot_optimize           | 57.5 ms                                                      | 63.2 ms: 1.10x slower                                                                  |
| sympy_expand               | 484 ms                                                       | 536 ms: 1.11x slower                                                                   |
| pprint_safe_repr           | 807 ms                                                       | 895 ms: 1.11x slower                                                                   |
| pprint_pformat             | 1.65 sec                                                     | 1.85 sec: 1.12x slower                                                                 |
| deepcopy_memo              | 36.8 us                                                      | 41.2 us: 1.12x slower                                                                  |
| chameleon                  | 7.23 ms                                                      | 8.13 ms: 1.12x slower                                                                  |
| chaos                      | 64.0 ms                                                      | 72.0 ms: 1.13x slower                                                                  |
| nqueens                    | 89.9 ms                                                      | 103 ms: 1.14x slower                                                                   |
| regex_compile              | 144 ms                                                       | 168 ms: 1.17x slower                                                                   |
| coverage                   | 66.7 ms                                                      | 78.5 ms: 1.18x slower                                                                  |
| richards_super             | 51.3 ms                                                      | 60.5 ms: 1.18x slower                                                                  |
| go                         | 150 ms                                                       | 177 ms: 1.18x slower                                                                   |
| richards                   | 45.7 ms                                                      | 54.2 ms: 1.18x slower                                                                  |
| scimark_monte_carlo        | 69.0 ms                                                      | 81.8 ms: 1.19x slower                                                                  |
| tomli_loads                | 2.16 sec                                                     | 2.58 sec: 1.19x slower                                                                 |
| telco                      | 6.96 ms                                                      | 8.35 ms: 1.20x slower                                                                  |
| float                      | 76.6 ms                                                      | 94.5 ms: 1.23x slower                                                                  |
| fannkuch                   | 350 ms                                                       | 438 ms: 1.25x slower                                                                   |
| scimark_fft                | 301 ms                                                       | 379 ms: 1.26x slower                                                                   |
| nbody                      | 88.0 ms                                                      | 111 ms: 1.26x slower                                                                   |
| pyflate                    | 439 ms                                                       | 554 ms: 1.26x slower                                                                   |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                                  |
| scimark_sor                | 109 ms                                                       | 147 ms: 1.35x slower                                                                   |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 5.82 ms: 1.38x slower                                                                  |
| mako                       | 10.0 ms                                                      | 14.0 ms: 1.40x slower                                                                  |
| spectral_norm              | 91.6 ms                                                      | 135 ms: 1.48x slower                                                                   |
| deltablue                  | 3.24 ms                                                      | 4.81 ms: 1.49x slower                                                                  |
| hexiom                     | 5.96 ms                                                      | 8.99 ms: 1.51x slower                                                                  |
| Geometric mean             | (ref)                                                        | 1.08x slower                                                                           |

Benchmark hidden because not significant (6): bench_mp_pool, asyncio_tcp_ssl, logging_simple, raytrace, create_gc_cycles, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 0.88x