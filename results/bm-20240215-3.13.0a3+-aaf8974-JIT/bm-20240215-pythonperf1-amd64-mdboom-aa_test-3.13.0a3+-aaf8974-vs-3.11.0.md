
# Results vs. 3.11.0

- fork: mdboom
- ref: aa_test
- machine: windows-amd64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 215 ms: 1.01x slower                                           |
| chameleon      | 5.26 ms                                                     | 4.78 ms: 1.10x faster                                          |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                         |
| tornado_http   | 92.8 ms                                                     | 84.9 ms: 1.09x faster                                          |
| Geometric mean | (ref)                                                       | 1.06x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 262 ms: 1.27x faster                                           |
| async_tree_memoization     | 399 ms                                                      | 336 ms: 1.19x faster                                           |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 447 ms: 1.19x faster                                           |
| async_tree_memoization_tg  | 405 ms                                                      | 345 ms: 1.17x faster                                           |
| async_tree_none_tg         | 309 ms                                                      | 271 ms: 1.14x faster                                           |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 464 ms: 1.13x faster                                           |
| async_tree_io              | 808 ms                                                      | 720 ms: 1.12x faster                                           |
| async_tree_io_tg           | 829 ms                                                      | 753 ms: 1.10x faster                                           |
| Geometric mean             | (ref)                                                       | 1.16x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 60.7 ms: 1.16x faster                                          |
| float          | 54.4 ms                                                     | 50.3 ms: 1.08x faster                                          |
| pidigits       | 150 ms                                                      | 152 ms: 1.01x slower                                           |
| Geometric mean | (ref)                                                       | 1.07x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 80.4 ms: 1.13x faster                                          |
| regex_dna      | 116 ms                                                      | 115 ms: 1.01x faster                                           |
| regex_v8       | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                          |
| regex_effbot   | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                          |
| Geometric mean | (ref)                                                       | 1.02x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.55 ms: 1.46x faster                                          |
| unpickle_pure_python | 157 us                                                      | 127 us: 1.23x faster                                           |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                           |
| tomli_loads          | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                         |
| pickle_dict          | 18.5 us                                                     | 17.4 us: 1.06x faster                                          |
| xml_etree_parse      | 97.6 ms                                                     | 93.1 ms: 1.05x faster                                          |
| xml_etree_process    | 37.2 ms                                                     | 36.1 ms: 1.03x faster                                          |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.8 ms: 1.03x faster                                          |
| xml_etree_generate   | 52.5 ms                                                     | 52.0 ms: 1.01x faster                                          |
| pickle_list          | 2.70 us                                                     | 2.78 us: 1.03x slower                                          |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.05x slower                                          |
| unpickle_list        | 2.59 us                                                     | 2.76 us: 1.07x slower                                          |
| pickle               | 6.64 us                                                     | 7.31 us: 1.10x slower                                          |
| unpickle             | 7.57 us                                                     | 8.63 us: 1.14x slower                                          |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.1 ms: 1.02x slower                                          |
| python_startup_no_site | 16.8 ms                                                     | 18.1 ms: 1.08x slower                                          |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.71 ms: 1.13x faster                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 69.8 us: 4.67x faster                                          |
| generators                 | 34.0 ms                                                     | 20.6 ms: 1.65x faster                                          |
| asyncio_tcp                | 726 ms                                                      | 466 ms: 1.56x faster                                           |
| json_dumps                 | 8.09 ms                                                     | 5.55 ms: 1.46x faster                                          |
| comprehensions             | 15.6 us                                                     | 10.7 us: 1.46x faster                                          |
| deltablue                  | 2.70 ms                                                     | 1.98 ms: 1.37x faster                                          |
| richards_super             | 38.7 ms                                                     | 28.5 ms: 1.36x faster                                          |
| logging_silent             | 71.8 ns                                                     | 54.2 ns: 1.32x faster                                          |
| async_tree_none            | 332 ms                                                      | 262 ms: 1.27x faster                                           |
| raytrace                   | 213 ms                                                      | 169 ms: 1.26x faster                                           |
| sqlglot_parse              | 953 us                                                      | 761 us: 1.25x faster                                           |
| unpickle_pure_python       | 157 us                                                      | 127 us: 1.23x faster                                           |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.65 sec: 1.23x faster                                         |
| deepcopy_memo              | 26.0 us                                                     | 21.6 us: 1.20x faster                                          |
| unpack_sequence            | 46.9 ns                                                     | 39.3 ns: 1.19x faster                                          |
| sqlglot_transpile          | 1.16 ms                                                     | 976 us: 1.19x faster                                           |
| richards                   | 31.4 ms                                                     | 26.4 ms: 1.19x faster                                          |
| pickle_pure_python         | 208 us                                                      | 175 us: 1.19x faster                                           |
| async_tree_memoization     | 399 ms                                                      | 336 ms: 1.19x faster                                           |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 447 ms: 1.19x faster                                           |
| sqlite_synth               | 1.77 us                                                     | 1.49 us: 1.18x faster                                          |
| async_tree_memoization_tg  | 405 ms                                                      | 345 ms: 1.17x faster                                           |
| coroutines                 | 15.0 ms                                                     | 12.8 ms: 1.17x faster                                          |
| logging_simple             | 6.86 us                                                     | 5.89 us: 1.17x faster                                          |
| nbody                      | 70.3 ms                                                     | 60.7 ms: 1.16x faster                                          |
| dulwich_log                | 46.4 ms                                                     | 40.3 ms: 1.15x faster                                          |
| chaos                      | 48.4 ms                                                     | 42.2 ms: 1.15x faster                                          |
| sympy_sum                  | 100 ms                                                      | 87.9 ms: 1.14x faster                                          |
| async_tree_none_tg         | 309 ms                                                      | 271 ms: 1.14x faster                                           |
| nqueens                    | 68.3 ms                                                     | 60.2 ms: 1.14x faster                                          |
| regex_compile              | 91.0 ms                                                     | 80.4 ms: 1.13x faster                                          |
| mako                       | 7.58 ms                                                     | 6.71 ms: 1.13x faster                                          |
| deepcopy                   | 246 us                                                      | 219 us: 1.13x faster                                           |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 464 ms: 1.13x faster                                           |
| sympy_str                  | 185 ms                                                      | 164 ms: 1.13x faster                                           |
| async_tree_io              | 808 ms                                                      | 720 ms: 1.12x faster                                           |
| logging_format             | 7.16 us                                                     | 6.39 us: 1.12x faster                                          |
| tomli_loads                | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                         |
| pprint_pformat             | 1.09 sec                                                    | 983 ms: 1.11x faster                                           |
| pprint_safe_repr           | 529 ms                                                      | 480 ms: 1.10x faster                                           |
| chameleon                  | 5.26 ms                                                     | 4.78 ms: 1.10x faster                                          |
| async_tree_io_tg           | 829 ms                                                      | 753 ms: 1.10x faster                                           |
| scimark_lu                 | 62.8 ms                                                     | 57.2 ms: 1.10x faster                                          |
| tornado_http               | 92.8 ms                                                     | 84.9 ms: 1.09x faster                                          |
| sqlglot_normalize          | 190 ms                                                      | 174 ms: 1.09x faster                                           |
| sympy_integrate            | 14.0 ms                                                     | 12.9 ms: 1.09x faster                                          |
| mypy2                      | 459 ms                                                      | 422 ms: 1.09x faster                                           |
| fannkuch                   | 253 ms                                                      | 234 ms: 1.08x faster                                           |
| float                      | 54.4 ms                                                     | 50.3 ms: 1.08x faster                                          |
| deepcopy_reduce            | 2.06 us                                                     | 1.91 us: 1.08x faster                                          |
| dask                       | 273 ms                                                      | 254 ms: 1.08x faster                                           |
| sympy_expand               | 299 ms                                                      | 281 ms: 1.06x faster                                           |
| pickle_dict                | 18.5 us                                                     | 17.4 us: 1.06x faster                                          |
| go                         | 101 ms                                                      | 95.8 ms: 1.06x faster                                          |
| spectral_norm              | 68.3 ms                                                     | 64.8 ms: 1.05x faster                                          |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                         |
| xml_etree_parse            | 97.6 ms                                                     | 93.1 ms: 1.05x faster                                          |
| crypto_pyaes               | 48.9 ms                                                     | 46.7 ms: 1.05x faster                                          |
| xml_etree_process          | 37.2 ms                                                     | 36.1 ms: 1.03x faster                                          |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.8 ms: 1.03x faster                                          |
| mdp                        | 1.59 sec                                                    | 1.55 sec: 1.03x faster                                         |
| sqlglot_optimize           | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                          |
| xml_etree_generate         | 52.5 ms                                                     | 52.0 ms: 1.01x faster                                          |
| regex_dna                  | 116 ms                                                      | 115 ms: 1.01x faster                                           |
| 2to3                       | 214 ms                                                      | 215 ms: 1.01x slower                                           |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                          |
| scimark_sor                | 78.1 ms                                                     | 78.9 ms: 1.01x slower                                          |
| pidigits                   | 150 ms                                                      | 152 ms: 1.01x slower                                           |
| regex_v8                   | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                          |
| meteor_contest             | 75.2 ms                                                     | 76.3 ms: 1.02x slower                                          |
| python_startup             | 19.8 ms                                                     | 20.1 ms: 1.02x slower                                          |
| pickle_list                | 2.70 us                                                     | 2.78 us: 1.03x slower                                          |
| regex_effbot               | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                          |
| create_gc_cycles           | 713 us                                                      | 741 us: 1.04x slower                                           |
| bench_mp_pool              | 63.2 ms                                                     | 66.2 ms: 1.05x slower                                          |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.71 ms: 1.05x slower                                          |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.05x slower                                          |
| pathlib                    | 70.9 ms                                                     | 74.8 ms: 1.06x slower                                          |
| coverage                   | 43.4 ms                                                     | 45.9 ms: 1.06x slower                                          |
| unpickle_list              | 2.59 us                                                     | 2.76 us: 1.07x slower                                          |
| scimark_fft                | 179 ms                                                      | 191 ms: 1.07x slower                                           |
| python_startup_no_site     | 16.8 ms                                                     | 18.1 ms: 1.08x slower                                          |
| pickle                     | 6.64 us                                                     | 7.31 us: 1.10x slower                                          |
| telco                      | 4.06 ms                                                     | 4.59 ms: 1.13x slower                                          |
| unpickle                   | 7.57 us                                                     | 8.63 us: 1.14x slower                                          |
| hexiom                     | 4.55 ms                                                     | 5.29 ms: 1.16x slower                                          |
| scimark_monte_carlo        | 45.3 ms                                                     | 56.8 ms: 1.25x slower                                          |
| async_generators           | 177 ms                                                      | 241 ms: 1.36x slower                                           |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                   |

Benchmark hidden because not significant (4): bench_thread_pool, pyflate, pycparser, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown