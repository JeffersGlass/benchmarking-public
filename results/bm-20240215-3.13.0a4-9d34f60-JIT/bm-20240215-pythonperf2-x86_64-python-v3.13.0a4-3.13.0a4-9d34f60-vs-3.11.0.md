# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a4
- machine: linux-x86_64
- commit hash: 9d34f60
- commit date: 2024-02-15
- overall geometric mean: 1.03x faster \*
- HPT reliability: 74.07%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 300 ms: 1.04x slower                                             |
| chameleon      | 7.92 ms                                                      | 7.14 ms: 1.11x faster                                            |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                           |
| tornado_http   | 124 ms                                                       | 126 ms: 1.01x slower                                             |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                             |
| async_tree_memoization     | 629 ms                                                       | 548 ms: 1.15x faster                                             |
| async_tree_memoization_tg  | 600 ms                                                       | 549 ms: 1.09x faster                                             |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                           |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                             |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 701 ms: 1.07x faster                                             |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                           |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 706 ms: 1.06x faster                                             |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                             |
| float          | 74.9 ms                                                      | 80.7 ms: 1.08x slower                                            |
| nbody          | 92.9 ms                                                      | 106 ms: 1.14x slower                                             |
| Geometric mean | (ref)                                                        | 1.09x slower                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 145 ms: 1.07x faster                                             |
| regex_v8       | 24.4 ms                                                      | 25.0 ms: 1.02x slower                                            |
| regex_effbot   | 3.34 ms                                                      | 3.53 ms: 1.06x slower                                            |
| regex_dna      | 227 ms                                                       | 244 ms: 1.07x slower                                             |
| Geometric mean | (ref)                                                        | 1.02x slower                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                            |
| json_loads           | 28.9 us                                                      | 25.6 us: 1.13x faster                                            |
| pickle_dict          | 32.3 us                                                      | 30.6 us: 1.06x faster                                            |
| xml_etree_parse      | 155 ms                                                       | 148 ms: 1.04x faster                                             |
| pickle_pure_python   | 316 us                                                       | 304 us: 1.04x faster                                             |
| unpickle_pure_python | 238 us                                                       | 230 us: 1.04x faster                                             |
| xml_etree_iterparse  | 107 ms                                                       | 103 ms: 1.03x faster                                             |
| unpickle_list        | 4.60 us                                                      | 4.67 us: 1.01x slower                                            |
| tomli_loads          | 2.25 sec                                                     | 2.31 sec: 1.03x slower                                           |
| xml_etree_process    | 55.9 ms                                                      | 57.6 ms: 1.03x slower                                            |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                            |
| xml_etree_generate   | 79.7 ms                                                      | 83.4 ms: 1.05x slower                                            |
| pickle_list          | 3.94 us                                                      | 4.50 us: 1.14x slower                                            |
| unpickle             | 13.3 us                                                      | 15.3 us: 1.15x slower                                            |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                            |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                            |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 11.8 ms: 1.07x slower                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf2-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 117 us: 4.54x faster                                             |
| asyncio_tcp                | 747 ms                                                       | 374 ms: 2.00x faster                                             |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.95x faster                                           |
| generators                 | 54.6 ms                                                      | 34.0 ms: 1.61x faster                                            |
| comprehensions             | 25.1 us                                                      | 19.3 us: 1.30x faster                                            |
| json_dumps                 | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                            |
| coroutines                 | 27.8 ms                                                      | 22.3 ms: 1.25x faster                                            |
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                             |
| gc_traversal               | 4.15 ms                                                      | 3.47 ms: 1.19x faster                                            |
| sympy_sum                  | 186 ms                                                       | 158 ms: 1.18x faster                                             |
| scimark_lu                 | 114 ms                                                       | 99.3 ms: 1.15x faster                                            |
| async_tree_memoization     | 629 ms                                                       | 548 ms: 1.15x faster                                             |
| json_loads                 | 28.9 us                                                      | 25.6 us: 1.13x faster                                            |
| sympy_str                  | 337 ms                                                       | 298 ms: 1.13x faster                                             |
| raytrace                   | 309 ms                                                       | 274 ms: 1.13x faster                                             |
| logging_simple             | 7.24 us                                                      | 6.51 us: 1.11x faster                                            |
| chameleon                  | 7.92 ms                                                      | 7.14 ms: 1.11x faster                                            |
| richards_super             | 63.6 ms                                                      | 57.6 ms: 1.10x faster                                            |
| sympy_expand               | 553 ms                                                       | 502 ms: 1.10x faster                                             |
| mdp                        | 2.77 sec                                                     | 2.53 sec: 1.09x faster                                           |
| async_tree_memoization_tg  | 600 ms                                                       | 549 ms: 1.09x faster                                             |
| sqlglot_parse              | 1.51 ms                                                      | 1.39 ms: 1.09x faster                                            |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                           |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                             |
| sympy_integrate            | 25.8 ms                                                      | 23.9 ms: 1.08x faster                                            |
| chaos                      | 74.9 ms                                                      | 69.4 ms: 1.08x faster                                            |
| deltablue                  | 3.97 ms                                                      | 3.69 ms: 1.08x faster                                            |
| nqueens                    | 103 ms                                                       | 95.4 ms: 1.08x faster                                            |
| regex_compile              | 156 ms                                                       | 145 ms: 1.07x faster                                             |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 701 ms: 1.07x faster                                             |
| logging_format             | 7.71 us                                                      | 7.20 us: 1.07x faster                                            |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.07x faster                                           |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 706 ms: 1.06x faster                                             |
| pickle_dict                | 32.3 us                                                      | 30.6 us: 1.06x faster                                            |
| deepcopy                   | 391 us                                                       | 370 us: 1.06x faster                                             |
| sqlglot_transpile          | 1.91 ms                                                      | 1.82 ms: 1.05x faster                                            |
| crypto_pyaes               | 83.3 ms                                                      | 79.3 ms: 1.05x faster                                            |
| json                       | 5.58 ms                                                      | 5.35 ms: 1.04x faster                                            |
| xml_etree_parse            | 155 ms                                                       | 148 ms: 1.04x faster                                             |
| sqlglot_normalize          | 122 ms                                                       | 117 ms: 1.04x faster                                             |
| pickle_pure_python         | 316 us                                                       | 304 us: 1.04x faster                                             |
| unpickle_pure_python       | 238 us                                                       | 230 us: 1.04x faster                                             |
| bench_thread_pool          | 1.00 ms                                                      | 967 us: 1.03x faster                                             |
| xml_etree_iterparse        | 107 ms                                                       | 103 ms: 1.03x faster                                             |
| logging_silent             | 100 ns                                                       | 97.7 ns: 1.03x faster                                            |
| create_gc_cycles           | 1.58 ms                                                      | 1.55 ms: 1.02x faster                                            |
| deepcopy_reduce            | 3.40 us                                                      | 3.33 us: 1.02x faster                                            |
| deepcopy_memo              | 37.5 us                                                      | 36.9 us: 1.02x faster                                            |
| fannkuch                   | 416 ms                                                       | 409 ms: 1.02x faster                                             |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                            |
| docutils                   | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                           |
| tornado_http               | 124 ms                                                       | 126 ms: 1.01x slower                                             |
| unpickle_list              | 4.60 us                                                      | 4.67 us: 1.01x slower                                            |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.01x slower                                           |
| regex_v8                   | 24.4 ms                                                      | 25.0 ms: 1.02x slower                                            |
| sqlglot_optimize           | 59.0 ms                                                      | 60.4 ms: 1.02x slower                                            |
| dulwich_log                | 67.4 ms                                                      | 69.1 ms: 1.03x slower                                            |
| unpack_sequence            | 45.7 ns                                                      | 46.9 ns: 1.03x slower                                            |
| pprint_safe_repr           | 805 ms                                                       | 826 ms: 1.03x slower                                             |
| tomli_loads                | 2.25 sec                                                     | 2.31 sec: 1.03x slower                                           |
| xml_etree_process          | 55.9 ms                                                      | 57.6 ms: 1.03x slower                                            |
| pprint_pformat             | 1.67 sec                                                     | 1.72 sec: 1.03x slower                                           |
| pickle                     | 9.89 us                                                      | 10.2 us: 1.03x slower                                            |
| richards                   | 49.7 ms                                                      | 51.7 ms: 1.04x slower                                            |
| bench_mp_pool              | 4.70 ms                                                      | 4.90 ms: 1.04x slower                                            |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                             |
| 2to3                       | 287 ms                                                       | 300 ms: 1.04x slower                                             |
| xml_etree_generate         | 79.7 ms                                                      | 83.4 ms: 1.05x slower                                            |
| regex_effbot               | 3.34 ms                                                      | 3.53 ms: 1.06x slower                                            |
| go                         | 158 ms                                                       | 167 ms: 1.06x slower                                             |
| mako                       | 11.0 ms                                                      | 11.8 ms: 1.07x slower                                            |
| regex_dna                  | 227 ms                                                       | 244 ms: 1.07x slower                                             |
| float                      | 74.9 ms                                                      | 80.7 ms: 1.08x slower                                            |
| hexiom                     | 6.98 ms                                                      | 7.63 ms: 1.09x slower                                            |
| sqlite_synth               | 2.52 us                                                      | 2.77 us: 1.10x slower                                            |
| scimark_monte_carlo        | 69.8 ms                                                      | 78.5 ms: 1.12x slower                                            |
| nbody                      | 92.9 ms                                                      | 106 ms: 1.14x slower                                             |
| pickle_list                | 3.94 us                                                      | 4.50 us: 1.14x slower                                            |
| unpickle                   | 13.3 us                                                      | 15.3 us: 1.15x slower                                            |
| async_generators           | 322 ms                                                       | 371 ms: 1.16x slower                                             |
| mypy2                      | 762 ms                                                       | 886 ms: 1.16x slower                                             |
| pyflate                    | 449 ms                                                       | 529 ms: 1.18x slower                                             |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                            |
| telco                      | 6.81 ms                                                      | 8.12 ms: 1.19x slower                                            |
| spectral_norm              | 95.1 ms                                                      | 115 ms: 1.21x slower                                             |
| scimark_fft                | 281 ms                                                       | 357 ms: 1.27x slower                                             |
| coverage                   | 66.1 ms                                                      | 84.4 ms: 1.28x slower                                            |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 5.23 ms: 1.29x slower                                            |
| scimark_sor                | 110 ms                                                       | 143 ms: 1.31x slower                                             |
| dask                       | 410 ms                                                       | 584 ms: 1.43x slower                                             |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                            |
| Geometric mean             | (ref)                                                        | 1.03x faster                                                     |

Benchmark hidden because not significant (2): asyncio_websockets, meteor_contest
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 74.07% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x