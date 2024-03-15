
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a1
- machine: windows-amd64
- commit hash: ad056f0
- commit date: 2023-10-13
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1-amd64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 216 ms: 1.01x slower                                            |
| chameleon      | 5.26 ms                                                     | 4.98 ms: 1.06x faster                                           |
| docutils       | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                          |
| tornado_http   | 92.8 ms                                                     | 89.1 ms: 1.04x faster                                           |
| Geometric mean | (ref)                                                       | 1.03x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1-amd64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 267 ms: 1.25x faster                                            |
| async_tree_memoization     | 399 ms                                                      | 340 ms: 1.17x faster                                            |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.16x faster                                            |
| async_tree_memoization_tg  | 405 ms                                                      | 359 ms: 1.13x faster                                            |
| async_tree_io              | 808 ms                                                      | 723 ms: 1.12x faster                                            |
| async_tree_none_tg         | 309 ms                                                      | 285 ms: 1.08x faster                                            |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 486 ms: 1.08x faster                                            |
| async_tree_io_tg           | 829 ms                                                      | 772 ms: 1.07x faster                                            |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1-amd64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 53.6 ms: 1.01x faster                                           |
| nbody          | 70.3 ms                                                     | 72.2 ms: 1.03x slower                                           |
| Geometric mean | (ref)                                                       | 1.00x slower                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1-amd64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_dna      | 116 ms                                                      | 119 ms: 1.02x slower                                            |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.05x slower                                           |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x slower                                                    |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1-amd64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.60 ms: 1.44x faster                                           |
| unpickle_pure_python | 157 us                                                      | 137 us: 1.14x faster                                            |
| pickle_pure_python   | 208 us                                                      | 190 us: 1.10x faster                                            |
| xml_etree_parse      | 97.6 ms                                                     | 91.6 ms: 1.07x faster                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.0 ms: 1.02x faster                                           |
| pickle_dict          | 18.5 us                                                     | 18.4 us: 1.01x faster                                           |
| tomli_loads          | 1.46 sec                                                    | 1.48 sec: 1.01x slower                                          |
| xml_etree_process    | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                           |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                           |
| pickle               | 6.64 us                                                     | 6.98 us: 1.05x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 55.4 ms: 1.05x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.74 us: 1.06x slower                                           |
| unpickle             | 7.57 us                                                     | 8.12 us: 1.07x slower                                           |
| pickle_list          | 2.70 us                                                     | 2.94 us: 1.09x slower                                           |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1-amd64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 16.2 ms: 1.04x faster                                           |
| Geometric mean         | (ref)                                                       | 1.02x faster                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1-amd64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.20 ms: 1.05x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-pythonperf1-amd64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 96.3 us: 3.38x faster                                           |
| asyncio_tcp                | 726 ms                                                      | 470 ms: 1.54x faster                                            |
| generators                 | 34.0 ms                                                     | 22.3 ms: 1.52x faster                                           |
| json_dumps                 | 8.09 ms                                                     | 5.60 ms: 1.44x faster                                           |
| async_tree_none            | 332 ms                                                      | 267 ms: 1.25x faster                                            |
| deltablue                  | 2.70 ms                                                     | 2.19 ms: 1.23x faster                                           |
| raytrace                   | 213 ms                                                      | 174 ms: 1.22x faster                                            |
| unpack_sequence            | 46.9 ns                                                     | 38.5 ns: 1.22x faster                                           |
| richards_super             | 38.7 ms                                                     | 32.0 ms: 1.21x faster                                           |
| chaos                      | 48.4 ms                                                     | 40.4 ms: 1.20x faster                                           |
| sqlglot_parse              | 953 us                                                      | 811 us: 1.18x faster                                            |
| async_tree_memoization     | 399 ms                                                      | 340 ms: 1.17x faster                                            |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.16x faster                                            |
| nqueens                    | 68.3 ms                                                     | 59.1 ms: 1.16x faster                                           |
| unpickle_pure_python       | 157 us                                                      | 137 us: 1.14x faster                                            |
| logging_silent             | 71.8 ns                                                     | 63.2 ns: 1.14x faster                                           |
| sqlglot_transpile          | 1.16 ms                                                     | 1.03 ms: 1.13x faster                                           |
| crypto_pyaes               | 48.9 ms                                                     | 43.3 ms: 1.13x faster                                           |
| async_tree_memoization_tg  | 405 ms                                                      | 359 ms: 1.13x faster                                            |
| go                         | 101 ms                                                      | 90.0 ms: 1.12x faster                                           |
| async_tree_io              | 808 ms                                                      | 723 ms: 1.12x faster                                            |
| hexiom                     | 4.55 ms                                                     | 4.09 ms: 1.11x faster                                           |
| scimark_monte_carlo        | 45.3 ms                                                     | 41.0 ms: 1.11x faster                                           |
| comprehensions             | 15.6 us                                                     | 14.2 us: 1.11x faster                                           |
| pickle_pure_python         | 208 us                                                      | 190 us: 1.10x faster                                            |
| sympy_sum                  | 100 ms                                                      | 91.1 ms: 1.10x faster                                           |
| richards                   | 31.4 ms                                                     | 28.8 ms: 1.09x faster                                           |
| spectral_norm              | 68.3 ms                                                     | 63.0 ms: 1.09x faster                                           |
| async_tree_none_tg         | 309 ms                                                      | 285 ms: 1.08x faster                                            |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 486 ms: 1.08x faster                                            |
| async_tree_io_tg           | 829 ms                                                      | 772 ms: 1.07x faster                                            |
| sqlite_synth               | 1.77 us                                                     | 1.65 us: 1.07x faster                                           |
| logging_simple             | 6.86 us                                                     | 6.40 us: 1.07x faster                                           |
| deepcopy                   | 246 us                                                      | 230 us: 1.07x faster                                            |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.89 sec: 1.07x faster                                          |
| scimark_lu                 | 62.8 ms                                                     | 58.6 ms: 1.07x faster                                           |
| sympy_integrate            | 14.0 ms                                                     | 13.1 ms: 1.07x faster                                           |
| mdp                        | 1.59 sec                                                    | 1.49 sec: 1.07x faster                                          |
| xml_etree_parse            | 97.6 ms                                                     | 91.6 ms: 1.07x faster                                           |
| sympy_str                  | 185 ms                                                      | 175 ms: 1.06x faster                                            |
| chameleon                  | 5.26 ms                                                     | 4.98 ms: 1.06x faster                                           |
| pprint_pformat             | 1.09 sec                                                    | 1.03 sec: 1.05x faster                                          |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.45 ms: 1.05x faster                                           |
| mako                       | 7.58 ms                                                     | 7.20 ms: 1.05x faster                                           |
| logging_format             | 7.16 us                                                     | 6.81 us: 1.05x faster                                           |
| deepcopy_memo              | 26.0 us                                                     | 24.8 us: 1.05x faster                                           |
| pyflate                    | 312 ms                                                      | 298 ms: 1.05x faster                                            |
| pprint_safe_repr           | 529 ms                                                      | 507 ms: 1.04x faster                                            |
| sympy_expand               | 299 ms                                                      | 287 ms: 1.04x faster                                            |
| bench_thread_pool          | 872 us                                                      | 836 us: 1.04x faster                                            |
| tornado_http               | 92.8 ms                                                     | 89.1 ms: 1.04x faster                                           |
| python_startup_no_site     | 16.8 ms                                                     | 16.2 ms: 1.04x faster                                           |
| sqlglot_normalize          | 190 ms                                                      | 184 ms: 1.04x faster                                            |
| dulwich_log                | 46.4 ms                                                     | 45.2 ms: 1.03x faster                                           |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.0 ms: 1.02x faster                                           |
| scimark_fft                | 179 ms                                                      | 176 ms: 1.02x faster                                            |
| docutils                   | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                          |
| coroutines                 | 15.0 ms                                                     | 14.7 ms: 1.02x faster                                           |
| fannkuch                   | 253 ms                                                      | 249 ms: 1.02x faster                                            |
| scimark_sor                | 78.1 ms                                                     | 77.0 ms: 1.01x faster                                           |
| float                      | 54.4 ms                                                     | 53.6 ms: 1.01x faster                                           |
| meteor_contest             | 75.2 ms                                                     | 74.5 ms: 1.01x faster                                           |
| pickle_dict                | 18.5 us                                                     | 18.4 us: 1.01x faster                                           |
| deepcopy_reduce            | 2.06 us                                                     | 2.07 us: 1.01x slower                                           |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                           |
| 2to3                       | 214 ms                                                      | 216 ms: 1.01x slower                                            |
| bench_mp_pool              | 63.2 ms                                                     | 64.0 ms: 1.01x slower                                           |
| tomli_loads                | 1.46 sec                                                    | 1.48 sec: 1.01x slower                                          |
| create_gc_cycles           | 713 us                                                      | 728 us: 1.02x slower                                            |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.02x slower                                            |
| nbody                      | 70.3 ms                                                     | 72.2 ms: 1.03x slower                                           |
| xml_etree_process          | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                           |
| json_loads                 | 13.0 us                                                     | 13.5 us: 1.04x slower                                           |
| coverage                   | 43.4 ms                                                     | 45.4 ms: 1.05x slower                                           |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.05x slower                                           |
| pickle                     | 6.64 us                                                     | 6.98 us: 1.05x slower                                           |
| xml_etree_generate         | 52.5 ms                                                     | 55.4 ms: 1.05x slower                                           |
| unpickle_list              | 2.59 us                                                     | 2.74 us: 1.06x slower                                           |
| regex_effbot               | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                           |
| unpickle                   | 7.57 us                                                     | 8.12 us: 1.07x slower                                           |
| pickle_list                | 2.70 us                                                     | 2.94 us: 1.09x slower                                           |
| pathlib                    | 70.9 ms                                                     | 78.5 ms: 1.11x slower                                           |
| telco                      | 4.06 ms                                                     | 4.73 ms: 1.16x slower                                           |
| pycparser                  | 720 ms                                                      | 861 ms: 1.20x slower                                            |
| async_generators           | 177 ms                                                      | 236 ms: 1.33x slower                                            |
| Geometric mean             | (ref)                                                       | 1.07x faster                                                    |

Benchmark hidden because not significant (5): python_startup, gc_traversal, regex_compile, pidigits, json
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown