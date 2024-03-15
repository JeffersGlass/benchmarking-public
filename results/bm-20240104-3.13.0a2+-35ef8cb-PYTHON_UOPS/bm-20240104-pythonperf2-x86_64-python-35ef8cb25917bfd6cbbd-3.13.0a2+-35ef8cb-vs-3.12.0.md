
# Results vs. 3.12.0

- fork: python
- ref: 35ef8cb25917bfd6cbbd
- machine: linux-x86_64
- commit hash: 35ef8cb
- commit date: 2024-01-04
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 311 ms: 1.09x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.82 ms: 1.08x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.93 sec: 1.02x slower                                                       |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 540 ms                                                       | 555 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 716 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 721 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 563 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 448 ms: 1.04x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 102 ms: 1.33x slower                                                         |
| nbody          | 88.0 ms                                                      | 126 ms: 1.44x slower                                                         |
| Geometric mean | (ref)                                                        | 1.24x slower                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.44 ms: 1.04x faster                                                        |
| regex_dna      | 239 ms                                                       | 236 ms: 1.01x faster                                                         |
| regex_v8       | 23.6 ms                                                      | 24.9 ms: 1.05x slower                                                        |
| regex_compile  | 144 ms                                                       | 173 ms: 1.20x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.5 us: 1.07x faster                                                        |
| pickle               | 10.5 us                                                      | 10.1 us: 1.05x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 309 us: 1.03x faster                                                         |
| unpickle_list        | 4.66 us                                                      | 4.57 us: 1.02x faster                                                        |
| pickle_list          | 4.43 us                                                      | 4.35 us: 1.02x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.7 us: 1.01x faster                                                        |
| xml_etree_parse      | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| json_loads           | 24.4 us                                                      | 25.2 us: 1.03x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.9 ms: 1.06x slower                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 92.8 ms: 1.08x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 63.0 ms: 1.08x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| unpickle_pure_python | 210 us                                                       | 241 us: 1.15x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.81 sec: 1.30x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.5 ms: 1.08x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.17x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 14.6 ms: 1.46x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 127 us: 1.20x faster                                                         |
| unpack_sequence            | 53.2 ns                                                      | 46.6 ns: 1.14x faster                                                        |
| generators                 | 37.4 ms                                                      | 33.8 ms: 1.11x faster                                                        |
| pickle_dict                | 32.5 us                                                      | 30.5 us: 1.07x faster                                                        |
| async_generators           | 390 ms                                                       | 370 ms: 1.06x faster                                                         |
| pickle                     | 10.5 us                                                      | 10.1 us: 1.05x faster                                                        |
| coroutines                 | 23.0 ms                                                      | 22.0 ms: 1.05x faster                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.44 ms: 1.04x faster                                                        |
| pickle_pure_python         | 318 us                                                       | 309 us: 1.03x faster                                                         |
| unpickle_list              | 4.66 us                                                      | 4.57 us: 1.02x faster                                                        |
| pickle_list                | 4.43 us                                                      | 4.35 us: 1.02x faster                                                        |
| asyncio_tcp                | 378 ms                                                       | 372 ms: 1.02x faster                                                         |
| regex_dna                  | 239 ms                                                       | 236 ms: 1.01x faster                                                         |
| asyncio_websockets         | 387 ms                                                       | 384 ms: 1.01x faster                                                         |
| unpickle                   | 14.8 us                                                      | 14.7 us: 1.01x faster                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.79 us: 1.01x slower                                                        |
| raytrace                   | 298 ms                                                       | 300 ms: 1.01x slower                                                         |
| logging_simple             | 6.71 us                                                      | 6.80 us: 1.01x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                        |
| create_gc_cycles           | 1.59 ms                                                      | 1.63 ms: 1.02x slower                                                        |
| docutils                   | 2.87 sec                                                     | 2.93 sec: 1.02x slower                                                       |
| json                       | 5.12 ms                                                      | 5.24 ms: 1.02x slower                                                        |
| bench_thread_pool          | 950 us                                                       | 974 us: 1.03x slower                                                         |
| mdp                        | 2.57 sec                                                     | 2.64 sec: 1.03x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 555 ms: 1.03x slower                                                         |
| xml_etree_parse            | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 716 ms: 1.03x slower                                                         |
| json_loads                 | 24.4 us                                                      | 25.2 us: 1.03x slower                                                        |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 721 ms: 1.03x slower                                                         |
| deepcopy                   | 368 us                                                       | 381 us: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 563 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 448 ms: 1.04x slower                                                         |
| sympy_sum                  | 162 ms                                                       | 169 ms: 1.04x slower                                                         |
| dask                       | 392 ms                                                       | 409 ms: 1.04x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                       |
| regex_v8                   | 23.6 ms                                                      | 24.9 ms: 1.05x slower                                                        |
| sqlglot_transpile          | 1.78 ms                                                      | 1.87 ms: 1.06x slower                                                        |
| sympy_integrate            | 23.9 ms                                                      | 25.3 ms: 1.06x slower                                                        |
| logging_silent             | 94.4 ns                                                      | 99.7 ns: 1.06x slower                                                        |
| sqlglot_parse              | 1.38 ms                                                      | 1.46 ms: 1.06x slower                                                        |
| json_dumps                 | 10.2 ms                                                      | 10.9 ms: 1.06x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                                       |
| sqlglot_normalize          | 116 ms                                                       | 124 ms: 1.07x slower                                                         |
| scimark_lu                 | 98.8 ms                                                      | 106 ms: 1.07x slower                                                         |
| crypto_pyaes               | 80.3 ms                                                      | 86.1 ms: 1.07x slower                                                        |
| mypy2                      | 830 ms                                                       | 893 ms: 1.08x slower                                                         |
| xml_etree_generate         | 86.1 ms                                                      | 92.8 ms: 1.08x slower                                                        |
| python_startup             | 11.6 ms                                                      | 12.5 ms: 1.08x slower                                                        |
| xml_etree_process          | 58.4 ms                                                      | 63.0 ms: 1.08x slower                                                        |
| sympy_str                  | 302 ms                                                       | 327 ms: 1.08x slower                                                         |
| chameleon                  | 7.23 ms                                                      | 7.82 ms: 1.08x slower                                                        |
| deepcopy_memo              | 36.8 us                                                      | 39.8 us: 1.08x slower                                                        |
| meteor_contest             | 128 ms                                                       | 140 ms: 1.09x slower                                                         |
| gc_traversal               | 3.48 ms                                                      | 3.79 ms: 1.09x slower                                                        |
| 2to3                       | 285 ms                                                       | 311 ms: 1.09x slower                                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 63.6 ms: 1.11x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 72.4 ms: 1.11x slower                                                        |
| sympy_expand               | 484 ms                                                       | 543 ms: 1.12x slower                                                         |
| xml_etree_iterparse        | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| comprehensions             | 21.9 us                                                      | 25.0 us: 1.14x slower                                                        |
| unpickle_pure_python       | 210 us                                                       | 241 us: 1.15x slower                                                         |
| pprint_safe_repr           | 807 ms                                                       | 929 ms: 1.15x slower                                                         |
| richards                   | 45.7 ms                                                      | 52.8 ms: 1.15x slower                                                        |
| pprint_pformat             | 1.65 sec                                                     | 1.92 sec: 1.16x slower                                                       |
| richards_super             | 51.3 ms                                                      | 59.6 ms: 1.16x slower                                                        |
| coverage                   | 66.7 ms                                                      | 79.9 ms: 1.20x slower                                                        |
| regex_compile              | 144 ms                                                       | 173 ms: 1.20x slower                                                         |
| go                         | 150 ms                                                       | 180 ms: 1.20x slower                                                         |
| chaos                      | 64.0 ms                                                      | 77.2 ms: 1.21x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 110 ms: 1.22x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.49 ms: 1.22x slower                                                        |
| scimark_monte_carlo        | 69.0 ms                                                      | 86.7 ms: 1.26x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.81 sec: 1.30x slower                                                       |
| float                      | 76.6 ms                                                      | 102 ms: 1.33x slower                                                         |
| scimark_sor                | 109 ms                                                       | 148 ms: 1.35x slower                                                         |
| fannkuch                   | 350 ms                                                       | 475 ms: 1.36x slower                                                         |
| pyflate                    | 439 ms                                                       | 597 ms: 1.36x slower                                                         |
| scimark_fft                | 301 ms                                                       | 429 ms: 1.42x slower                                                         |
| nbody                      | 88.0 ms                                                      | 126 ms: 1.44x slower                                                         |
| mako                       | 10.0 ms                                                      | 14.6 ms: 1.46x slower                                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.52 ms: 1.55x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 9.85 ms: 1.65x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 5.37 ms: 1.66x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 172 ms: 1.87x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.10x slower                                                                 |

Benchmark hidden because not significant (7): async_tree_none, deepcopy_reduce, bench_mp_pool, pidigits, asyncio_tcp_ssl, logging_format, tornado_http
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.88x