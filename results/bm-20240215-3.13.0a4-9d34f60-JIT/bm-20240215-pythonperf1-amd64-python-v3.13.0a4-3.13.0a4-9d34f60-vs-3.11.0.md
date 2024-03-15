# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a4
- machine: windows-amd64
- commit hash: 9d34f60
- commit date: 2024-02-15
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 217 ms: 1.02x slower                                            |
| chameleon      | 5.26 ms                                                     | 4.74 ms: 1.11x faster                                           |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.06x faster                                          |
| tornado_http   | 92.8 ms                                                     | 85.5 ms: 1.09x faster                                           |
| Geometric mean | (ref)                                                       | 1.06x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                            |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                            |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.16x faster                                            |
| async_tree_memoization_tg  | 405 ms                                                      | 350 ms: 1.16x faster                                            |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.13x faster                                            |
| async_tree_io              | 808 ms                                                      | 726 ms: 1.11x faster                                            |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 472 ms: 1.11x faster                                            |
| async_tree_io_tg           | 829 ms                                                      | 759 ms: 1.09x faster                                            |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 61.0 ms: 1.15x faster                                           |
| float          | 54.4 ms                                                     | 51.4 ms: 1.06x faster                                           |
| pidigits       | 150 ms                                                      | 151 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                       | 1.07x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 79.3 ms: 1.15x faster                                           |
| regex_v8       | 14.2 ms                                                     | 14.3 ms: 1.01x slower                                           |
| regex_dna      | 116 ms                                                      | 118 ms: 1.01x slower                                            |
| regex_effbot   | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                           |
| Geometric mean | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.54 ms: 1.46x faster                                           |
| unpickle_pure_python | 157 us                                                      | 126 us: 1.24x faster                                            |
| pickle_pure_python   | 208 us                                                      | 174 us: 1.20x faster                                            |
| tomli_loads          | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                          |
| xml_etree_parse      | 97.6 ms                                                     | 91.2 ms: 1.07x faster                                           |
| pickle_dict          | 18.5 us                                                     | 17.6 us: 1.05x faster                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.9 ms: 1.04x faster                                           |
| xml_etree_process    | 37.2 ms                                                     | 35.9 ms: 1.04x faster                                           |
| xml_etree_generate   | 52.5 ms                                                     | 51.9 ms: 1.01x faster                                           |
| pickle_list          | 2.70 us                                                     | 2.78 us: 1.03x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.74 us: 1.06x slower                                           |
| json_loads           | 13.0 us                                                     | 13.8 us: 1.06x slower                                           |
| pickle               | 6.64 us                                                     | 7.32 us: 1.10x slower                                           |
| unpickle             | 7.57 us                                                     | 8.41 us: 1.11x slower                                           |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                           |
| python_startup_no_site | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                           |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.71 ms: 1.13x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 69.7 us: 4.68x faster                                           |
| generators                 | 34.0 ms                                                     | 19.9 ms: 1.71x faster                                           |
| asyncio_tcp                | 726 ms                                                      | 477 ms: 1.52x faster                                            |
| comprehensions             | 15.6 us                                                     | 10.6 us: 1.47x faster                                           |
| json_dumps                 | 8.09 ms                                                     | 5.54 ms: 1.46x faster                                           |
| richards_super             | 38.7 ms                                                     | 28.2 ms: 1.38x faster                                           |
| deltablue                  | 2.70 ms                                                     | 1.99 ms: 1.36x faster                                           |
| logging_silent             | 71.8 ns                                                     | 54.0 ns: 1.33x faster                                           |
| raytrace                   | 213 ms                                                      | 166 ms: 1.29x faster                                            |
| richards                   | 31.4 ms                                                     | 24.8 ms: 1.27x faster                                           |
| sqlglot_parse              | 953 us                                                      | 755 us: 1.26x faster                                            |
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                            |
| unpickle_pure_python       | 157 us                                                      | 126 us: 1.24x faster                                            |
| deepcopy_memo              | 26.0 us                                                     | 21.3 us: 1.22x faster                                           |
| pickle_pure_python         | 208 us                                                      | 174 us: 1.20x faster                                            |
| sqlglot_transpile          | 1.16 ms                                                     | 978 us: 1.19x faster                                            |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.70 sec: 1.19x faster                                          |
| unpack_sequence            | 46.9 ns                                                     | 40.0 ns: 1.17x faster                                           |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                            |
| sqlite_synth               | 1.77 us                                                     | 1.51 us: 1.17x faster                                           |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.16x faster                                            |
| chaos                      | 48.4 ms                                                     | 41.7 ms: 1.16x faster                                           |
| async_tree_memoization_tg  | 405 ms                                                      | 350 ms: 1.16x faster                                            |
| nbody                      | 70.3 ms                                                     | 61.0 ms: 1.15x faster                                           |
| logging_simple             | 6.86 us                                                     | 5.95 us: 1.15x faster                                           |
| sympy_sum                  | 100 ms                                                      | 86.8 ms: 1.15x faster                                           |
| dulwich_log                | 46.4 ms                                                     | 40.4 ms: 1.15x faster                                           |
| regex_compile              | 91.0 ms                                                     | 79.3 ms: 1.15x faster                                           |
| nqueens                    | 68.3 ms                                                     | 59.7 ms: 1.14x faster                                           |
| coroutines                 | 15.0 ms                                                     | 13.2 ms: 1.14x faster                                           |
| scimark_lu                 | 62.8 ms                                                     | 55.3 ms: 1.14x faster                                           |
| deepcopy                   | 246 us                                                      | 217 us: 1.14x faster                                            |
| sympy_str                  | 185 ms                                                      | 163 ms: 1.14x faster                                            |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.13x faster                                            |
| mako                       | 7.58 ms                                                     | 6.71 ms: 1.13x faster                                           |
| logging_format             | 7.16 us                                                     | 6.39 us: 1.12x faster                                           |
| tomli_loads                | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                          |
| async_tree_io              | 808 ms                                                      | 726 ms: 1.11x faster                                            |
| pprint_pformat             | 1.09 sec                                                    | 980 ms: 1.11x faster                                            |
| chameleon                  | 5.26 ms                                                     | 4.74 ms: 1.11x faster                                           |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 472 ms: 1.11x faster                                            |
| pprint_safe_repr           | 529 ms                                                      | 480 ms: 1.10x faster                                            |
| sqlglot_normalize          | 190 ms                                                      | 173 ms: 1.10x faster                                            |
| sympy_integrate            | 14.0 ms                                                     | 12.8 ms: 1.09x faster                                           |
| async_tree_io_tg           | 829 ms                                                      | 759 ms: 1.09x faster                                            |
| mypy2                      | 459 ms                                                      | 423 ms: 1.09x faster                                            |
| tornado_http               | 92.8 ms                                                     | 85.5 ms: 1.09x faster                                           |
| spectral_norm              | 68.3 ms                                                     | 63.3 ms: 1.08x faster                                           |
| sympy_expand               | 299 ms                                                      | 277 ms: 1.08x faster                                            |
| deepcopy_reduce            | 2.06 us                                                     | 1.92 us: 1.08x faster                                           |
| mdp                        | 1.59 sec                                                    | 1.49 sec: 1.07x faster                                          |
| xml_etree_parse            | 97.6 ms                                                     | 91.2 ms: 1.07x faster                                           |
| bench_thread_pool          | 872 us                                                      | 817 us: 1.07x faster                                            |
| crypto_pyaes               | 48.9 ms                                                     | 45.8 ms: 1.07x faster                                           |
| go                         | 101 ms                                                      | 94.8 ms: 1.07x faster                                           |
| float                      | 54.4 ms                                                     | 51.4 ms: 1.06x faster                                           |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.06x faster                                          |
| pickle_dict                | 18.5 us                                                     | 17.6 us: 1.05x faster                                           |
| fannkuch                   | 253 ms                                                      | 242 ms: 1.05x faster                                            |
| xml_etree_iterparse        | 65.6 ms                                                     | 62.9 ms: 1.04x faster                                           |
| xml_etree_process          | 37.2 ms                                                     | 35.9 ms: 1.04x faster                                           |
| sqlglot_optimize           | 34.5 ms                                                     | 33.5 ms: 1.03x faster                                           |
| scimark_sor                | 78.1 ms                                                     | 76.0 ms: 1.03x faster                                           |
| pyflate                    | 312 ms                                                      | 308 ms: 1.01x faster                                            |
| xml_etree_generate         | 52.5 ms                                                     | 51.9 ms: 1.01x faster                                           |
| pidigits                   | 150 ms                                                      | 151 ms: 1.01x slower                                            |
| regex_v8                   | 14.2 ms                                                     | 14.3 ms: 1.01x slower                                           |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                           |
| regex_dna                  | 116 ms                                                      | 118 ms: 1.01x slower                                            |
| 2to3                       | 214 ms                                                      | 217 ms: 1.02x slower                                            |
| meteor_contest             | 75.2 ms                                                     | 76.7 ms: 1.02x slower                                           |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.65 ms: 1.03x slower                                           |
| pickle_list                | 2.70 us                                                     | 2.78 us: 1.03x slower                                           |
| create_gc_cycles           | 713 us                                                      | 736 us: 1.03x slower                                            |
| python_startup             | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                           |
| regex_effbot               | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                           |
| bench_mp_pool              | 63.2 ms                                                     | 66.6 ms: 1.05x slower                                           |
| scimark_fft                | 179 ms                                                      | 189 ms: 1.05x slower                                            |
| unpickle_list              | 2.59 us                                                     | 2.74 us: 1.06x slower                                           |
| pathlib                    | 70.9 ms                                                     | 75.3 ms: 1.06x slower                                           |
| json_loads                 | 13.0 us                                                     | 13.8 us: 1.06x slower                                           |
| python_startup_no_site     | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                           |
| pickle                     | 6.64 us                                                     | 7.32 us: 1.10x slower                                           |
| unpickle                   | 7.57 us                                                     | 8.41 us: 1.11x slower                                           |
| coverage                   | 43.4 ms                                                     | 48.4 ms: 1.11x slower                                           |
| telco                      | 4.06 ms                                                     | 4.57 ms: 1.13x slower                                           |
| hexiom                     | 4.55 ms                                                     | 5.14 ms: 1.13x slower                                           |
| scimark_monte_carlo        | 45.3 ms                                                     | 56.9 ms: 1.26x slower                                           |
| dask                       | 273 ms                                                      | 360 ms: 1.32x slower                                            |
| async_generators           | 177 ms                                                      | 238 ms: 1.34x slower                                            |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                    |

Benchmark hidden because not significant (2): json, pycparser
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown