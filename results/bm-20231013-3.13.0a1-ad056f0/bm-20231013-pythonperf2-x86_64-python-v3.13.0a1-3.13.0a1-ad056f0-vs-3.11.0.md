
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a1
- machine: linux-x86_64
- commit hash: ad056f0
- commit date: 2023-10-13
- overall geometric mean: 1.04x faster \*
- HPT reliability: 97.15%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf2-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 297 ms: 1.04x slower                                             |
| chameleon      | 7.92 ms                                                      | 7.78 ms: 1.02x faster                                            |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                           |
| tornado_http   | 124 ms                                                       | 121 ms: 1.03x faster                                             |
| Geometric mean | (ref)                                                        | 1.00x slower                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf2-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 439 ms: 1.18x faster                                             |
| async_tree_memoization     | 629 ms                                                       | 557 ms: 1.13x faster                                             |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                           |
| async_tree_none_tg         | 474 ms                                                       | 447 ms: 1.06x faster                                             |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 713 ms: 1.06x faster                                             |
| async_tree_memoization_tg  | 600 ms                                                       | 571 ms: 1.05x faster                                             |
| async_tree_io_tg           | 1.15 sec                                                     | 1.11 sec: 1.04x faster                                           |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 727 ms: 1.03x faster                                             |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf2-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 87.7 ms: 1.06x faster                                            |
| pidigits       | 251 ms                                                       | 264 ms: 1.05x slower                                             |
| float          | 74.9 ms                                                      | 81.5 ms: 1.09x slower                                            |
| Geometric mean | (ref)                                                        | 1.03x slower                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf2-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 150 ms: 1.04x faster                                             |
| regex_dna      | 227 ms                                                       | 241 ms: 1.06x slower                                             |
| regex_effbot   | 3.34 ms                                                      | 3.55 ms: 1.06x slower                                            |
| regex_v8       | 24.4 ms                                                      | 26.2 ms: 1.07x slower                                            |
| Geometric mean | (ref)                                                        | 1.04x slower                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf2-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                            |
| json_loads           | 28.9 us                                                      | 24.3 us: 1.19x faster                                            |
| unpickle_pure_python | 238 us                                                       | 220 us: 1.08x faster                                             |
| xml_etree_parse      | 155 ms                                                       | 152 ms: 1.02x faster                                             |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.01x faster                                             |
| pickle_dict          | 32.3 us                                                      | 32.9 us: 1.02x slower                                            |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                            |
| xml_etree_iterparse  | 107 ms                                                       | 110 ms: 1.03x slower                                             |
| xml_etree_process    | 55.9 ms                                                      | 59.9 ms: 1.07x slower                                            |
| unpickle             | 13.3 us                                                      | 14.3 us: 1.08x slower                                            |
| xml_etree_generate   | 79.7 ms                                                      | 87.3 ms: 1.10x slower                                            |
| pickle_list          | 3.94 us                                                      | 4.45 us: 1.13x slower                                            |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                     |

