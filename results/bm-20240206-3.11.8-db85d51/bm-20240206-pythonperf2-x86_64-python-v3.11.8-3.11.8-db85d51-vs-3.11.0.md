
# Results vs. 3.11.0

- fork: python
- ref: v3.11.8
- machine: linux-x86_64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.00x faster \*
- HPT reliability: 98.10%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 283 ms: 1.01x faster                                         |
| chameleon      | 7.92 ms                                                      | 7.43 ms: 1.07x faster                                        |
| docutils       | 2.85 sec                                                     | 2.82 sec: 1.01x faster                                       |
| html5lib       | 72.2 ms                                                      | 71.2 ms: 1.01x faster                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_memoization_tg  | 600 ms                                                       | 592 ms: 1.01x faster                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 744 ms: 1.01x faster                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.15 sec: 1.01x faster                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 748 ms: 1.01x faster                                         |
| async_tree_none            | 518 ms                                                       | 523 ms: 1.01x slower                                         |
| async_tree_memoization     | 629 ms                                                       | 636 ms: 1.01x slower                                         |
| Geometric mean             | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (2): async_tree_none_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 96.9 ms: 1.04x slower                                        |
| pidigits       | 251 ms                                                       | 268 ms: 1.07x slower                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                 |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.27 ms: 1.02x faster                                        |
| regex_compile  | 156 ms                                                       | 153 ms: 1.02x faster                                         |
| regex_dna      | 227 ms                                                       | 227 ms: 1.00x faster                                         |
| regex_v8       | 24.4 ms                                                      | 24.5 ms: 1.00x slower                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|---------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_loads          | 28.9 us                                                      | 25.1 us: 1.15x faster                                        |
| unpickle_list       | 4.60 us                                                      | 4.51 us: 1.02x faster                                        |
| xml_etree_iterparse | 107 ms                                                       | 105 ms: 1.02x faster                                         |
| pickle_list         | 3.94 us                                                      | 3.90 us: 1.01x faster                                        |
| xml_etree_process   | 55.9 ms                                                      | 56.2 ms: 1.01x slower                                        |
| json_dumps          | 13.3 ms                                                      | 13.4 ms: 1.01x slower                                        |
| tomli_loads         | 2.25 sec                                                     | 2.28 sec: 1.01x slower                                       |
| xml_etree_generate  | 79.7 ms                                                      | 80.9 ms: 1.01x slower                                        |
| pickle_pure_python  | 316 us                                                       | 322 us: 1.02x slower                                         |
| pickle              | 9.89 us                                                      | 10.3 us: 1.04x slower                                        |
| pickle_dict         | 32.3 us                                                      | 34.4 us: 1.06x slower                                        |
| Geometric mean      | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (3): xml_etree_parse, unpickle, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.69 ms: 1.01x faster                                        |
| python_startup         | 10.7 ms                                                      | 10.7 ms: 1.00x faster                                        |
| Geometric mean         | (ref)                                                        | 1.00x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.8 ms: 1.02x faster                                        |
| genshi_xml      | 57.1 ms                                                      | 55.9 ms: 1.02x faster                                        |
| django_template | 39.3 ms                                                      | 40.3 ms: 1.03x slower                                        |
| Geometric mean  | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| gc_traversal               | 4.15 ms                                                      | 3.46 ms: 1.20x faster                                        |
| json_loads                 | 28.9 us                                                      | 25.1 us: 1.15x faster                                        |
| chameleon                  | 7.92 ms                                                      | 7.43 ms: 1.07x faster                                        |
| json                       | 5.58 ms                                                      | 5.26 ms: 1.06x faster                                        |
| pylint                     | 514 ms                                                       | 496 ms: 1.04x faster                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 67.5 ms: 1.03x faster                                        |
| comprehensions             | 25.1 us                                                      | 24.4 us: 1.03x faster                                        |
| telco                      | 6.81 ms                                                      | 6.62 ms: 1.03x faster                                        |
| richards_super             | 63.6 ms                                                      | 61.9 ms: 1.03x faster                                        |
| pyflate                    | 449 ms                                                       | 438 ms: 1.02x faster                                         |
| pprint_safe_repr           | 805 ms                                                       | 785 ms: 1.02x faster                                         |
| scimark_fft                | 281 ms                                                       | 274 ms: 1.02x faster                                         |
| mako                       | 11.0 ms                                                      | 10.8 ms: 1.02x faster                                        |
| logging_simple             | 7.24 us                                                      | 7.08 us: 1.02x faster                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.63 sec: 1.02x faster                                       |
| regex_effbot               | 3.34 ms                                                      | 3.27 ms: 1.02x faster                                        |
| regex_compile              | 156 ms                                                       | 153 ms: 1.02x faster                                         |
| genshi_xml                 | 57.1 ms                                                      | 55.9 ms: 1.02x faster                                        |
| typing_runtime_protocols   | 532 us                                                       | 522 us: 1.02x faster                                         |
| unpickle_list              | 4.60 us                                                      | 4.51 us: 1.02x faster                                        |
| xml_etree_iterparse        | 107 ms                                                       | 105 ms: 1.02x faster                                         |
| sympy_sum                  | 186 ms                                                       | 182 ms: 1.02x faster                                         |
| deepcopy                   | 391 us                                                       | 384 us: 1.02x faster                                         |
| sympy_integrate            | 25.8 ms                                                      | 25.4 ms: 1.02x faster                                        |
| asyncio_tcp                | 747 ms                                                       | 735 ms: 1.02x faster                                         |
| mypy2                      | 762 ms                                                       | 751 ms: 1.01x faster                                         |
| html5lib                   | 72.2 ms                                                      | 71.2 ms: 1.01x faster                                        |
| 2to3                       | 287 ms                                                       | 283 ms: 1.01x faster                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.01 ms: 1.01x faster                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 592 ms: 1.01x faster                                         |
| aiohttp                    | 986 us                                                       | 974 us: 1.01x faster                                         |
| flaskblogging              | 3.88 ms                                                      | 3.83 ms: 1.01x faster                                        |
| sympy_str                  | 337 ms                                                       | 333 ms: 1.01x faster                                         |
| meteor_contest             | 131 ms                                                       | 129 ms: 1.01x faster                                         |
| async_generators           | 322 ms                                                       | 318 ms: 1.01x faster                                         |
| thrift                     | 931 us                                                       | 922 us: 1.01x faster                                         |
| pickle_list                | 3.94 us                                                      | 3.90 us: 1.01x faster                                        |
| docutils                   | 2.85 sec                                                     | 2.82 sec: 1.01x faster                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 744 ms: 1.01x faster                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.15 sec: 1.01x faster                                       |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 3.04 sec: 1.01x faster                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 748 ms: 1.01x faster                                         |
| pathlib                    | 18.9 ms                                                      | 18.8 ms: 1.01x faster                                        |
| coroutines                 | 27.8 ms                                                      | 27.6 ms: 1.01x faster                                        |
| python_startup_no_site     | 7.73 ms                                                      | 7.69 ms: 1.01x faster                                        |
| regex_dna                  | 227 ms                                                       | 227 ms: 1.00x faster                                         |
| python_startup             | 10.7 ms                                                      | 10.7 ms: 1.00x faster                                        |
| regex_v8                   | 24.4 ms                                                      | 24.5 ms: 1.00x slower                                        |
| sqlglot_normalize          | 122 ms                                                       | 122 ms: 1.01x slower                                         |
| xml_etree_process          | 55.9 ms                                                      | 56.2 ms: 1.01x slower                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.93 ms: 1.01x slower                                        |
| json_dumps                 | 13.3 ms                                                      | 13.4 ms: 1.01x slower                                        |
| gunicorn                   | 966 us                                                       | 976 us: 1.01x slower                                         |
| async_tree_none            | 518 ms                                                       | 523 ms: 1.01x slower                                         |
| async_tree_memoization     | 629 ms                                                       | 636 ms: 1.01x slower                                         |
| crypto_pyaes               | 83.3 ms                                                      | 84.3 ms: 1.01x slower                                        |
| nqueens                    | 103 ms                                                       | 104 ms: 1.01x slower                                         |
| tomli_loads                | 2.25 sec                                                     | 2.28 sec: 1.01x slower                                       |
| xml_etree_generate         | 79.7 ms                                                      | 80.9 ms: 1.01x slower                                        |
| hexiom                     | 6.98 ms                                                      | 7.08 ms: 1.01x slower                                        |
| logging_silent             | 100 ns                                                       | 102 ns: 1.02x slower                                         |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.02x slower                                       |
| pickle_pure_python         | 316 us                                                       | 322 us: 1.02x slower                                         |
| deltablue                  | 3.97 ms                                                      | 4.06 ms: 1.02x slower                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.55 ms: 1.03x slower                                        |
| spectral_norm              | 95.1 ms                                                      | 97.5 ms: 1.03x slower                                        |
| sqlalchemy_imperative      | 19.8 ms                                                      | 20.3 ms: 1.03x slower                                        |
| django_template            | 39.3 ms                                                      | 40.3 ms: 1.03x slower                                        |
| scimark_sor                | 110 ms                                                       | 113 ms: 1.03x slower                                         |
| pickle                     | 9.89 us                                                      | 10.3 us: 1.04x slower                                        |
| nbody                      | 92.9 ms                                                      | 96.9 ms: 1.04x slower                                        |
| mdp                        | 2.77 sec                                                     | 2.92 sec: 1.05x slower                                       |
| chaos                      | 74.9 ms                                                      | 79.0 ms: 1.05x slower                                        |
| go                         | 158 ms                                                       | 167 ms: 1.06x slower                                         |
| pickle_dict                | 32.3 us                                                      | 34.4 us: 1.06x slower                                        |
| fannkuch                   | 416 ms                                                       | 442 ms: 1.06x slower                                         |
| pidigits                   | 251 ms                                                       | 268 ms: 1.07x slower                                         |
| Geometric mean             | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (27): bench_mp_pool, dask, tornado_http, unpack_sequence, genshi_text, dulwich_log, sqlalchemy_declarative, bench_thread_pool, richards, sqlglot_optimize, asyncio_websockets, async_tree_none_tg, coverage, float, async_tree_io, sqlite_synth, generators, logging_format, sympy_expand, scimark_lu, xml_etree_parse, unpickle, raytrace, create_gc_cycles, deepcopy_memo, unpickle_pure_python, deepcopy_reduce


# HPT report

- Reliability score: 98.10% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x