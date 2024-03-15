
# Results vs. 3.11.0

- fork: python
- ref: v3.11.5
- machine: linux-x86_64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.00x slower \*
- HPT reliability: 69.97%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 285 ms: 1.01x faster                                         |
| chameleon      | 7.92 ms                                                      | 7.28 ms: 1.09x faster                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                 |

Benchmark hidden because not significant (3): docutils, html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 753 ms                                                       | 765 ms: 1.02x slower                                         |
| Geometric mean          | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (3): async_tree_memoization, async_tree_none, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 90.5 ms: 1.03x faster                                        |
| float          | 74.9 ms                                                      | 74.3 ms: 1.01x faster                                        |
| pidigits       | 251 ms                                                       | 251 ms: 1.00x faster                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 24.2 ms: 1.01x faster                                        |
| regex_effbot   | 3.34 ms                                                      | 3.31 ms: 1.01x faster                                        |
| regex_compile  | 156 ms                                                       | 155 ms: 1.01x faster                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_loads           | 28.9 us                                                      | 27.9 us: 1.04x faster                                        |
| xml_etree_iterparse  | 107 ms                                                       | 103 ms: 1.04x faster                                         |
| xml_etree_process    | 55.9 ms                                                      | 56.1 ms: 1.00x slower                                        |
| pickle               | 9.89 us                                                      | 9.98 us: 1.01x slower                                        |
| unpickle_pure_python | 238 us                                                       | 241 us: 1.01x slower                                         |
| pickle_pure_python   | 316 us                                                       | 320 us: 1.01x slower                                         |
| xml_etree_generate   | 79.7 ms                                                      | 80.8 ms: 1.01x slower                                        |
| json_dumps           | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                        |
| pickle_dict          | 32.3 us                                                      | 33.1 us: 1.02x slower                                        |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (5): pickle_list, unpickle, unpickle_list, xml_etree_parse, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.8 ms: 1.00x slower                                        |
| python_startup_no_site | 7.73 ms                                                      | 7.79 ms: 1.01x slower                                        |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.6 ms: 1.03x faster                                        |
| genshi_xml      | 57.1 ms                                                      | 55.7 ms: 1.02x faster                                        |
| django_template | 39.3 ms                                                      | 40.7 ms: 1.04x slower                                        |
| Geometric mean  | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| gc_traversal             | 4.15 ms                                                      | 3.77 ms: 1.10x faster                                        |
| chameleon                | 7.92 ms                                                      | 7.28 ms: 1.09x faster                                        |
| pprint_safe_repr         | 805 ms                                                       | 775 ms: 1.04x faster                                         |
| json_loads               | 28.9 us                                                      | 27.9 us: 1.04x faster                                        |
| xml_etree_iterparse      | 107 ms                                                       | 103 ms: 1.04x faster                                         |
| pprint_pformat           | 1.67 sec                                                     | 1.61 sec: 1.04x faster                                       |
| mako                     | 11.0 ms                                                      | 10.6 ms: 1.03x faster                                        |
| dulwich_log              | 67.4 ms                                                      | 65.3 ms: 1.03x faster                                        |
| nbody                    | 92.9 ms                                                      | 90.5 ms: 1.03x faster                                        |
| typing_runtime_protocols | 532 us                                                       | 518 us: 1.03x faster                                         |
| genshi_xml               | 57.1 ms                                                      | 55.7 ms: 1.02x faster                                        |
| crypto_pyaes             | 83.3 ms                                                      | 81.7 ms: 1.02x faster                                        |
| pyflate                  | 449 ms                                                       | 441 ms: 1.02x faster                                         |
| spectral_norm            | 95.1 ms                                                      | 93.3 ms: 1.02x faster                                        |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.00 ms: 1.02x faster                                        |
| flaskblogging            | 3.88 ms                                                      | 3.83 ms: 1.01x faster                                        |
| sqlalchemy_imperative    | 19.8 ms                                                      | 19.5 ms: 1.01x faster                                        |
| async_generators         | 322 ms                                                       | 318 ms: 1.01x faster                                         |
| scimark_monte_carlo      | 69.8 ms                                                      | 69.0 ms: 1.01x faster                                        |
| regex_v8                 | 24.4 ms                                                      | 24.2 ms: 1.01x faster                                        |
| telco                    | 6.81 ms                                                      | 6.75 ms: 1.01x faster                                        |
| nqueens                  | 103 ms                                                       | 102 ms: 1.01x faster                                         |
| float                    | 74.9 ms                                                      | 74.3 ms: 1.01x faster                                        |
| regex_effbot             | 3.34 ms                                                      | 3.31 ms: 1.01x faster                                        |
| sympy_integrate          | 25.8 ms                                                      | 25.6 ms: 1.01x faster                                        |
| sympy_sum                | 186 ms                                                       | 184 ms: 1.01x faster                                         |
| 2to3                     | 287 ms                                                       | 285 ms: 1.01x faster                                         |
| regex_compile            | 156 ms                                                       | 155 ms: 1.01x faster                                         |
| sympy_str                | 337 ms                                                       | 336 ms: 1.00x faster                                         |
| pidigits                 | 251 ms                                                       | 251 ms: 1.00x faster                                         |
| mdp                      | 2.77 sec                                                     | 2.78 sec: 1.00x slower                                       |
| sympy_expand             | 553 ms                                                       | 555 ms: 1.00x slower                                         |
| python_startup           | 10.7 ms                                                      | 10.8 ms: 1.00x slower                                        |
| meteor_contest           | 131 ms                                                       | 131 ms: 1.00x slower                                         |
| xml_etree_process        | 55.9 ms                                                      | 56.1 ms: 1.00x slower                                        |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 3.08 sec: 1.01x slower                                       |
| python_startup_no_site   | 7.73 ms                                                      | 7.79 ms: 1.01x slower                                        |
| pickle                   | 9.89 us                                                      | 9.98 us: 1.01x slower                                        |
| asyncio_tcp              | 747 ms                                                       | 753 ms: 1.01x slower                                         |
| unpickle_pure_python     | 238 us                                                       | 241 us: 1.01x slower                                         |
| pycparser                | 1.31 sec                                                     | 1.32 sec: 1.01x slower                                       |
| richards_super           | 63.6 ms                                                      | 64.3 ms: 1.01x slower                                        |
| pickle_pure_python       | 316 us                                                       | 320 us: 1.01x slower                                         |
| deepcopy                 | 391 us                                                       | 396 us: 1.01x slower                                         |
| sqlite_synth             | 2.52 us                                                      | 2.55 us: 1.01x slower                                        |
| xml_etree_generate       | 79.7 ms                                                      | 80.8 ms: 1.01x slower                                        |
| generators               | 54.6 ms                                                      | 55.4 ms: 1.01x slower                                        |
| scimark_sor              | 110 ms                                                       | 111 ms: 1.01x slower                                         |
| deltablue                | 3.97 ms                                                      | 4.03 ms: 1.01x slower                                        |
| async_tree_cpu_io_mixed  | 753 ms                                                       | 765 ms: 1.02x slower                                         |
| logging_format           | 7.71 us                                                      | 7.83 us: 1.02x slower                                        |
| sqlglot_parse            | 1.51 ms                                                      | 1.54 ms: 1.02x slower                                        |
| json_dumps               | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                        |
| sqlglot_normalize        | 122 ms                                                       | 124 ms: 1.02x slower                                         |
| pickle_dict              | 32.3 us                                                      | 33.1 us: 1.02x slower                                        |
| create_gc_cycles         | 1.58 ms                                                      | 1.62 ms: 1.03x slower                                        |
| unpack_sequence          | 45.7 ns                                                      | 46.9 ns: 1.03x slower                                        |
| raytrace                 | 309 ms                                                       | 318 ms: 1.03x slower                                         |
| go                       | 158 ms                                                       | 163 ms: 1.03x slower                                         |
| hexiom                   | 6.98 ms                                                      | 7.21 ms: 1.03x slower                                        |
| gunicorn                 | 966 us                                                       | 999 us: 1.03x slower                                         |
| django_template          | 39.3 ms                                                      | 40.7 ms: 1.04x slower                                        |
| richards                 | 49.7 ms                                                      | 51.6 ms: 1.04x slower                                        |
| chaos                    | 74.9 ms                                                      | 79.1 ms: 1.06x slower                                        |
| thrift                   | 931 us                                                       | 986 us: 1.06x slower                                         |
| fannkuch                 | 416 ms                                                       | 470 ms: 1.13x slower                                         |
| Geometric mean           | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (31): html5lib, bench_thread_pool, async_tree_memoization, tornado_http, scimark_lu, json, deepcopy_memo, docutils, coroutines, logging_silent, sqlglot_optimize, scimark_fft, regex_dna, dask, sqlalchemy_declarative, comprehensions, async_tree_none, genshi_text, sqlglot_transpile, pickle_list, unpickle, async_tree_io, deepcopy_reduce, pathlib, aiohttp, pylint, unpickle_list, bench_mp_pool, logging_simple, xml_etree_parse, tomli_loads
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 69.97% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x