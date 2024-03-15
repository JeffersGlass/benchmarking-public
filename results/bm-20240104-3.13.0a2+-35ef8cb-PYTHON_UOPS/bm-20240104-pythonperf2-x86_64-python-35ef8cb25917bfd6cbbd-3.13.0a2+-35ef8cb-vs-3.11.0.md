
# Results vs. 3.11.0

- fork: python
- ref: 35ef8cb25917bfd6cbbd
- machine: linux-x86_64
- commit hash: 35ef8cb
- commit date: 2024-01-04
- overall geometric mean: 1.02x slower
- HPT reliability: 93.56%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 311 ms: 1.08x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.82 ms: 1.01x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.93 sec: 1.03x slower                                                       |
| tornado_http   | 124 ms                                                       | 122 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 449 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 563 ms: 1.12x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 555 ms: 1.08x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 448 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 716 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 721 ms: 1.04x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 265 ms: 1.05x slower                                                         |
| float          | 74.9 ms                                                      | 102 ms: 1.36x slower                                                         |
| nbody          | 92.9 ms                                                      | 126 ms: 1.36x slower                                                         |
| Geometric mean | (ref)                                                        | 1.25x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 24.9 ms: 1.02x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.44 ms: 1.03x slower                                                        |
| regex_dna      | 227 ms                                                       | 236 ms: 1.04x slower                                                         |
| regex_compile  | 156 ms                                                       | 173 ms: 1.11x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.9 ms: 1.22x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.2 us: 1.15x faster                                                        |
| pickle_dict          | 32.3 us                                                      | 30.5 us: 1.06x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.05x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 309 us: 1.02x faster                                                         |
| unpickle_list        | 4.60 us                                                      | 4.57 us: 1.01x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 241 us: 1.01x slower                                                         |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 116 ms: 1.09x slower                                                         |
| pickle_list          | 3.94 us                                                      | 4.35 us: 1.10x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.7 us: 1.11x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 63.0 ms: 1.13x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 92.8 ms: 1.16x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.81 sec: 1.25x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 14.6 ms: 1.33x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 127 us: 4.20x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 372 ms: 2.01x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 33.8 ms: 1.62x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.0 ms: 1.26x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.9 ms: 1.22x faster                                                        |
| async_tree_none            | 518 ms                                                       | 449 ms: 1.15x faster                                                         |
| json_loads                 | 28.9 us                                                      | 25.2 us: 1.15x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 563 ms: 1.12x faster                                                         |
| sympy_sum                  | 186 ms                                                       | 169 ms: 1.10x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.79 ms: 1.09x faster                                                        |
| scimark_lu                 | 114 ms                                                       | 106 ms: 1.08x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 555 ms: 1.08x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                       |
| richards_super             | 63.6 ms                                                      | 59.6 ms: 1.07x faster                                                        |
| json                       | 5.58 ms                                                      | 5.24 ms: 1.07x faster                                                        |
| logging_simple             | 7.24 us                                                      | 6.80 us: 1.07x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 30.5 us: 1.06x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 448 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| mdp                        | 2.77 sec                                                     | 2.64 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 716 ms: 1.05x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 721 ms: 1.04x faster                                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.46 ms: 1.04x faster                                                        |
| sympy_str                  | 337 ms                                                       | 327 ms: 1.03x faster                                                         |
| raytrace                   | 309 ms                                                       | 300 ms: 1.03x faster                                                         |
| logging_format             | 7.71 us                                                      | 7.49 us: 1.03x faster                                                        |
| bench_thread_pool          | 1.00 ms                                                      | 974 us: 1.03x faster                                                         |
| deepcopy                   | 391 us                                                       | 381 us: 1.03x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 309 us: 1.02x faster                                                         |
| sympy_integrate            | 25.8 ms                                                      | 25.3 ms: 1.02x faster                                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.87 ms: 1.02x faster                                                        |
| sympy_expand               | 553 ms                                                       | 543 ms: 1.02x faster                                                         |
| asyncio_websockets         | 390 ms                                                       | 384 ms: 1.02x faster                                                         |
| tornado_http               | 124 ms                                                       | 122 ms: 1.02x faster                                                         |
| chameleon                  | 7.92 ms                                                      | 7.82 ms: 1.01x faster                                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.36 us: 1.01x faster                                                        |
| unpickle_list              | 4.60 us                                                      | 4.57 us: 1.01x faster                                                        |
| logging_silent             | 100 ns                                                       | 99.7 ns: 1.01x faster                                                        |
| unpickle_pure_python       | 238 us                                                       | 241 us: 1.01x slower                                                         |
| sqlglot_normalize          | 122 ms                                                       | 124 ms: 1.02x slower                                                         |
| pickle                     | 9.89 us                                                      | 10.1 us: 1.02x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                        |
| unpack_sequence            | 45.7 ns                                                      | 46.6 ns: 1.02x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 24.9 ms: 1.02x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.44 ms: 1.03x slower                                                        |
| chaos                      | 74.9 ms                                                      | 77.2 ms: 1.03x slower                                                        |
| docutils                   | 2.85 sec                                                     | 2.93 sec: 1.03x slower                                                       |
| create_gc_cycles           | 1.58 ms                                                      | 1.63 ms: 1.03x slower                                                        |
| crypto_pyaes               | 83.3 ms                                                      | 86.1 ms: 1.03x slower                                                        |
| regex_dna                  | 227 ms                                                       | 236 ms: 1.04x slower                                                         |
| pidigits                   | 251 ms                                                       | 265 ms: 1.05x slower                                                         |
| deepcopy_memo              | 37.5 us                                                      | 39.8 us: 1.06x slower                                                        |
| richards                   | 49.7 ms                                                      | 52.8 ms: 1.06x slower                                                        |
| nqueens                    | 103 ms                                                       | 110 ms: 1.07x slower                                                         |
| meteor_contest             | 131 ms                                                       | 140 ms: 1.07x slower                                                         |
| dulwich_log                | 67.4 ms                                                      | 72.4 ms: 1.07x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 63.6 ms: 1.08x slower                                                        |
| 2to3                       | 287 ms                                                       | 311 ms: 1.08x slower                                                         |
| xml_etree_iterparse        | 107 ms                                                       | 116 ms: 1.09x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.35 us: 1.10x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.7 us: 1.11x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.79 us: 1.11x slower                                                        |
| regex_compile              | 156 ms                                                       | 173 ms: 1.11x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 63.0 ms: 1.13x slower                                                        |
| fannkuch                   | 416 ms                                                       | 475 ms: 1.14x slower                                                         |
| go                         | 158 ms                                                       | 180 ms: 1.14x slower                                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.92 sec: 1.15x slower                                                       |
| async_generators           | 322 ms                                                       | 370 ms: 1.15x slower                                                         |
| pprint_safe_repr           | 805 ms                                                       | 929 ms: 1.16x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 92.8 ms: 1.16x slower                                                        |
| python_startup             | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                                        |
| mypy2                      | 762 ms                                                       | 893 ms: 1.17x slower                                                         |
| coverage                   | 66.1 ms                                                      | 79.9 ms: 1.21x slower                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 86.7 ms: 1.24x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.81 sec: 1.25x slower                                                       |
| telco                      | 6.81 ms                                                      | 8.49 ms: 1.25x slower                                                        |
| pyflate                    | 449 ms                                                       | 597 ms: 1.33x slower                                                         |
| mako                       | 11.0 ms                                                      | 14.6 ms: 1.33x slower                                                        |
| scimark_sor                | 110 ms                                                       | 148 ms: 1.35x slower                                                         |
| deltablue                  | 3.97 ms                                                      | 5.37 ms: 1.35x slower                                                        |
| float                      | 74.9 ms                                                      | 102 ms: 1.36x slower                                                         |
| nbody                      | 92.9 ms                                                      | 126 ms: 1.36x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 9.85 ms: 1.41x slower                                                        |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.42x slower                                                        |
| scimark_fft                | 281 ms                                                       | 429 ms: 1.53x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.52 ms: 1.60x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 172 ms: 1.80x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (4): comprehensions, dask, pycparser, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 93.56% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x