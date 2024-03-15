# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_inliner_redux
- machine: linux-x86_64
- commit hash: b04215f
- commit date: 2024-03-05
- overall geometric mean: 1.10x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 300 ms: 1.09x slower                                                            |
| chameleon      | 7.41 ms                                                | 7.00 ms: 1.06x faster                                                           |
| docutils       | 2.77 sec                                               | 2.84 sec: 1.03x slower                                                          |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                    |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 462 ms: 1.02x faster                                                            |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 734 ms: 1.01x slower                                                            |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 737 ms: 1.02x slower                                                            |
| async_tree_memoization_tg  | 575 ms                                                 | 589 ms: 1.03x slower                                                            |
| async_tree_memoization     | 578 ms                                                 | 592 ms: 1.03x slower                                                            |
| async_tree_none_tg         | 450 ms                                                 | 462 ms: 1.03x slower                                                            |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                          |
| async_tree_io              | 1.16 sec                                               | 1.25 sec: 1.08x slower                                                          |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                                            |
| float          | 84.7 ms                                                | 106 ms: 1.25x slower                                                            |
| nbody          | 97.0 ms                                                | 132 ms: 1.36x slower                                                            |
| Geometric mean | (ref)                                                  | 1.20x slower                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.55 ms: 1.02x faster                                                           |
| regex_dna      | 212 ms                                                 | 213 ms: 1.00x slower                                                            |
| regex_v8       | 23.1 ms                                                | 24.4 ms: 1.05x slower                                                           |
| regex_compile  | 148 ms                                                 | 191 ms: 1.29x slower                                                            |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 303 us: 1.07x faster                                                            |
| unpickle_list        | 5.29 us                                                | 5.12 us: 1.03x faster                                                           |
| json_loads           | 28.5 us                                                | 27.9 us: 1.02x faster                                                           |
| pickle_dict          | 35.5 us                                                | 35.1 us: 1.01x faster                                                           |
| unpickle             | 15.9 us                                                | 15.7 us: 1.01x faster                                                           |
| xml_etree_process    | 61.7 ms                                                | 63.1 ms: 1.02x slower                                                           |
| pickle               | 11.6 us                                                | 11.9 us: 1.02x slower                                                           |
| xml_etree_generate   | 89.2 ms                                                | 93.3 ms: 1.05x slower                                                           |
| pickle_list          | 5.08 us                                                | 5.33 us: 1.05x slower                                                           |
| xml_etree_iterparse  | 107 ms                                                 | 116 ms: 1.08x slower                                                            |
| tomli_loads          | 2.33 sec                                               | 2.79 sec: 1.20x slower                                                          |
| unpickle_pure_python | 230 us                                                 | 309 us: 1.34x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                                    |

