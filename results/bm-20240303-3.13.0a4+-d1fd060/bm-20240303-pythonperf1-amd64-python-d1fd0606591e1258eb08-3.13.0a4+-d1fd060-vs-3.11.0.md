# Results vs. 3.11.0

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.11x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| chameleon      | 5.26 ms                                                     | 4.79 ms: 1.10x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.55 sec: 1.06x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 83.4 ms: 1.11x faster                                                       |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 451 ms: 1.17x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.16x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 348 ms: 1.16x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 273 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 469 ms: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 760 ms: 1.09x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 52.9 ms: 1.03x faster                                                       |
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| nbody          | 70.3 ms                                                     | 69.7 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 77.5 ms: 1.17x faster                                                       |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.58 ms: 1.45x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 127 us: 1.23x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 181 us: 1.15x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 93.4 ms: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.6 ms: 1.03x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.44 sec: 1.01x faster                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 52.2 ms: 1.01x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.4 us: 1.01x faster                                                       |
| unpickle_list        | 2.59 us                                                     | 2.71 us: 1.05x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| pickle               | 6.64 us                                                     | 7.14 us: 1.08x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.28 us: 1.09x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.97 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.0 ms: 1.01x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 17.8 ms: 1.06x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.03x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.48 ms: 1.17x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 72.7 us: 4.48x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.2 ms: 1.60x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 479 ms: 1.52x faster                                                        |
| comprehensions             | 15.6 us                                                     | 10.7 us: 1.45x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.58 ms: 1.45x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.02 ms: 1.34x faster                                                       |
| raytrace                   | 213 ms                                                      | 164 ms: 1.30x faster                                                        |
| logging_silent             | 71.8 ns                                                     | 56.1 ns: 1.28x faster                                                       |
| richards_super             | 38.7 ms                                                     | 30.3 ms: 1.28x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 749 us: 1.27x faster                                                        |
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| chaos                      | 48.4 ms                                                     | 39.1 ms: 1.24x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 81.1 ms: 1.23x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 127 us: 1.23x faster                                                        |
| hexiom                     | 4.55 ms                                                     | 3.76 ms: 1.21x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 967 us: 1.20x faster                                                        |
| sympy_str                  | 185 ms                                                      | 155 ms: 1.20x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 57.1 ms: 1.20x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 52.5 ms: 1.20x faster                                                       |
| go                         | 101 ms                                                      | 84.7 ms: 1.19x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 39.3 ns: 1.19x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 77.5 ms: 1.17x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 451 ms: 1.17x faster                                                        |
| mako                       | 7.58 ms                                                     | 6.48 ms: 1.17x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 41.8 ms: 1.17x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.16x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 12.1 ms: 1.16x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.0 ms: 1.16x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 39.9 ms: 1.16x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 348 ms: 1.16x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 22.4 us: 1.16x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 181 us: 1.15x faster                                                        |
| logging_simple             | 6.86 us                                                     | 5.95 us: 1.15x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.76 sec: 1.15x faster                                                      |
| mdp                        | 1.59 sec                                                    | 1.39 sec: 1.15x faster                                                      |
| scimark_monte_carlo        | 45.3 ms                                                     | 39.6 ms: 1.14x faster                                                       |
| sympy_expand               | 299 ms                                                      | 262 ms: 1.14x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.13x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 273 ms: 1.13x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 60.8 ms: 1.12x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.40 us: 1.12x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 469 ms: 1.12x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 83.4 ms: 1.11x faster                                                       |
| mypy2                      | 459 ms                                                      | 413 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.79 ms: 1.10x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 760 ms: 1.09x faster                                                        |
| deepcopy                   | 246 us                                                      | 227 us: 1.09x faster                                                        |
| pyflate                    | 312 ms                                                      | 290 ms: 1.08x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.41 ms: 1.07x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.02 sec: 1.07x faster                                                      |
| sqlglot_normalize          | 190 ms                                                      | 179 ms: 1.06x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.55 sec: 1.06x faster                                                      |
| pprint_safe_repr           | 529 ms                                                      | 499 ms: 1.06x faster                                                        |
| fannkuch                   | 253 ms                                                      | 241 ms: 1.05x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 830 us: 1.05x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 93.4 ms: 1.05x faster                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.6 ms: 1.03x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 2.00 us: 1.03x faster                                                       |
| meteor_contest             | 75.2 ms                                                     | 73.1 ms: 1.03x faster                                                       |
| float                      | 54.4 ms                                                     | 52.9 ms: 1.03x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 33.7 ms: 1.02x faster                                                       |
| pidigits                   | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| scimark_sor                | 78.1 ms                                                     | 76.6 ms: 1.02x faster                                                       |
| scimark_fft                | 179 ms                                                      | 177 ms: 1.01x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.44 sec: 1.01x faster                                                      |
| nbody                      | 70.3 ms                                                     | 69.7 ms: 1.01x faster                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 52.2 ms: 1.01x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.4 us: 1.01x faster                                                       |
| python_startup             | 19.8 ms                                                     | 20.0 ms: 1.01x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 64.1 ms: 1.01x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 735 us: 1.03x slower                                                        |
| regex_dna                  | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| unpickle_list              | 2.59 us                                                     | 2.71 us: 1.05x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 17.8 ms: 1.06x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 75.2 ms: 1.06x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.14 us: 1.08x slower                                                       |
| coverage                   | 43.4 ms                                                     | 47.0 ms: 1.08x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.28 us: 1.09x slower                                                       |
| json                       | 2.98 ms                                                     | 3.28 ms: 1.10x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.97 us: 1.10x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.85 ms: 1.19x slower                                                       |
| async_generators           | 177 ms                                                      | 228 ms: 1.29x slower                                                        |
| dask                       | 273 ms                                                      | 359 ms: 1.32x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                |

Benchmark hidden because not significant (2): pycparser, 2to3
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown