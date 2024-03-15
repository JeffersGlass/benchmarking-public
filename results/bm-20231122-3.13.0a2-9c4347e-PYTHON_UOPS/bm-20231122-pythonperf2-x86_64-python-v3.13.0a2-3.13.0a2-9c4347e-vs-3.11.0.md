
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a2
- machine: linux-x86_64
- commit hash: 9c4347e
- commit date: 2023-11-22
- overall geometric mean: 1.01x slower
- HPT reliability: 89.66%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf2-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 311 ms: 1.09x slower                                             |
| docutils       | 2.85 sec                                                     | 2.93 sec: 1.03x slower                                           |
| Geometric mean | (ref)                                                        | 1.03x slower                                                     |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf2-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 447 ms: 1.16x faster                                             |
| async_tree_memoization     | 629 ms                                                       | 561 ms: 1.12x faster                                             |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                           |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 711 ms: 1.06x faster                                             |
| async_tree_none_tg         | 474 ms                                                       | 453 ms: 1.05x faster                                             |
| async_tree_io_tg           | 1.15 sec                                                     | 1.11 sec: 1.04x faster                                           |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 725 ms: 1.03x faster                                             |
| async_tree_memoization_tg  | 600 ms                                                       | 586 ms: 1.02x faster                                             |
| Geometric mean             | (ref)                                                        | 1.07x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf2-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 267 ms: 1.06x slower                                             |
| nbody          | 92.9 ms                                                      | 112 ms: 1.21x slower                                             |
| float          | 74.9 ms                                                      | 92.5 ms: 1.23x slower                                            |
| Geometric mean | (ref)                                                        | 1.17x slower                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf2-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 24.9 ms: 1.02x slower                                            |
| regex_effbot   | 3.34 ms                                                      | 3.51 ms: 1.05x slower                                            |
| regex_dna      | 227 ms                                                       | 249 ms: 1.10x slower                                             |
| regex_compile  | 156 ms                                                       | 172 ms: 1.10x slower                                             |
| Geometric mean | (ref)                                                        | 1.07x slower                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf2-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.7 ms: 1.24x faster                                            |
| json_loads           | 28.9 us                                                      | 25.3 us: 1.14x faster                                            |
| unpickle_pure_python | 238 us                                                       | 231 us: 1.03x faster                                             |
| pickle_dict          | 32.3 us                                                      | 31.8 us: 1.02x faster                                            |
| pickle_pure_python   | 316 us                                                       | 312 us: 1.01x faster                                             |
| unpickle_list        | 4.60 us                                                      | 4.56 us: 1.01x faster                                            |
| pickle               | 9.89 us                                                      | 9.98 us: 1.01x slower                                            |
| xml_etree_parse      | 155 ms                                                       | 157 ms: 1.02x slower                                             |
| pickle_list          | 3.94 us                                                      | 4.27 us: 1.08x slower                                            |
| xml_etree_process    | 55.9 ms                                                      | 60.9 ms: 1.09x slower                                            |
| xml_etree_iterparse  | 107 ms                                                       | 117 ms: 1.10x slower                                             |
| xml_etree_generate   | 79.7 ms                                                      | 90.1 ms: 1.13x slower                                            |
| unpickle             | 13.3 us                                                      | 15.2 us: 1.15x slower                                            |
| tomli_loads          | 2.25 sec                                                     | 2.61 sec: 1.16x slower                                           |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf2-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.9 ms: 1.20x slower                                            |
| python_startup_no_site | 7.73 ms                                                      | 11.3 ms: 1.47x slower                                            |
| Geometric mean         | (ref)                                                        | 1.33x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf2-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 13.6 ms: 1.24x slower                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf2-x86_64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 133 us: 3.99x faster                                             |
| asyncio_tcp                | 747 ms                                                       | 373 ms: 2.00x faster                                             |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                           |
| generators                 | 54.6 ms                                                      | 35.0 ms: 1.56x faster                                            |
| json_dumps                 | 13.3 ms                                                      | 10.7 ms: 1.24x faster                                            |
| coroutines                 | 27.8 ms                                                      | 22.6 ms: 1.23x faster                                            |
| async_tree_none            | 518 ms                                                       | 447 ms: 1.16x faster                                             |
| json_loads                 | 28.9 us                                                      | 25.3 us: 1.14x faster                                            |
| async_tree_memoization     | 629 ms                                                       | 561 ms: 1.12x faster                                             |
| sympy_sum                  | 186 ms                                                       | 167 ms: 1.11x faster                                             |
| gc_traversal               | 4.15 ms                                                      | 3.76 ms: 1.10x faster                                            |
| richards_super             | 63.6 ms                                                      | 58.4 ms: 1.09x faster                                            |
| scimark_lu                 | 114 ms                                                       | 105 ms: 1.09x faster                                             |
| comprehensions             | 25.1 us                                                      | 23.3 us: 1.07x faster                                            |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                           |
| deepcopy                   | 391 us                                                       | 366 us: 1.07x faster                                             |
| logging_simple             | 7.24 us                                                      | 6.80 us: 1.06x faster                                            |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 711 ms: 1.06x faster                                             |
| json                       | 5.58 ms                                                      | 5.30 ms: 1.05x faster                                            |
| unpack_sequence            | 45.7 ns                                                      | 43.3 ns: 1.05x faster                                            |
| mdp                        | 2.77 sec                                                     | 2.63 sec: 1.05x faster                                           |
| async_tree_none_tg         | 474 ms                                                       | 453 ms: 1.05x faster                                             |
| sympy_str                  | 337 ms                                                       | 322 ms: 1.05x faster                                             |
| logging_format             | 7.71 us                                                      | 7.40 us: 1.04x faster                                            |
| async_tree_io_tg           | 1.15 sec                                                     | 1.11 sec: 1.04x faster                                           |
| sympy_integrate            | 25.8 ms                                                      | 24.9 ms: 1.03x faster                                            |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 725 ms: 1.03x faster                                             |
| crypto_pyaes               | 83.3 ms                                                      | 80.6 ms: 1.03x faster                                            |
| raytrace                   | 309 ms                                                       | 299 ms: 1.03x faster                                             |
| sympy_expand               | 553 ms                                                       | 535 ms: 1.03x faster                                             |
| unpickle_pure_python       | 238 us                                                       | 231 us: 1.03x faster                                             |
| async_tree_memoization_tg  | 600 ms                                                       | 586 ms: 1.02x faster                                             |
| chaos                      | 74.9 ms                                                      | 73.3 ms: 1.02x faster                                            |
| sqlglot_parse              | 1.51 ms                                                      | 1.49 ms: 1.02x faster                                            |
| pickle_dict                | 32.3 us                                                      | 31.8 us: 1.02x faster                                            |
| logging_silent             | 100 ns                                                       | 98.7 ns: 1.02x faster                                            |
| deepcopy_reduce            | 3.40 us                                                      | 3.35 us: 1.01x faster                                            |
| pickle_pure_python         | 316 us                                                       | 312 us: 1.01x faster                                             |
| unpickle_list              | 4.60 us                                                      | 4.56 us: 1.01x faster                                            |
| sqlglot_transpile          | 1.91 ms                                                      | 1.90 ms: 1.01x faster                                            |
| pickle                     | 9.89 us                                                      | 9.98 us: 1.01x slower                                            |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.02x slower                                           |
| xml_etree_parse            | 155 ms                                                       | 157 ms: 1.02x slower                                             |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                            |
| sqlglot_normalize          | 122 ms                                                       | 124 ms: 1.02x slower                                             |
| regex_v8                   | 24.4 ms                                                      | 24.9 ms: 1.02x slower                                            |
| create_gc_cycles           | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                            |
| nqueens                    | 103 ms                                                       | 105 ms: 1.02x slower                                             |
| deepcopy_memo              | 37.5 us                                                      | 38.6 us: 1.03x slower                                            |
| docutils                   | 2.85 sec                                                     | 2.93 sec: 1.03x slower                                           |
| richards                   | 49.7 ms                                                      | 51.6 ms: 1.04x slower                                            |
| meteor_contest             | 131 ms                                                       | 137 ms: 1.05x slower                                             |
| regex_effbot               | 3.34 ms                                                      | 3.51 ms: 1.05x slower                                            |
| pidigits                   | 251 ms                                                       | 267 ms: 1.06x slower                                             |
| dulwich_log                | 67.4 ms                                                      | 72.0 ms: 1.07x slower                                            |
| sqlglot_optimize           | 59.0 ms                                                      | 63.2 ms: 1.07x slower                                            |
| pickle_list                | 3.94 us                                                      | 4.27 us: 1.08x slower                                            |
| 2to3                       | 287 ms                                                       | 311 ms: 1.09x slower                                             |
| pprint_pformat             | 1.67 sec                                                     | 1.81 sec: 1.09x slower                                           |
| fannkuch                   | 416 ms                                                       | 453 ms: 1.09x slower                                             |
| xml_etree_process          | 55.9 ms                                                      | 60.9 ms: 1.09x slower                                            |
| pprint_safe_repr           | 805 ms                                                       | 880 ms: 1.09x slower                                             |
| regex_dna                  | 227 ms                                                       | 249 ms: 1.10x slower                                             |
| xml_etree_iterparse        | 107 ms                                                       | 117 ms: 1.10x slower                                             |
| regex_compile              | 156 ms                                                       | 172 ms: 1.10x slower                                             |
| sqlite_synth               | 2.52 us                                                      | 2.83 us: 1.12x slower                                            |
| xml_etree_generate         | 79.7 ms                                                      | 90.1 ms: 1.13x slower                                            |
| go                         | 158 ms                                                       | 179 ms: 1.14x slower                                             |
| unpickle                   | 13.3 us                                                      | 15.2 us: 1.15x slower                                            |
| tomli_loads                | 2.25 sec                                                     | 2.61 sec: 1.16x slower                                           |
| mypy2                      | 762 ms                                                       | 893 ms: 1.17x slower                                             |
| async_generators           | 322 ms                                                       | 377 ms: 1.17x slower                                             |
| coverage                   | 66.1 ms                                                      | 78.8 ms: 1.19x slower                                            |
| python_startup             | 10.7 ms                                                      | 12.9 ms: 1.20x slower                                            |
| nbody                      | 92.9 ms                                                      | 112 ms: 1.21x slower                                             |
| float                      | 74.9 ms                                                      | 92.5 ms: 1.23x slower                                            |
| pyflate                    | 449 ms                                                       | 557 ms: 1.24x slower                                             |
| mako                       | 11.0 ms                                                      | 13.6 ms: 1.24x slower                                            |
| telco                      | 6.81 ms                                                      | 8.47 ms: 1.24x slower                                            |
| scimark_monte_carlo        | 69.8 ms                                                      | 87.4 ms: 1.25x slower                                            |
| deltablue                  | 3.97 ms                                                      | 4.98 ms: 1.25x slower                                            |
| hexiom                     | 6.98 ms                                                      | 9.10 ms: 1.30x slower                                            |
| scimark_sor                | 110 ms                                                       | 149 ms: 1.36x slower                                             |
| scimark_fft                | 281 ms                                                       | 407 ms: 1.45x slower                                             |
| python_startup_no_site     | 7.73 ms                                                      | 11.3 ms: 1.47x slower                                            |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.01 ms: 1.48x slower                                            |
| spectral_norm              | 95.1 ms                                                      | 144 ms: 1.51x slower                                             |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                     |

Benchmark hidden because not significant (6): bench_thread_pool, asyncio_websockets, tornado_http, chameleon, dask, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 89.66% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.97x