Benchmark hidden because not significant (2): json_dumps, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                           |
| python_startup_no_site | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                           |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 15.1 ms: 1.27x slower                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 119 us: 1.33x faster                                                            |
| logging_simple             | 6.46 us                                                | 6.00 us: 1.08x faster                                                           |
| pickle_pure_python         | 324 us                                                 | 303 us: 1.07x faster                                                            |
| logging_format             | 7.23 us                                                | 6.79 us: 1.06x faster                                                           |
| deepcopy_reduce            | 3.35 us                                                | 3.15 us: 1.06x faster                                                           |
| chameleon                  | 7.41 ms                                                | 7.00 ms: 1.06x faster                                                           |
| generators                 | 31.2 ms                                                | 29.9 ms: 1.04x faster                                                           |
| unpickle_list              | 5.29 us                                                | 5.12 us: 1.03x faster                                                           |
| json                       | 5.26 ms                                                | 5.13 ms: 1.02x faster                                                           |
| json_loads                 | 28.5 us                                                | 27.9 us: 1.02x faster                                                           |
| async_tree_none            | 472 ms                                                 | 462 ms: 1.02x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 166 ms: 1.02x faster                                                            |
| coroutines                 | 23.2 ms                                                | 22.7 ms: 1.02x faster                                                           |
| regex_effbot               | 3.61 ms                                                | 3.55 ms: 1.02x faster                                                           |
| deepcopy                   | 371 us                                                 | 366 us: 1.01x faster                                                            |
| pickle_dict                | 35.5 us                                                | 35.1 us: 1.01x faster                                                           |
| unpickle                   | 15.9 us                                                | 15.7 us: 1.01x faster                                                           |
| asyncio_tcp                | 491 ms                                                 | 489 ms: 1.00x faster                                                            |
| regex_dna                  | 212 ms                                                 | 213 ms: 1.00x slower                                                            |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                          |
| sympy_integrate            | 21.4 ms                                                | 21.6 ms: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 734 ms: 1.01x slower                                                            |
| pidigits                   | 187 ms                                                 | 190 ms: 1.01x slower                                                            |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 737 ms: 1.02x slower                                                            |
| create_gc_cycles           | 1.48 ms                                                | 1.50 ms: 1.02x slower                                                           |
| xml_etree_process          | 61.7 ms                                                | 63.1 ms: 1.02x slower                                                           |
| sympy_str                  | 300 ms                                                 | 306 ms: 1.02x slower                                                            |
| pickle                     | 11.6 us                                                | 11.9 us: 1.02x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 589 ms: 1.03x slower                                                            |
| async_tree_memoization     | 578 ms                                                 | 592 ms: 1.03x slower                                                            |
| docutils                   | 2.77 sec                                               | 2.84 sec: 1.03x slower                                                          |
| async_tree_none_tg         | 450 ms                                                 | 462 ms: 1.03x slower                                                            |
| bench_thread_pool          | 842 us                                                 | 867 us: 1.03x slower                                                            |
| sqlglot_normalize          | 110 ms                                                 | 114 ms: 1.03x slower                                                            |
| xml_etree_generate         | 89.2 ms                                                | 93.3 ms: 1.05x slower                                                           |
| pickle_list                | 5.08 us                                                | 5.33 us: 1.05x slower                                                           |
| sqlite_synth               | 2.83 us                                                | 2.98 us: 1.05x slower                                                           |
| dulwich_log                | 68.5 ms                                                | 72.1 ms: 1.05x slower                                                           |
| regex_v8                   | 23.1 ms                                                | 24.4 ms: 1.05x slower                                                           |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                          |
| gc_traversal               | 3.79 ms                                                | 4.02 ms: 1.06x slower                                                           |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                           |
| sympy_expand               | 478 ms                                                 | 514 ms: 1.08x slower                                                            |
| deepcopy_memo              | 40.7 us                                                | 43.8 us: 1.08x slower                                                           |
| comprehensions             | 21.8 us                                                | 23.5 us: 1.08x slower                                                           |
| sqlglot_transpile          | 1.68 ms                                                | 1.82 ms: 1.08x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.25 sec: 1.08x slower                                                          |
| deltablue                  | 3.72 ms                                                | 4.02 ms: 1.08x slower                                                           |
| xml_etree_iterparse        | 107 ms                                                 | 116 ms: 1.08x slower                                                            |
| sqlglot_parse              | 1.36 ms                                                | 1.48 ms: 1.08x slower                                                           |
| meteor_contest             | 112 ms                                                 | 122 ms: 1.09x slower                                                            |
| 2to3                       | 274 ms                                                 | 300 ms: 1.09x slower                                                            |
| mdp                        | 2.63 sec                                               | 2.88 sec: 1.09x slower                                                          |
| mypy2                      | 830 ms                                                 | 911 ms: 1.10x slower                                                            |
| pycparser                  | 1.18 sec                                               | 1.30 sec: 1.10x slower                                                          |
| crypto_pyaes               | 81.9 ms                                                | 92.2 ms: 1.13x slower                                                           |
| unpack_sequence            | 54.0 ns                                                | 61.2 ns: 1.13x slower                                                           |
| sqlglot_optimize           | 54.8 ms                                                | 62.7 ms: 1.14x slower                                                           |
| scimark_sor                | 129 ms                                                 | 148 ms: 1.15x slower                                                            |
| raytrace                   | 312 ms                                                 | 367 ms: 1.18x slower                                                            |
| tomli_loads                | 2.33 sec                                               | 2.79 sec: 1.20x slower                                                          |
| chaos                      | 67.0 ms                                                | 80.3 ms: 1.20x slower                                                           |
| pprint_safe_repr           | 776 ms                                                 | 945 ms: 1.22x slower                                                            |
| scimark_fft                | 382 ms                                                 | 473 ms: 1.24x slower                                                            |
| telco                      | 7.10 ms                                                | 8.84 ms: 1.25x slower                                                           |
| float                      | 84.7 ms                                                | 106 ms: 1.25x slower                                                            |
| pprint_pformat             | 1.57 sec                                               | 1.96 sec: 1.25x slower                                                          |
| mako                       | 11.9 ms                                                | 15.1 ms: 1.27x slower                                                           |
| python_startup_no_site     | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                           |
| regex_compile              | 148 ms                                                 | 191 ms: 1.29x slower                                                            |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.53 ms: 1.29x slower                                                           |
| fannkuch                   | 417 ms                                                 | 540 ms: 1.30x slower                                                            |
| richards_super             | 51.5 ms                                                | 67.7 ms: 1.31x slower                                                           |
| richards                   | 45.8 ms                                                | 61.2 ms: 1.34x slower                                                           |
| coverage                   | 72.7 ms                                                | 97.4 ms: 1.34x slower                                                           |
| unpickle_pure_python       | 230 us                                                 | 309 us: 1.34x slower                                                            |
| nqueens                    | 83.3 ms                                                | 112 ms: 1.35x slower                                                            |
| go                         | 139 ms                                                 | 190 ms: 1.36x slower                                                            |
| scimark_monte_carlo        | 75.1 ms                                                | 102 ms: 1.36x slower                                                            |
| nbody                      | 97.0 ms                                                | 132 ms: 1.36x slower                                                            |
| pyflate                    | 482 ms                                                 | 660 ms: 1.37x slower                                                            |
| spectral_norm              | 115 ms                                                 | 162 ms: 1.41x slower                                                            |
| scimark_lu                 | 118 ms                                                 | 169 ms: 1.44x slower                                                            |
| dask                       | 372 ms                                                 | 538 ms: 1.45x slower                                                            |
| hexiom                     | 6.41 ms                                                | 10.6 ms: 1.65x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.10x slower                                                                    |

Benchmark hidden because not significant (8): pathlib, tornado_http, async_generators, json_dumps, xml_etree_parse, bench_mp_pool, asyncio_websockets, logging_silent
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.94x