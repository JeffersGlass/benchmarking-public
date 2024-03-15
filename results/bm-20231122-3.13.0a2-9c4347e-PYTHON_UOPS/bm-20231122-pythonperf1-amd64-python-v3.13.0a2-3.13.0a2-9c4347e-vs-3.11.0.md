
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a2
- machine: windows-amd64
- commit hash: 9c4347e
- commit date: 2023-11-22
- overall geometric mean: 1.05x faster
- HPT reliability: 99.82%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1-amd64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 218 ms: 1.02x slower                                            |
| chameleon      | 5.26 ms                                                     | 4.84 ms: 1.09x faster                                           |
| docutils       | 1.64 sec                                                    | 1.55 sec: 1.06x faster                                          |
| tornado_http   | 92.8 ms                                                     | 89.4 ms: 1.04x faster                                           |
| Geometric mean | (ref)                                                       | 1.04x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1-amd64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 267 ms: 1.24x faster                                            |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 454 ms: 1.17x faster                                            |
| async_tree_memoization     | 399 ms                                                      | 346 ms: 1.15x faster                                            |
| async_tree_memoization_tg  | 405 ms                                                      | 363 ms: 1.11x faster                                            |
| async_tree_io              | 808 ms                                                      | 729 ms: 1.11x faster                                            |
| async_tree_none_tg         | 309 ms                                                      | 281 ms: 1.10x faster                                            |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 481 ms: 1.09x faster                                            |
| async_tree_io_tg           | 829 ms                                                      | 766 ms: 1.08x faster                                            |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1-amd64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.01x faster                                            |
| float          | 54.4 ms                                                     | 57.1 ms: 1.05x slower                                           |
| nbody          | 70.3 ms                                                     | 81.4 ms: 1.16x slower                                           |
| Geometric mean | (ref)                                                       | 1.06x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1-amd64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 88.1 ms: 1.03x faster                                           |
| regex_dna      | 116 ms                                                      | 120 ms: 1.03x slower                                            |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                           |
| regex_v8       | 14.2 ms                                                     | 17.9 ms: 1.26x slower                                           |
| Geometric mean | (ref)                                                       | 1.07x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1-amd64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.46 ms: 1.48x faster                                           |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                            |
| unpickle_pure_python | 157 us                                                      | 136 us: 1.15x faster                                            |
| xml_etree_parse      | 97.6 ms                                                     | 93.0 ms: 1.05x faster                                           |
| tomli_loads          | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                          |
| pickle_dict          | 18.5 us                                                     | 18.6 us: 1.01x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.62 us: 1.01x slower                                           |
| xml_etree_process    | 37.2 ms                                                     | 37.6 ms: 1.01x slower                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 67.5 ms: 1.03x slower                                           |
| json_loads           | 13.0 us                                                     | 13.4 us: 1.03x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 55.1 ms: 1.05x slower                                           |
| pickle               | 6.64 us                                                     | 6.96 us: 1.05x slower                                           |
| unpickle             | 7.57 us                                                     | 8.09 us: 1.07x slower                                           |
| pickle_list          | 2.70 us                                                     | 3.32 us: 1.23x slower                                           |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1-amd64-python-v3.13.0a2-3.13.0a2-9c4347e |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.7 ms: 1.05x slower                                           |
| python_startup_no_site | 16.8 ms                                                     | 19.6 ms: 1.16x slower                                           |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1-amd64-python-v3.13.0a2-3.13.0a2-9c4347e |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.38 ms: 1.03x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231122-pythonperf1-amd64-python-v3.13.0a2-3.13.0a2-9c4347e |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 77.0 us: 4.23x faster                                           |
| generators                 | 34.0 ms                                                     | 20.3 ms: 1.67x faster                                           |
| asyncio_tcp                | 726 ms                                                      | 477 ms: 1.52x faster                                            |
| json_dumps                 | 8.09 ms                                                     | 5.46 ms: 1.48x faster                                           |
| logging_silent             | 71.8 ns                                                     | 55.5 ns: 1.29x faster                                           |
| richards_super             | 38.7 ms                                                     | 30.1 ms: 1.29x faster                                           |
| async_tree_none            | 332 ms                                                      | 267 ms: 1.24x faster                                            |
| sqlglot_parse              | 953 us                                                      | 779 us: 1.22x faster                                            |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.66 sec: 1.22x faster                                          |
| comprehensions             | 15.6 us                                                     | 12.9 us: 1.21x faster                                           |
| raytrace                   | 213 ms                                                      | 177 ms: 1.20x faster                                            |
| pickle_pure_python         | 208 us                                                      | 175 us: 1.19x faster                                            |
| unpack_sequence            | 46.9 ns                                                     | 40.1 ns: 1.17x faster                                           |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 454 ms: 1.17x faster                                            |
| richards                   | 31.4 ms                                                     | 27.0 ms: 1.16x faster                                           |
| sqlglot_transpile          | 1.16 ms                                                     | 1.01 ms: 1.16x faster                                           |
| async_tree_memoization     | 399 ms                                                      | 346 ms: 1.15x faster                                            |
| unpickle_pure_python       | 157 us                                                      | 136 us: 1.15x faster                                            |
| deepcopy                   | 246 us                                                      | 216 us: 1.14x faster                                            |
| deepcopy_memo              | 26.0 us                                                     | 22.9 us: 1.14x faster                                           |
| coroutines                 | 15.0 ms                                                     | 13.3 ms: 1.13x faster                                           |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.13x faster                                           |
| sympy_sum                  | 100 ms                                                      | 89.1 ms: 1.12x faster                                           |
| async_tree_memoization_tg  | 405 ms                                                      | 363 ms: 1.11x faster                                            |
| mdp                        | 1.59 sec                                                    | 1.44 sec: 1.11x faster                                          |
| async_tree_io              | 808 ms                                                      | 729 ms: 1.11x faster                                            |
| logging_simple             | 6.86 us                                                     | 6.24 us: 1.10x faster                                           |
| sympy_str                  | 185 ms                                                      | 168 ms: 1.10x faster                                            |
| go                         | 101 ms                                                      | 92.1 ms: 1.10x faster                                           |
| async_tree_none_tg         | 309 ms                                                      | 281 ms: 1.10x faster                                            |
| scimark_lu                 | 62.8 ms                                                     | 57.6 ms: 1.09x faster                                           |
| chaos                      | 48.4 ms                                                     | 44.4 ms: 1.09x faster                                           |
| chameleon                  | 5.26 ms                                                     | 4.84 ms: 1.09x faster                                           |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 481 ms: 1.09x faster                                            |
| dulwich_log                | 46.4 ms                                                     | 42.8 ms: 1.08x faster                                           |
| async_tree_io_tg           | 829 ms                                                      | 766 ms: 1.08x faster                                            |
| dask                       | 273 ms                                                      | 254 ms: 1.07x faster                                            |
| pycparser                  | 720 ms                                                      | 675 ms: 1.07x faster                                            |
| sympy_expand               | 299 ms                                                      | 281 ms: 1.06x faster                                            |
| docutils                   | 1.64 sec                                                    | 1.55 sec: 1.06x faster                                          |
| logging_format             | 7.16 us                                                     | 6.76 us: 1.06x faster                                           |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.06x faster                                           |
| deepcopy_reduce            | 2.06 us                                                     | 1.94 us: 1.06x faster                                           |
| xml_etree_parse            | 97.6 ms                                                     | 93.0 ms: 1.05x faster                                           |
| nqueens                    | 68.3 ms                                                     | 65.3 ms: 1.05x faster                                           |
| sqlglot_normalize          | 190 ms                                                      | 183 ms: 1.04x faster                                            |
| tornado_http               | 92.8 ms                                                     | 89.4 ms: 1.04x faster                                           |
| regex_compile              | 91.0 ms                                                     | 88.1 ms: 1.03x faster                                           |
| mako                       | 7.58 ms                                                     | 7.38 ms: 1.03x faster                                           |
| tomli_loads                | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                          |
| pprint_safe_repr           | 529 ms                                                      | 519 ms: 1.02x faster                                            |
| bench_thread_pool          | 872 us                                                      | 858 us: 1.02x faster                                            |
| pidigits                   | 150 ms                                                      | 148 ms: 1.01x faster                                            |
| pprint_pformat             | 1.09 sec                                                    | 1.07 sec: 1.01x faster                                          |
| pickle_dict                | 18.5 us                                                     | 18.6 us: 1.01x slower                                           |
| crypto_pyaes               | 48.9 ms                                                     | 49.2 ms: 1.01x slower                                           |
| scimark_sor                | 78.1 ms                                                     | 78.6 ms: 1.01x slower                                           |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                           |
| deltablue                  | 2.70 ms                                                     | 2.72 ms: 1.01x slower                                           |
| unpickle_list              | 2.59 us                                                     | 2.62 us: 1.01x slower                                           |
| xml_etree_process          | 37.2 ms                                                     | 37.6 ms: 1.01x slower                                           |
| 2to3                       | 214 ms                                                      | 218 ms: 1.02x slower                                            |
| bench_mp_pool              | 63.2 ms                                                     | 64.9 ms: 1.03x slower                                           |
| create_gc_cycles           | 713 us                                                      | 732 us: 1.03x slower                                            |
| xml_etree_iterparse        | 65.6 ms                                                     | 67.5 ms: 1.03x slower                                           |
| meteor_contest             | 75.2 ms                                                     | 77.5 ms: 1.03x slower                                           |
| regex_dna                  | 116 ms                                                      | 120 ms: 1.03x slower                                            |
| json_loads                 | 13.0 us                                                     | 13.4 us: 1.03x slower                                           |
| pyflate                    | 312 ms                                                      | 324 ms: 1.04x slower                                            |
| coverage                   | 43.4 ms                                                     | 45.2 ms: 1.04x slower                                           |
| python_startup             | 19.8 ms                                                     | 20.7 ms: 1.05x slower                                           |
| xml_etree_generate         | 52.5 ms                                                     | 55.1 ms: 1.05x slower                                           |
| pickle                     | 6.64 us                                                     | 6.96 us: 1.05x slower                                           |
| float                      | 54.4 ms                                                     | 57.1 ms: 1.05x slower                                           |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                           |
| unpickle                   | 7.57 us                                                     | 8.09 us: 1.07x slower                                           |
| scimark_monte_carlo        | 45.3 ms                                                     | 49.4 ms: 1.09x slower                                           |
| fannkuch                   | 253 ms                                                      | 277 ms: 1.09x slower                                            |
| hexiom                     | 4.55 ms                                                     | 5.03 ms: 1.10x slower                                           |
| pathlib                    | 70.9 ms                                                     | 78.5 ms: 1.11x slower                                           |
| telco                      | 4.06 ms                                                     | 4.64 ms: 1.14x slower                                           |
| nbody                      | 70.3 ms                                                     | 81.4 ms: 1.16x slower                                           |
| python_startup_no_site     | 16.8 ms                                                     | 19.6 ms: 1.16x slower                                           |
| scimark_fft                | 179 ms                                                      | 213 ms: 1.19x slower                                            |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.09 ms: 1.20x slower                                           |
| spectral_norm              | 68.3 ms                                                     | 84.1 ms: 1.23x slower                                           |
| pickle_list                | 2.70 us                                                     | 3.32 us: 1.23x slower                                           |
| regex_v8                   | 14.2 ms                                                     | 17.9 ms: 1.26x slower                                           |
| mypy2                      | 459 ms                                                      | 589 ms: 1.28x slower                                            |
| async_generators           | 177 ms                                                      | 228 ms: 1.29x slower                                            |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                    |

Benchmark hidden because not significant (2): gc_traversal, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.82% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown