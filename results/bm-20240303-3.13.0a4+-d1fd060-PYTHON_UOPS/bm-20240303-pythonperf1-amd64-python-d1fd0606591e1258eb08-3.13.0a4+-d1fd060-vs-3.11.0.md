# Results vs. 3.11.0

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.03x faster \*
- HPT reliability: 56.80%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 224 ms: 1.05x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.74 ms: 1.11x faster                                                       |
| tornado_http   | 92.8 ms                                                     | 86.1 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 280 ms: 1.19x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 467 ms: 1.13x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 353 ms: 1.13x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 361 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 479 ms: 1.09x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 285 ms: 1.08x faster                                                        |
| async_tree_io              | 808 ms                                                      | 751 ms: 1.08x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 777 ms: 1.07x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.02x faster                                                        |
| float          | 54.4 ms                                                     | 59.9 ms: 1.10x slower                                                       |
| nbody          | 70.3 ms                                                     | 80.1 ms: 1.14x slower                                                       |
| Geometric mean | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 116 ms                                                      | 119 ms: 1.03x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| regex_compile  | 91.0 ms                                                     | 99.9 ms: 1.10x slower                                                       |
| Geometric mean | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.66 ms: 1.43x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 179 us: 1.17x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.6 us: 1.00x slower                                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.7 ms: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 66.9 ms: 1.02x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.70 us: 1.04x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| unpickle_pure_python | 157 us                                                      | 164 us: 1.05x slower                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.53 sec: 1.05x slower                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 55.8 ms: 1.06x slower                                                       |
| pickle               | 6.64 us                                                     | 7.24 us: 1.09x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.49 us: 1.12x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.14 us: 1.17x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 17.7 ms: 1.05x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.03x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.70 ms: 1.02x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 76.3 us: 4.27x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.7 ms: 1.64x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 484 ms: 1.50x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.66 ms: 1.43x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.9 ns: 1.28x faster                                                       |
| async_tree_none            | 332 ms                                                      | 280 ms: 1.19x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.71 sec: 1.18x faster                                                      |
| deltablue                  | 2.70 ms                                                     | 2.30 ms: 1.18x faster                                                       |
| comprehensions             | 15.6 us                                                     | 13.3 us: 1.17x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 179 us: 1.17x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 819 us: 1.16x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                       |
| richards_super             | 38.7 ms                                                     | 33.8 ms: 1.15x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 41.1 ns: 1.14x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 467 ms: 1.13x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 353 ms: 1.13x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 23.1 us: 1.13x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 361 ms: 1.12x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 1.04 ms: 1.12x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 4.74 ms: 1.11x faster                                                       |
| logging_simple             | 6.86 us                                                     | 6.23 us: 1.10x faster                                                       |
| raytrace                   | 213 ms                                                      | 194 ms: 1.10x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 91.2 ms: 1.10x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 479 ms: 1.09x faster                                                        |
| deepcopy                   | 246 us                                                      | 226 us: 1.09x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 285 ms: 1.08x faster                                                        |
| chaos                      | 48.4 ms                                                     | 44.8 ms: 1.08x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 86.1 ms: 1.08x faster                                                       |
| async_tree_io              | 808 ms                                                      | 751 ms: 1.08x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.69 us: 1.07x faster                                                       |
| sympy_str                  | 185 ms                                                      | 173 ms: 1.07x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 777 ms: 1.07x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 179 ms: 1.06x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 43.7 ms: 1.06x faster                                                       |
| richards                   | 31.4 ms                                                     | 29.6 ms: 1.06x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.06x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.96 us: 1.05x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 836 us: 1.04x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                                       |
| mypy2                      | 459 ms                                                      | 442 ms: 1.04x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.54 sec: 1.04x faster                                                      |
| sqlite_synth               | 1.77 us                                                     | 1.71 us: 1.03x faster                                                       |
| sympy_expand               | 299 ms                                                      | 291 ms: 1.03x faster                                                        |
| pidigits                   | 150 ms                                                      | 148 ms: 1.02x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 48.6 ms: 1.00x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.6 us: 1.00x slower                                                       |
| nqueens                    | 68.3 ms                                                     | 68.9 ms: 1.01x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                       |
| xml_etree_process          | 37.2 ms                                                     | 37.7 ms: 1.01x slower                                                       |
| mako                       | 7.58 ms                                                     | 7.70 ms: 1.02x slower                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 66.9 ms: 1.02x slower                                                       |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.03x slower                                                        |
| bench_mp_pool              | 63.2 ms                                                     | 65.5 ms: 1.04x slower                                                       |
| go                         | 101 ms                                                      | 105 ms: 1.04x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 36.0 ms: 1.04x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.70 us: 1.04x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 747 us: 1.05x slower                                                        |
| 2to3                       | 214 ms                                                      | 224 ms: 1.05x slower                                                        |
| meteor_contest             | 75.2 ms                                                     | 78.9 ms: 1.05x slower                                                       |
| unpickle_pure_python       | 157 us                                                      | 164 us: 1.05x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 17.7 ms: 1.05x slower                                                       |
| pprint_safe_repr           | 529 ms                                                      | 557 ms: 1.05x slower                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.53 sec: 1.05x slower                                                      |
| pprint_pformat             | 1.09 sec                                                    | 1.15 sec: 1.05x slower                                                      |
| xml_etree_generate         | 52.5 ms                                                     | 55.8 ms: 1.06x slower                                                       |
| fannkuch                   | 253 ms                                                      | 271 ms: 1.07x slower                                                        |
| pathlib                    | 70.9 ms                                                     | 75.9 ms: 1.07x slower                                                       |
| coverage                   | 43.4 ms                                                     | 46.6 ms: 1.07x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.24 us: 1.09x slower                                                       |
| regex_compile              | 91.0 ms                                                     | 99.9 ms: 1.10x slower                                                       |
| float                      | 54.4 ms                                                     | 59.9 ms: 1.10x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 86.7 ms: 1.11x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.49 us: 1.12x slower                                                       |
| nbody                      | 70.3 ms                                                     | 80.1 ms: 1.14x slower                                                       |
| pyflate                    | 312 ms                                                      | 363 ms: 1.16x slower                                                        |
| scimark_fft                | 179 ms                                                      | 209 ms: 1.16x slower                                                        |
| pickle_list                | 2.70 us                                                     | 3.14 us: 1.17x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.83 ms: 1.19x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.44 ms: 1.20x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 54.4 ms: 1.20x slower                                                       |
| spectral_norm              | 68.3 ms                                                     | 82.9 ms: 1.21x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.21 ms: 1.25x slower                                                       |
| scimark_lu                 | 62.8 ms                                                     | 79.7 ms: 1.27x slower                                                       |
| dask                       | 273 ms                                                      | 361 ms: 1.32x slower                                                        |
| async_generators           | 177 ms                                                      | 240 ms: 1.36x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.03x faster                                                                |

Benchmark hidden because not significant (4): json, docutils, python_startup, pycparser
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 56.80% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown