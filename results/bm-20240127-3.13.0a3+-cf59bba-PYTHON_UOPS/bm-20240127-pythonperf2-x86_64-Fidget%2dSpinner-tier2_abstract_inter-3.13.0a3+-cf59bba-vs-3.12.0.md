
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 310 ms: 1.09x slower                                                                   |
| chameleon      | 7.23 ms                                                      | 7.83 ms: 1.08x slower                                                                  |
| docutils       | 2.87 sec                                                     | 2.93 sec: 1.02x slower                                                                 |
| tornado_http   | 121 ms                                                       | 127 ms: 1.05x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 441 ms: 1.02x faster                                                                   |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 705 ms: 1.01x slower                                                                   |
| async_tree_memoization     | 544 ms                                                       | 554 ms: 1.02x slower                                                                   |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 711 ms: 1.02x slower                                                                   |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.02x slower                                                                 |
| async_tree_none_tg         | 431 ms                                                       | 441 ms: 1.02x slower                                                                   |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                                 |
| async_tree_memoization_tg  | 540 ms                                                       | 561 ms: 1.04x slower                                                                   |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 94.0 ms: 1.23x slower                                                                  |
| nbody          | 88.0 ms                                                      | 112 ms: 1.27x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.16x slower                                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.47 ms: 1.03x faster                                                                  |
| regex_dna      | 239 ms                                                       | 241 ms: 1.01x slower                                                                   |
| regex_v8       | 23.6 ms                                                      | 25.4 ms: 1.08x slower                                                                  |
| regex_compile  | 144 ms                                                       | 167 ms: 1.16x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 314 us: 1.01x faster                                                                   |
| pickle_dict          | 32.5 us                                                      | 32.8 us: 1.01x slower                                                                  |
| pickle               | 10.5 us                                                      | 10.6 us: 1.01x slower                                                                  |
| json_loads           | 24.4 us                                                      | 24.8 us: 1.02x slower                                                                  |
| unpickle_list        | 4.66 us                                                      | 4.74 us: 1.02x slower                                                                  |
| unpickle             | 14.8 us                                                      | 15.1 us: 1.02x slower                                                                  |
| pickle_list          | 4.43 us                                                      | 4.52 us: 1.02x slower                                                                  |
| xml_etree_parse      | 144 ms                                                       | 148 ms: 1.03x slower                                                                   |
| xml_etree_generate   | 86.1 ms                                                      | 90.0 ms: 1.05x slower                                                                  |
| xml_etree_process    | 58.4 ms                                                      | 61.6 ms: 1.06x slower                                                                  |
| json_dumps           | 10.2 ms                                                      | 10.9 ms: 1.07x slower                                                                  |
| xml_etree_iterparse  | 103 ms                                                       | 114 ms: 1.11x slower                                                                   |
| unpickle_pure_python | 210 us                                                       | 241 us: 1.15x slower                                                                   |
| tomli_loads          | 2.16 sec                                                     | 2.60 sec: 1.21x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.05x slower                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                                  |
| python_startup_no_site | 8.64 ms                                                      | 11.2 ms: 1.30x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.19x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 13.3 ms: 1.33x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 126 us: 1.20x faster                                                                   |
| unpack_sequence            | 53.2 ns                                                      | 46.5 ns: 1.14x faster                                                                  |
| generators                 | 37.4 ms                                                      | 34.2 ms: 1.09x faster                                                                  |
| coroutines                 | 23.0 ms                                                      | 22.0 ms: 1.04x faster                                                                  |
| async_generators           | 390 ms                                                       | 374 ms: 1.04x faster                                                                   |
| regex_effbot               | 3.57 ms                                                      | 3.47 ms: 1.03x faster                                                                  |
| async_tree_none            | 452 ms                                                       | 441 ms: 1.02x faster                                                                   |
| asyncio_tcp                | 378 ms                                                       | 373 ms: 1.01x faster                                                                   |
| pickle_pure_python         | 318 us                                                       | 314 us: 1.01x faster                                                                   |
| pathlib                    | 18.9 ms                                                      | 19.0 ms: 1.01x slower                                                                  |
| pickle_dict                | 32.5 us                                                      | 32.8 us: 1.01x slower                                                                  |
| pickle                     | 10.5 us                                                      | 10.6 us: 1.01x slower                                                                  |
| sqlite_synth               | 2.77 us                                                      | 2.80 us: 1.01x slower                                                                  |
| mdp                        | 2.57 sec                                                     | 2.60 sec: 1.01x slower                                                                 |
| regex_dna                  | 239 ms                                                       | 241 ms: 1.01x slower                                                                   |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 705 ms: 1.01x slower                                                                   |
| deepcopy_reduce            | 3.37 us                                                      | 3.42 us: 1.01x slower                                                                  |
| create_gc_cycles           | 1.59 ms                                                      | 1.62 ms: 1.02x slower                                                                  |
| gc_traversal               | 3.48 ms                                                      | 3.53 ms: 1.02x slower                                                                  |
| json_loads                 | 24.4 us                                                      | 24.8 us: 1.02x slower                                                                  |
| unpickle_list              | 4.66 us                                                      | 4.74 us: 1.02x slower                                                                  |
| async_tree_memoization     | 544 ms                                                       | 554 ms: 1.02x slower                                                                   |
| unpickle                   | 14.8 us                                                      | 15.1 us: 1.02x slower                                                                  |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 711 ms: 1.02x slower                                                                   |
| pickle_list                | 4.43 us                                                      | 4.52 us: 1.02x slower                                                                  |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.02x slower                                                                 |
| docutils                   | 2.87 sec                                                     | 2.93 sec: 1.02x slower                                                                 |
| async_tree_none_tg         | 431 ms                                                       | 441 ms: 1.02x slower                                                                   |
| sqlglot_parse              | 1.38 ms                                                      | 1.41 ms: 1.02x slower                                                                  |
| json                       | 5.12 ms                                                      | 5.25 ms: 1.03x slower                                                                  |
| sqlglot_transpile          | 1.78 ms                                                      | 1.82 ms: 1.03x slower                                                                  |
| sympy_sum                  | 162 ms                                                       | 167 ms: 1.03x slower                                                                   |
| xml_etree_parse            | 144 ms                                                       | 148 ms: 1.03x slower                                                                   |
| sympy_integrate            | 23.9 ms                                                      | 24.7 ms: 1.03x slower                                                                  |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                                 |
| bench_thread_pool          | 950 us                                                       | 985 us: 1.04x slower                                                                   |
| async_tree_memoization_tg  | 540 ms                                                       | 561 ms: 1.04x slower                                                                   |
| deepcopy                   | 368 us                                                       | 383 us: 1.04x slower                                                                   |
| logging_simple             | 6.71 us                                                      | 6.98 us: 1.04x slower                                                                  |
| dask                       | 392 ms                                                       | 410 ms: 1.04x slower                                                                   |
| xml_etree_generate         | 86.1 ms                                                      | 90.0 ms: 1.05x slower                                                                  |
| tornado_http               | 121 ms                                                       | 127 ms: 1.05x slower                                                                   |
| comprehensions             | 21.9 us                                                      | 23.0 us: 1.05x slower                                                                  |
| sqlglot_normalize          | 116 ms                                                       | 122 ms: 1.05x slower                                                                   |
| logging_silent             | 94.4 ns                                                      | 99.6 ns: 1.06x slower                                                                  |
| xml_etree_process          | 58.4 ms                                                      | 61.6 ms: 1.06x slower                                                                  |
| scimark_lu                 | 98.8 ms                                                      | 104 ms: 1.06x slower                                                                   |
| sympy_str                  | 302 ms                                                       | 320 ms: 1.06x slower                                                                   |
| meteor_contest             | 128 ms                                                       | 136 ms: 1.06x slower                                                                   |
| json_dumps                 | 10.2 ms                                                      | 10.9 ms: 1.07x slower                                                                  |
| regex_v8                   | 23.6 ms                                                      | 25.4 ms: 1.08x slower                                                                  |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.08x slower                                                                 |
| mypy2                      | 830 ms                                                       | 897 ms: 1.08x slower                                                                   |
| chameleon                  | 7.23 ms                                                      | 7.83 ms: 1.08x slower                                                                  |
| 2to3                       | 285 ms                                                       | 310 ms: 1.09x slower                                                                   |
| python_startup             | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                                  |
| sqlglot_optimize           | 57.5 ms                                                      | 63.3 ms: 1.10x slower                                                                  |
| dulwich_log                | 65.4 ms                                                      | 72.0 ms: 1.10x slower                                                                  |
| deepcopy_memo              | 36.8 us                                                      | 40.7 us: 1.11x slower                                                                  |
| sympy_expand               | 484 ms                                                       | 537 ms: 1.11x slower                                                                   |
| xml_etree_iterparse        | 103 ms                                                       | 114 ms: 1.11x slower                                                                   |
| pprint_safe_repr           | 807 ms                                                       | 901 ms: 1.12x slower                                                                   |
| pprint_pformat             | 1.65 sec                                                     | 1.85 sec: 1.12x slower                                                                 |
| nqueens                    | 89.9 ms                                                      | 102 ms: 1.14x slower                                                                   |
| chaos                      | 64.0 ms                                                      | 72.8 ms: 1.14x slower                                                                  |
| richards_super             | 51.3 ms                                                      | 59.1 ms: 1.15x slower                                                                  |
| unpickle_pure_python       | 210 us                                                       | 241 us: 1.15x slower                                                                   |
| regex_compile              | 144 ms                                                       | 167 ms: 1.16x slower                                                                   |
| richards                   | 45.7 ms                                                      | 53.5 ms: 1.17x slower                                                                  |
| scimark_monte_carlo        | 69.0 ms                                                      | 81.1 ms: 1.18x slower                                                                  |
| telco                      | 6.96 ms                                                      | 8.29 ms: 1.19x slower                                                                  |
| go                         | 150 ms                                                       | 180 ms: 1.20x slower                                                                   |
| coverage                   | 66.7 ms                                                      | 80.4 ms: 1.20x slower                                                                  |
| tomli_loads                | 2.16 sec                                                     | 2.60 sec: 1.21x slower                                                                 |
| float                      | 76.6 ms                                                      | 94.0 ms: 1.23x slower                                                                  |
| fannkuch                   | 350 ms                                                       | 445 ms: 1.27x slower                                                                   |
| nbody                      | 88.0 ms                                                      | 112 ms: 1.27x slower                                                                   |
| python_startup_no_site     | 8.64 ms                                                      | 11.2 ms: 1.30x slower                                                                  |
| scimark_fft                | 301 ms                                                       | 392 ms: 1.30x slower                                                                   |
| pyflate                    | 439 ms                                                       | 576 ms: 1.31x slower                                                                   |
| scimark_sor                | 109 ms                                                       | 143 ms: 1.32x slower                                                                   |
| mako                       | 10.0 ms                                                      | 13.3 ms: 1.33x slower                                                                  |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.01 ms: 1.43x slower                                                                  |
| deltablue                  | 3.24 ms                                                      | 4.86 ms: 1.50x slower                                                                  |
| spectral_norm              | 91.6 ms                                                      | 138 ms: 1.51x slower                                                                   |
| hexiom                     | 5.96 ms                                                      | 9.05 ms: 1.52x slower                                                                  |
| Geometric mean             | (ref)                                                        | 1.08x slower                                                                           |

Benchmark hidden because not significant (7): bench_mp_pool, asyncio_websockets, raytrace, asyncio_tcp_ssl, pidigits, crypto_pyaes, logging_format
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 0.90x