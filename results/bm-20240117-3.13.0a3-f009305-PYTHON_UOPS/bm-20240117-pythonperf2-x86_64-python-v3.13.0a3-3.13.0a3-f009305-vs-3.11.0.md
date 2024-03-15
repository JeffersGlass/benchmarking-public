
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a3
- machine: linux-x86_64
- commit hash: f009305
- commit date: 2024-01-17
- overall geometric mean: 1.02x slower
- HPT reliability: 93.71%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf2-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 308 ms: 1.08x slower                                             |
| chameleon      | 7.92 ms                                                      | 7.89 ms: 1.00x faster                                            |
| docutils       | 2.85 sec                                                     | 2.94 sec: 1.03x slower                                           |
| Geometric mean | (ref)                                                        | 1.02x slower                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf2-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 446 ms: 1.16x faster                                             |
| async_tree_memoization     | 629 ms                                                       | 558 ms: 1.13x faster                                             |
| async_tree_none_tg         | 474 ms                                                       | 442 ms: 1.07x faster                                             |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                           |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 710 ms: 1.06x faster                                             |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                           |
| async_tree_memoization_tg  | 600 ms                                                       | 570 ms: 1.05x faster                                             |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 713 ms: 1.05x faster                                             |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf2-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 265 ms: 1.05x slower                                             |
| nbody          | 92.9 ms                                                      | 125 ms: 1.35x slower                                             |
| float          | 74.9 ms                                                      | 103 ms: 1.37x slower                                             |
| Geometric mean | (ref)                                                        | 1.25x slower                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf2-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.43 ms: 1.03x slower                                            |
| regex_dna      | 227 ms                                                       | 240 ms: 1.06x slower                                             |
| regex_v8       | 24.4 ms                                                      | 26.4 ms: 1.08x slower                                            |
| regex_compile  | 156 ms                                                       | 170 ms: 1.09x slower                                             |
| Geometric mean | (ref)                                                        | 1.06x slower                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf2-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.8 ms: 1.22x faster                                            |
| json_loads           | 28.9 us                                                      | 25.1 us: 1.15x faster                                            |
| xml_etree_parse      | 155 ms                                                       | 146 ms: 1.06x faster                                             |
| pickle_dict          | 32.3 us                                                      | 30.7 us: 1.05x faster                                            |
| pickle_pure_python   | 316 us                                                       | 311 us: 1.01x faster                                             |
| unpickle_pure_python | 238 us                                                       | 245 us: 1.03x slower                                             |
| unpickle_list        | 4.60 us                                                      | 4.74 us: 1.03x slower                                            |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                            |
| xml_etree_iterparse  | 107 ms                                                       | 117 ms: 1.10x slower                                             |
| pickle_list          | 3.94 us                                                      | 4.32 us: 1.10x slower                                            |
| xml_etree_process    | 55.9 ms                                                      | 62.3 ms: 1.11x slower                                            |
| unpickle             | 13.3 us                                                      | 15.1 us: 1.14x slower                                            |
| xml_etree_generate   | 79.7 ms                                                      | 90.9 ms: 1.14x slower                                            |
| tomli_loads          | 2.25 sec                                                     | 2.82 sec: 1.25x slower                                           |
| Geometric mean       | (ref)                                                        | 1.03x slower                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf2-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                            |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                            |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf2-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 14.8 ms: 1.34x slower                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-pythonperf2-x86_64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 124 us: 4.29x faster                                             |
| asyncio_tcp                | 747 ms                                                       | 375 ms: 1.99x faster                                             |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                           |
| generators                 | 54.6 ms                                                      | 34.3 ms: 1.59x faster                                            |
| coroutines                 | 27.8 ms                                                      | 22.5 ms: 1.23x faster                                            |
| json_dumps                 | 13.3 ms                                                      | 10.8 ms: 1.22x faster                                            |
| async_tree_none            | 518 ms                                                       | 446 ms: 1.16x faster                                             |
| json_loads                 | 28.9 us                                                      | 25.1 us: 1.15x faster                                            |
| async_tree_memoization     | 629 ms                                                       | 558 ms: 1.13x faster                                             |
| sympy_sum                  | 186 ms                                                       | 166 ms: 1.12x faster                                             |
| gc_traversal               | 4.15 ms                                                      | 3.74 ms: 1.11x faster                                            |
| scimark_lu                 | 114 ms                                                       | 104 ms: 1.09x faster                                             |
| async_tree_none_tg         | 474 ms                                                       | 442 ms: 1.07x faster                                             |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                           |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 710 ms: 1.06x faster                                             |
| xml_etree_parse            | 155 ms                                                       | 146 ms: 1.06x faster                                             |
| richards_super             | 63.6 ms                                                      | 60.0 ms: 1.06x faster                                            |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                           |
| logging_simple             | 7.24 us                                                      | 6.88 us: 1.05x faster                                            |
| async_tree_memoization_tg  | 600 ms                                                       | 570 ms: 1.05x faster                                             |
| pickle_dict                | 32.3 us                                                      | 30.7 us: 1.05x faster                                            |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 713 ms: 1.05x faster                                             |
| mdp                        | 2.77 sec                                                     | 2.64 sec: 1.05x faster                                           |
| sympy_str                  | 337 ms                                                       | 322 ms: 1.05x faster                                             |
| logging_format             | 7.71 us                                                      | 7.38 us: 1.04x faster                                            |
| json                       | 5.58 ms                                                      | 5.35 ms: 1.04x faster                                            |
| sqlglot_parse              | 1.51 ms                                                      | 1.45 ms: 1.04x faster                                            |
| sympy_integrate            | 25.8 ms                                                      | 24.8 ms: 1.04x faster                                            |
| sympy_expand               | 553 ms                                                       | 534 ms: 1.03x faster                                             |
| unpack_sequence            | 45.7 ns                                                      | 44.2 ns: 1.03x faster                                            |
| bench_thread_pool          | 1.00 ms                                                      | 969 us: 1.03x faster                                             |
| deepcopy                   | 391 us                                                       | 379 us: 1.03x faster                                             |
| sqlglot_transpile          | 1.91 ms                                                      | 1.87 ms: 1.02x faster                                            |
| pickle_pure_python         | 316 us                                                       | 311 us: 1.01x faster                                             |
| logging_silent             | 100 ns                                                       | 98.9 ns: 1.01x faster                                            |
| raytrace                   | 309 ms                                                       | 305 ms: 1.01x faster                                             |
| chameleon                  | 7.92 ms                                                      | 7.89 ms: 1.00x faster                                            |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                            |
| sqlglot_normalize          | 122 ms                                                       | 124 ms: 1.02x slower                                             |
| unpickle_pure_python       | 238 us                                                       | 245 us: 1.03x slower                                             |
| regex_effbot               | 3.34 ms                                                      | 3.43 ms: 1.03x slower                                            |
| unpickle_list              | 4.60 us                                                      | 4.74 us: 1.03x slower                                            |
| docutils                   | 2.85 sec                                                     | 2.94 sec: 1.03x slower                                           |
| chaos                      | 74.9 ms                                                      | 77.4 ms: 1.03x slower                                            |
| crypto_pyaes               | 83.3 ms                                                      | 86.6 ms: 1.04x slower                                            |
| pycparser                  | 1.31 sec                                                     | 1.36 sec: 1.04x slower                                           |
| pickle                     | 9.89 us                                                      | 10.3 us: 1.04x slower                                            |
| nqueens                    | 103 ms                                                       | 108 ms: 1.05x slower                                             |
| pidigits                   | 251 ms                                                       | 265 ms: 1.05x slower                                             |
| regex_dna                  | 227 ms                                                       | 240 ms: 1.06x slower                                             |
| meteor_contest             | 131 ms                                                       | 139 ms: 1.06x slower                                             |
| dulwich_log                | 67.4 ms                                                      | 72.1 ms: 1.07x slower                                            |
| deepcopy_memo              | 37.5 us                                                      | 40.3 us: 1.07x slower                                            |
| 2to3                       | 287 ms                                                       | 308 ms: 1.08x slower                                             |
| sqlglot_optimize           | 59.0 ms                                                      | 63.6 ms: 1.08x slower                                            |
| regex_v8                   | 24.4 ms                                                      | 26.4 ms: 1.08x slower                                            |
| regex_compile              | 156 ms                                                       | 170 ms: 1.09x slower                                             |
| xml_etree_iterparse        | 107 ms                                                       | 117 ms: 1.10x slower                                             |
| pickle_list                | 3.94 us                                                      | 4.32 us: 1.10x slower                                            |
| richards                   | 49.7 ms                                                      | 54.5 ms: 1.10x slower                                            |
| sqlite_synth               | 2.52 us                                                      | 2.80 us: 1.11x slower                                            |
| xml_etree_process          | 55.9 ms                                                      | 62.3 ms: 1.11x slower                                            |
| unpickle                   | 13.3 us                                                      | 15.1 us: 1.14x slower                                            |
| pprint_pformat             | 1.67 sec                                                     | 1.90 sec: 1.14x slower                                           |
| xml_etree_generate         | 79.7 ms                                                      | 90.9 ms: 1.14x slower                                            |
| go                         | 158 ms                                                       | 180 ms: 1.14x slower                                             |
| pprint_safe_repr           | 805 ms                                                       | 921 ms: 1.14x slower                                             |
| fannkuch                   | 416 ms                                                       | 481 ms: 1.16x slower                                             |
| async_generators           | 322 ms                                                       | 372 ms: 1.16x slower                                             |
| python_startup             | 10.7 ms                                                      | 12.5 ms: 1.17x slower                                            |
| mypy2                      | 762 ms                                                       | 893 ms: 1.17x slower                                             |
| telco                      | 6.81 ms                                                      | 8.28 ms: 1.22x slower                                            |
| coverage                   | 66.1 ms                                                      | 81.8 ms: 1.24x slower                                            |
| tomli_loads                | 2.25 sec                                                     | 2.82 sec: 1.25x slower                                           |
| scimark_monte_carlo        | 69.8 ms                                                      | 88.7 ms: 1.27x slower                                            |
| pyflate                    | 449 ms                                                       | 582 ms: 1.30x slower                                             |
| scimark_sor                | 110 ms                                                       | 147 ms: 1.34x slower                                             |
| mako                       | 11.0 ms                                                      | 14.8 ms: 1.34x slower                                            |
| nbody                      | 92.9 ms                                                      | 125 ms: 1.35x slower                                             |
| deltablue                  | 3.97 ms                                                      | 5.40 ms: 1.36x slower                                            |
| float                      | 74.9 ms                                                      | 103 ms: 1.37x slower                                             |
| hexiom                     | 6.98 ms                                                      | 9.82 ms: 1.41x slower                                            |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                            |
| scimark_fft                | 281 ms                                                       | 429 ms: 1.53x slower                                             |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.49 ms: 1.60x slower                                            |
| spectral_norm              | 95.1 ms                                                      | 161 ms: 1.69x slower                                             |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                     |

Benchmark hidden because not significant (7): tornado_http, dask, comprehensions, asyncio_websockets, deepcopy_reduce, bench_mp_pool, create_gc_cycles
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 93.71% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x