Benchmark hidden because not significant (2): tomli_loads, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf2-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 8.70 ms: 1.13x slower                                            |
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                            |
| Geometric mean         | (ref)                                                        | 1.15x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf2-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf2-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 155 us: 3.44x faster                                             |
| asyncio_tcp                | 747 ms                                                       | 367 ms: 2.04x faster                                             |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.94x faster                                           |
| generators                 | 54.6 ms                                                      | 35.4 ms: 1.55x faster                                            |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                            |
| coroutines                 | 27.8 ms                                                      | 22.6 ms: 1.23x faster                                            |
| chaos                      | 74.9 ms                                                      | 62.7 ms: 1.19x faster                                            |
| json_loads                 | 28.9 us                                                      | 24.3 us: 1.19x faster                                            |
| async_tree_none            | 518 ms                                                       | 439 ms: 1.18x faster                                             |
| comprehensions             | 25.1 us                                                      | 21.5 us: 1.16x faster                                            |
| sympy_sum                  | 186 ms                                                       | 161 ms: 1.15x faster                                             |
| nqueens                    | 103 ms                                                       | 89.2 ms: 1.15x faster                                            |
| crypto_pyaes               | 83.3 ms                                                      | 73.4 ms: 1.13x faster                                            |
| async_tree_memoization     | 629 ms                                                       | 557 ms: 1.13x faster                                             |
| raytrace                   | 309 ms                                                       | 276 ms: 1.12x faster                                             |
| sympy_expand               | 553 ms                                                       | 494 ms: 1.12x faster                                             |
| scimark_lu                 | 114 ms                                                       | 103 ms: 1.11x faster                                             |
| mdp                        | 2.77 sec                                                     | 2.52 sec: 1.10x faster                                           |
| sympy_str                  | 337 ms                                                       | 307 ms: 1.10x faster                                             |
| json                       | 5.58 ms                                                      | 5.12 ms: 1.09x faster                                            |
| deltablue                  | 3.97 ms                                                      | 3.66 ms: 1.09x faster                                            |
| unpickle_pure_python       | 238 us                                                       | 220 us: 1.08x faster                                             |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                           |
| logging_simple             | 7.24 us                                                      | 6.79 us: 1.07x faster                                            |
| hexiom                     | 6.98 ms                                                      | 6.54 ms: 1.07x faster                                            |
| sympy_integrate            | 25.8 ms                                                      | 24.2 ms: 1.07x faster                                            |
| sqlglot_parse              | 1.51 ms                                                      | 1.42 ms: 1.06x faster                                            |
| async_tree_none_tg         | 474 ms                                                       | 447 ms: 1.06x faster                                             |
| mako                       | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                            |
| nbody                      | 92.9 ms                                                      | 87.7 ms: 1.06x faster                                            |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 713 ms: 1.06x faster                                             |
| async_tree_memoization_tg  | 600 ms                                                       | 571 ms: 1.05x faster                                             |
| fannkuch                   | 416 ms                                                       | 396 ms: 1.05x faster                                             |
| gc_traversal               | 4.15 ms                                                      | 3.95 ms: 1.05x faster                                            |
| sqlglot_normalize          | 122 ms                                                       | 117 ms: 1.04x faster                                             |
| sqlglot_transpile          | 1.91 ms                                                      | 1.83 ms: 1.04x faster                                            |
| async_tree_io_tg           | 1.15 sec                                                     | 1.11 sec: 1.04x faster                                           |
| bench_thread_pool          | 1.00 ms                                                      | 961 us: 1.04x faster                                             |
| regex_compile              | 156 ms                                                       | 150 ms: 1.04x faster                                             |
| logging_format             | 7.71 us                                                      | 7.44 us: 1.04x faster                                            |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 727 ms: 1.03x faster                                             |
| deepcopy                   | 391 us                                                       | 379 us: 1.03x faster                                             |
| richards_super             | 63.6 ms                                                      | 61.7 ms: 1.03x faster                                            |
| spectral_norm              | 95.1 ms                                                      | 92.3 ms: 1.03x faster                                            |
| tornado_http               | 124 ms                                                       | 121 ms: 1.03x faster                                             |
| logging_silent             | 100 ns                                                       | 98.3 ns: 1.02x faster                                            |
| chameleon                  | 7.92 ms                                                      | 7.78 ms: 1.02x faster                                            |
| xml_etree_parse            | 155 ms                                                       | 152 ms: 1.02x faster                                             |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.01x faster                                             |
| meteor_contest             | 131 ms                                                       | 131 ms: 1.00x slower                                             |
| docutils                   | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                           |
| pprint_pformat             | 1.67 sec                                                     | 1.68 sec: 1.01x slower                                           |
| scimark_monte_carlo        | 69.8 ms                                                      | 71.0 ms: 1.02x slower                                            |
| pickle_dict                | 32.3 us                                                      | 32.9 us: 1.02x slower                                            |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.02x slower                                           |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                            |
| pickle                     | 9.89 us                                                      | 10.1 us: 1.02x slower                                            |
| dulwich_log                | 67.4 ms                                                      | 69.2 ms: 1.03x slower                                            |
| deepcopy_memo              | 37.5 us                                                      | 38.6 us: 1.03x slower                                            |
| pprint_safe_repr           | 805 ms                                                       | 829 ms: 1.03x slower                                             |
| xml_etree_iterparse        | 107 ms                                                       | 110 ms: 1.03x slower                                             |
| 2to3                       | 287 ms                                                       | 297 ms: 1.04x slower                                             |
| pidigits                   | 251 ms                                                       | 264 ms: 1.05x slower                                             |
| regex_dna                  | 227 ms                                                       | 241 ms: 1.06x slower                                             |
| regex_effbot               | 3.34 ms                                                      | 3.55 ms: 1.06x slower                                            |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.34 ms: 1.07x slower                                            |
| regex_v8                   | 24.4 ms                                                      | 26.2 ms: 1.07x slower                                            |
| sqlite_synth               | 2.52 us                                                      | 2.70 us: 1.07x slower                                            |
| xml_etree_process          | 55.9 ms                                                      | 59.9 ms: 1.07x slower                                            |
| unpickle                   | 13.3 us                                                      | 14.3 us: 1.08x slower                                            |
| float                      | 74.9 ms                                                      | 81.5 ms: 1.09x slower                                            |
| go                         | 158 ms                                                       | 172 ms: 1.09x slower                                             |
| xml_etree_generate         | 79.7 ms                                                      | 87.3 ms: 1.10x slower                                            |
| unpack_sequence            | 45.7 ns                                                      | 50.9 ns: 1.11x slower                                            |
| richards                   | 49.7 ms                                                      | 55.4 ms: 1.12x slower                                            |
| scimark_fft                | 281 ms                                                       | 315 ms: 1.12x slower                                             |
| python_startup_no_site     | 7.73 ms                                                      | 8.70 ms: 1.13x slower                                            |
| pickle_list                | 3.94 us                                                      | 4.45 us: 1.13x slower                                            |
| pyflate                    | 449 ms                                                       | 513 ms: 1.14x slower                                             |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                            |
| telco                      | 6.81 ms                                                      | 8.25 ms: 1.21x slower                                            |
| async_generators           | 322 ms                                                       | 399 ms: 1.24x slower                                             |
| coverage                   | 66.1 ms                                                      | 83.6 ms: 1.26x slower                                            |
| scimark_sor                | 110 ms                                                       | 149 ms: 1.36x slower                                             |
| Geometric mean             | (ref)                                                        | 1.04x faster                                                     |

Benchmark hidden because not significant (7): tomli_loads, asyncio_websockets, sqlglot_optimize, deepcopy_reduce, create_gc_cycles, unpickle_list, bench_mp_pool
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 97.15% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x