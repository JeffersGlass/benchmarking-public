
# Results vs. 3.11.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.02x slower
- HPT reliability: 95.39%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 310 ms: 1.08x slower                                                         |
| chameleon      | 7.92 ms                                                      | 8.01 ms: 1.01x slower                                                        |
| docutils       | 2.85 sec                                                     | 2.95 sec: 1.04x slower                                                       |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 449 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 562 ms: 1.12x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 445 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 567 ms: 1.06x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 714 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 718 ms: 1.04x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 265 ms: 1.06x slower                                                         |
| float          | 74.9 ms                                                      | 103 ms: 1.38x slower                                                         |
| nbody          | 92.9 ms                                                      | 128 ms: 1.38x slower                                                         |
| Geometric mean | (ref)                                                        | 1.26x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.51 ms: 1.05x slower                                                        |
| regex_dna      | 227 ms                                                       | 239 ms: 1.05x slower                                                         |
| regex_v8       | 24.4 ms                                                      | 25.9 ms: 1.06x slower                                                        |
| regex_compile  | 156 ms                                                       | 173 ms: 1.11x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 11.0 ms: 1.21x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.7 us: 1.17x faster                                                        |
| pickle_dict          | 32.3 us                                                      | 31.2 us: 1.04x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 150 ms: 1.03x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.01x faster                                                         |
| unpickle_pure_python | 238 us                                                       | 241 us: 1.01x slower                                                         |
| unpickle_list        | 4.60 us                                                      | 4.68 us: 1.02x slower                                                        |
| pickle               | 9.89 us                                                      | 10.2 us: 1.04x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 116 ms: 1.09x slower                                                         |
| unpickle             | 13.3 us                                                      | 14.6 us: 1.10x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 62.7 ms: 1.12x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 92.1 ms: 1.16x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.57 us: 1.16x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.77 sec: 1.23x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.17x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 15.0 ms: 1.37x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-pythonperf2-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 129 us: 4.11x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 375 ms: 1.99x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.1 ms: 1.60x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.2 ms: 1.25x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 11.0 ms: 1.21x faster                                                        |
| json_loads                 | 28.9 us                                                      | 24.7 us: 1.17x faster                                                        |
| async_tree_none            | 518 ms                                                       | 449 ms: 1.15x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 562 ms: 1.12x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.74 ms: 1.11x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 170 ms: 1.09x faster                                                         |
| scimark_lu                 | 114 ms                                                       | 105 ms: 1.09x faster                                                         |
| richards_super             | 63.6 ms                                                      | 58.7 ms: 1.08x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                       |
| json                       | 5.58 ms                                                      | 5.20 ms: 1.07x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 445 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 567 ms: 1.06x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.85 us: 1.06x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.63 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 714 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 718 ms: 1.04x faster                                                         |
| deepcopy                   | 391 us                                                       | 375 us: 1.04x faster                                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.45 ms: 1.04x faster                                                        |
| unpack_sequence            | 45.7 ns                                                      | 44.0 ns: 1.04x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.44 us: 1.04x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 31.2 us: 1.04x faster                                                        |
| sympy_str                  | 337 ms                                                       | 326 ms: 1.03x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 150 ms: 1.03x faster                                                         |
| raytrace                   | 309 ms                                                       | 301 ms: 1.03x faster                                                         |
| bench_thread_pool          | 1.00 ms                                                      | 977 us: 1.02x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.87 ms: 1.02x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 25.3 ms: 1.02x faster                                                        |
| sympy_expand               | 553 ms                                                       | 543 ms: 1.02x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.01x faster                                                         |
| comprehensions             | 25.1 us                                                      | 24.9 us: 1.01x faster                                                        |
| dask                       | 410 ms                                                       | 414 ms: 1.01x slower                                                         |
| unpickle_pure_python       | 238 us                                                       | 241 us: 1.01x slower                                                         |
| chameleon                  | 7.92 ms                                                      | 8.01 ms: 1.01x slower                                                        |
| pycparser                  | 1.31 sec                                                     | 1.32 sec: 1.01x slower                                                       |
| chaos                      | 74.9 ms                                                      | 76.0 ms: 1.01x slower                                                        |
| unpickle_list              | 4.60 us                                                      | 4.68 us: 1.02x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                        |
| create_gc_cycles           | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                                        |
| sqlglot_normalize          | 122 ms                                                       | 125 ms: 1.02x slower                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 86.1 ms: 1.03x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.2 us: 1.04x slower                                                        |
| docutils                   | 2.85 sec                                                     | 2.95 sec: 1.04x slower                                                       |
| nqueens                    | 103 ms                                                       | 107 ms: 1.05x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.51 ms: 1.05x slower                                                        |
| regex_dna                  | 227 ms                                                       | 239 ms: 1.05x slower                                                         |
| pidigits                   | 251 ms                                                       | 265 ms: 1.06x slower                                                         |
| regex_v8                   | 24.4 ms                                                      | 25.9 ms: 1.06x slower                                                        |
| meteor_contest             | 131 ms                                                       | 139 ms: 1.06x slower                                                         |
| richards                   | 49.7 ms                                                      | 52.9 ms: 1.06x slower                                                        |
| deepcopy_memo              | 37.5 us                                                      | 40.1 us: 1.07x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 72.4 ms: 1.07x slower                                                        |
| 2to3                       | 287 ms                                                       | 310 ms: 1.08x slower                                                         |
| sqlglot_optimize           | 59.0 ms                                                      | 63.8 ms: 1.08x slower                                                        |
| xml_etree_iterparse        | 107 ms                                                       | 116 ms: 1.09x slower                                                         |
| unpickle                   | 13.3 us                                                      | 14.6 us: 1.10x slower                                                        |
| regex_compile              | 156 ms                                                       | 173 ms: 1.11x slower                                                         |
| sqlite_synth               | 2.52 us                                                      | 2.82 us: 1.12x slower                                                        |
| xml_etree_process          | 55.9 ms                                                      | 62.7 ms: 1.12x slower                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.89 sec: 1.13x slower                                                       |
| fannkuch                   | 416 ms                                                       | 473 ms: 1.14x slower                                                         |
| pprint_safe_repr           | 805 ms                                                       | 915 ms: 1.14x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 92.1 ms: 1.16x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.57 us: 1.16x slower                                                        |
| async_generators           | 322 ms                                                       | 374 ms: 1.16x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.17x slower                                                        |
| mypy2                      | 762 ms                                                       | 895 ms: 1.17x slower                                                         |
| go                         | 158 ms                                                       | 187 ms: 1.18x slower                                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 85.8 ms: 1.23x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.77 sec: 1.23x slower                                                       |
| telco                      | 6.81 ms                                                      | 8.41 ms: 1.24x slower                                                        |
| pyflate                    | 449 ms                                                       | 574 ms: 1.28x slower                                                         |
| coverage                   | 66.1 ms                                                      | 85.7 ms: 1.30x slower                                                        |
| scimark_sor                | 110 ms                                                       | 148 ms: 1.35x slower                                                         |
| mako                       | 11.0 ms                                                      | 15.0 ms: 1.37x slower                                                        |
| float                      | 74.9 ms                                                      | 103 ms: 1.38x slower                                                         |
| nbody                      | 92.9 ms                                                      | 128 ms: 1.38x slower                                                         |
| deltablue                  | 3.97 ms                                                      | 5.49 ms: 1.38x slower                                                        |
| hexiom                     | 6.98 ms                                                      | 9.85 ms: 1.41x slower                                                        |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                                        |
| scimark_fft                | 281 ms                                                       | 423 ms: 1.51x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.37 ms: 1.57x slower                                                        |
| spectral_norm              | 95.1 ms                                                      | 164 ms: 1.73x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (5): tornado_http, asyncio_websockets, bench_mp_pool, deepcopy_reduce, logging_silent
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 95.39% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x