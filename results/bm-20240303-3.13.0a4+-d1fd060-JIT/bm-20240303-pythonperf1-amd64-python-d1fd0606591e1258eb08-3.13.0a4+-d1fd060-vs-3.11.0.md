# Results vs. 3.11.0

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 226 ms: 1.06x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.77 ms: 1.10x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 85.2 ms: 1.09x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 351 ms: 1.15x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 273 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.13x faster                                                        |
| async_tree_io              | 808 ms                                                      | 725 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 758 ms: 1.09x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 60.2 ms: 1.17x faster                                                       |
| float          | 54.4 ms                                                     | 49.5 ms: 1.10x faster                                                       |
| Geometric mean | (ref)                                                       | 1.09x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 116 ms                                                      | 116 ms: 1.00x faster                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.55 ms: 1.03x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.56 ms: 1.46x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 176 us: 1.18x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 139 us: 1.13x faster                                                        |
| pickle_dict          | 18.5 us                                                     | 17.6 us: 1.05x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 93.6 ms: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.8 ms: 1.03x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.9 ms: 1.01x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 54.3 ms: 1.03x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.73 us: 1.05x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.9 us: 1.07x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.94 us: 1.09x slower                                                       |
| pickle               | 6.64 us                                                     | 7.33 us: 1.10x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.46 us: 1.12x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 24.3 ms: 1.23x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 22.2 ms: 1.32x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.27x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.12 ms: 1.24x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.9 us: 4.60x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.3 ms: 1.59x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 475 ms: 1.53x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.56 ms: 1.46x faster                                                       |
| comprehensions             | 15.6 us                                                     | 11.0 us: 1.42x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.06 ms: 1.31x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.4 ns: 1.30x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.12 ms: 1.24x faster                                                       |
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 57.0 ms: 1.20x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 796 us: 1.20x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.70 sec: 1.19x faster                                                      |
| pickle_pure_python         | 208 us                                                      | 176 us: 1.18x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 22.1 us: 1.17x faster                                                       |
| raytrace                   | 213 ms                                                      | 182 ms: 1.17x faster                                                        |
| chaos                      | 48.4 ms                                                     | 41.3 ms: 1.17x faster                                                       |
| nbody                      | 70.3 ms                                                     | 60.2 ms: 1.17x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| logging_simple             | 6.86 us                                                     | 5.90 us: 1.16x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 351 ms: 1.15x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 1.02 ms: 1.14x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 87.9 ms: 1.14x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 40.8 ms: 1.14x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 273 ms: 1.13x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| richards_super             | 38.7 ms                                                     | 34.2 ms: 1.13x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 139 us: 1.13x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.29 ms: 1.13x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.13x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.37 us: 1.12x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| async_tree_io              | 808 ms                                                      | 725 ms: 1.11x faster                                                        |
| sympy_str                  | 185 ms                                                      | 166 ms: 1.11x faster                                                        |
| deepcopy                   | 246 us                                                      | 222 us: 1.11x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.77 ms: 1.10x faster                                                       |
| float                      | 54.4 ms                                                     | 49.5 ms: 1.10x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 44.5 ms: 1.10x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 758 ms: 1.09x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 85.2 ms: 1.09x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 176 ms: 1.08x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.48 sec: 1.08x faster                                                      |
| deepcopy_reduce            | 2.06 us                                                     | 1.94 us: 1.06x faster                                                       |
| pycparser                  | 720 ms                                                      | 681 ms: 1.06x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 17.6 us: 1.05x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.4 ms: 1.05x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 65.3 ms: 1.05x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 836 us: 1.04x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 93.6 ms: 1.04x faster                                                       |
| mypy2                      | 459 ms                                                      | 441 ms: 1.04x faster                                                        |
| sympy_expand               | 299 ms                                                      | 287 ms: 1.04x faster                                                        |
| pyflate                    | 312 ms                                                      | 301 ms: 1.04x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.8 ms: 1.03x faster                                                       |
| meteor_contest             | 75.2 ms                                                     | 73.4 ms: 1.02x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 518 ms: 1.02x faster                                                        |
| richards                   | 31.4 ms                                                     | 30.8 ms: 1.02x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.07 sec: 1.02x faster                                                      |
| docutils                   | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                      |
| go                         | 101 ms                                                      | 99.5 ms: 1.02x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.9 ms: 1.01x faster                                                       |
| regex_dna                  | 116 ms                                                      | 116 ms: 1.00x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 35.0 ms: 1.01x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 46.6 ms: 1.03x slower                                                       |
| fannkuch                   | 253 ms                                                      | 261 ms: 1.03x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 54.3 ms: 1.03x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.55 ms: 1.03x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 740 us: 1.04x slower                                                        |
| coverage                   | 43.4 ms                                                     | 45.7 ms: 1.05x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.73 us: 1.05x slower                                                       |
| 2to3                       | 214 ms                                                      | 226 ms: 1.06x slower                                                        |
| pathlib                    | 70.9 ms                                                     | 75.2 ms: 1.06x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.9 us: 1.07x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.94 us: 1.09x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.33 us: 1.10x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.04 ms: 1.11x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 87.3 ms: 1.12x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.46 us: 1.12x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.70 ms: 1.16x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 73.4 ms: 1.16x slower                                                       |
| scimark_lu                 | 62.8 ms                                                     | 74.0 ms: 1.18x slower                                                       |
| unpack_sequence            | 46.9 ns                                                     | 57.1 ns: 1.22x slower                                                       |
| python_startup             | 19.8 ms                                                     | 24.3 ms: 1.23x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 22.2 ms: 1.32x slower                                                       |
| dask                       | 273 ms                                                      | 360 ms: 1.32x slower                                                        |
| async_generators           | 177 ms                                                      | 247 ms: 1.40x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.07x faster                                                                |

Benchmark hidden because not significant (5): regex_compile, pidigits, scimark_fft, gc_traversal, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown