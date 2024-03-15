
# Results vs. 3.11.0

- fork: python
- ref: v3.11.6
- machine: linux-x86_64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.00x faster \*
- HPT reliability: 93.80%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 285 ms: 1.00x faster                                         |
| chameleon      | 7.92 ms                                                      | 7.64 ms: 1.04x faster                                        |
| docutils       | 2.85 sec                                                     | 2.83 sec: 1.00x faster                                       |
| tornado_http   | 124 ms                                                       | 123 ms: 1.01x faster                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_memoization | 629 ms                                                       | 622 ms: 1.01x faster                                         |
| Geometric mean         | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_io, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 76.4 ms: 1.02x slower                                        |
| nbody          | 92.9 ms                                                      | 96.9 ms: 1.04x slower                                        |
| pidigits       | 251 ms                                                       | 268 ms: 1.07x slower                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 23.2 ms: 1.05x faster                                        |
| regex_dna      | 227 ms                                                       | 220 ms: 1.04x faster                                         |
| regex_effbot   | 3.34 ms                                                      | 3.29 ms: 1.02x faster                                        |
| regex_compile  | 156 ms                                                       | 157 ms: 1.00x slower                                         |
| Geometric mean | (ref)                                                        | 1.03x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|---------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_loads          | 28.9 us                                                      | 24.6 us: 1.18x faster                                        |
| pickle_list         | 3.94 us                                                      | 3.77 us: 1.04x faster                                        |
| xml_etree_iterparse | 107 ms                                                       | 105 ms: 1.01x faster                                         |
| pickle_dict         | 32.3 us                                                      | 32.1 us: 1.01x faster                                        |
| pickle_pure_python  | 316 us                                                       | 315 us: 1.00x faster                                         |
| pickle              | 9.89 us                                                      | 9.99 us: 1.01x slower                                        |
| tomli_loads         | 2.25 sec                                                     | 2.28 sec: 1.01x slower                                       |
| unpickle_list       | 4.60 us                                                      | 4.69 us: 1.02x slower                                        |
| xml_etree_parse     | 155 ms                                                       | 159 ms: 1.03x slower                                         |
| Geometric mean      | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (5): xml_etree_process, xml_etree_generate, unpickle_pure_python, unpickle, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.8 ms: 1.01x slower                                        |
| python_startup_no_site | 7.73 ms                                                      | 7.81 ms: 1.01x slower                                        |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.8 ms: 1.02x faster                                        |
| genshi_xml      | 57.1 ms                                                      | 56.3 ms: 1.01x faster                                        |
| django_template | 39.3 ms                                                      | 40.5 ms: 1.03x slower                                        |
| Geometric mean  | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_loads               | 28.9 us                                                      | 24.6 us: 1.18x faster                                        |
| json                     | 5.58 ms                                                      | 5.23 ms: 1.07x faster                                        |
| regex_v8                 | 24.4 ms                                                      | 23.2 ms: 1.05x faster                                        |
| pickle_list              | 3.94 us                                                      | 3.77 us: 1.04x faster                                        |
| gc_traversal             | 4.15 ms                                                      | 3.97 ms: 1.04x faster                                        |
| logging_simple           | 7.24 us                                                      | 6.96 us: 1.04x faster                                        |
| pprint_safe_repr         | 805 ms                                                       | 775 ms: 1.04x faster                                         |
| chameleon                | 7.92 ms                                                      | 7.64 ms: 1.04x faster                                        |
| regex_dna                | 227 ms                                                       | 220 ms: 1.04x faster                                         |
| pprint_pformat           | 1.67 sec                                                     | 1.61 sec: 1.03x faster                                       |
| dulwich_log              | 67.4 ms                                                      | 65.3 ms: 1.03x faster                                        |
| raytrace                 | 309 ms                                                       | 301 ms: 1.03x faster                                         |
| pycparser                | 1.31 sec                                                     | 1.28 sec: 1.02x faster                                       |
| typing_runtime_protocols | 532 us                                                       | 519 us: 1.02x faster                                         |
| scimark_monte_carlo      | 69.8 ms                                                      | 68.3 ms: 1.02x faster                                        |
| chaos                    | 74.9 ms                                                      | 73.4 ms: 1.02x faster                                        |
| deepcopy                 | 391 us                                                       | 383 us: 1.02x faster                                         |
| meteor_contest           | 131 ms                                                       | 128 ms: 1.02x faster                                         |
| mako                     | 11.0 ms                                                      | 10.8 ms: 1.02x faster                                        |
| async_generators         | 322 ms                                                       | 316 ms: 1.02x faster                                         |
| regex_effbot             | 3.34 ms                                                      | 3.29 ms: 1.02x faster                                        |
| pyflate                  | 449 ms                                                       | 442 ms: 1.02x faster                                         |
| xml_etree_iterparse      | 107 ms                                                       | 105 ms: 1.01x faster                                         |
| genshi_xml               | 57.1 ms                                                      | 56.3 ms: 1.01x faster                                        |
| tornado_http             | 124 ms                                                       | 123 ms: 1.01x faster                                         |
| nqueens                  | 103 ms                                                       | 101 ms: 1.01x faster                                         |
| async_tree_memoization   | 629 ms                                                       | 622 ms: 1.01x faster                                         |
| crypto_pyaes             | 83.3 ms                                                      | 82.4 ms: 1.01x faster                                        |
| comprehensions           | 25.1 us                                                      | 24.8 us: 1.01x faster                                        |
| pickle_dict              | 32.3 us                                                      | 32.1 us: 1.01x faster                                        |
| generators               | 54.6 ms                                                      | 54.3 ms: 1.01x faster                                        |
| sqlglot_optimize         | 59.0 ms                                                      | 58.6 ms: 1.01x faster                                        |
| sympy_str                | 337 ms                                                       | 335 ms: 1.01x faster                                         |
| sympy_sum                | 186 ms                                                       | 184 ms: 1.01x faster                                         |
| sqlglot_normalize        | 122 ms                                                       | 121 ms: 1.01x faster                                         |
| sympy_expand             | 553 ms                                                       | 550 ms: 1.01x faster                                         |
| docutils                 | 2.85 sec                                                     | 2.83 sec: 1.00x faster                                       |
| 2to3                     | 287 ms                                                       | 285 ms: 1.00x faster                                         |
| pickle_pure_python       | 316 us                                                       | 315 us: 1.00x faster                                         |
| coroutines               | 27.8 ms                                                      | 27.9 ms: 1.00x slower                                        |
| regex_compile            | 156 ms                                                       | 157 ms: 1.00x slower                                         |
| sympy_integrate          | 25.8 ms                                                      | 25.9 ms: 1.00x slower                                        |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 3.09 sec: 1.01x slower                                       |
| python_startup           | 10.7 ms                                                      | 10.8 ms: 1.01x slower                                        |
| logging_silent           | 100 ns                                                       | 101 ns: 1.01x slower                                         |
| python_startup_no_site   | 7.73 ms                                                      | 7.81 ms: 1.01x slower                                        |
| pickle                   | 9.89 us                                                      | 9.99 us: 1.01x slower                                        |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.11 ms: 1.01x slower                                        |
| gunicorn                 | 966 us                                                       | 977 us: 1.01x slower                                         |
| pathlib                  | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                        |
| sqlglot_parse            | 1.51 ms                                                      | 1.53 ms: 1.01x slower                                        |
| tomli_loads              | 2.25 sec                                                     | 2.28 sec: 1.01x slower                                       |
| float                    | 74.9 ms                                                      | 76.4 ms: 1.02x slower                                        |
| scimark_fft              | 281 ms                                                       | 286 ms: 1.02x slower                                         |
| unpickle_list            | 4.60 us                                                      | 4.69 us: 1.02x slower                                        |
| create_gc_cycles         | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                        |
| spectral_norm            | 95.1 ms                                                      | 97.3 ms: 1.02x slower                                        |
| scimark_sor              | 110 ms                                                       | 112 ms: 1.02x slower                                         |
| go                       | 158 ms                                                       | 162 ms: 1.03x slower                                         |
| thrift                   | 931 us                                                       | 958 us: 1.03x slower                                         |
| xml_etree_parse          | 155 ms                                                       | 159 ms: 1.03x slower                                         |
| django_template          | 39.3 ms                                                      | 40.5 ms: 1.03x slower                                        |
| mdp                      | 2.77 sec                                                     | 2.86 sec: 1.03x slower                                       |
| nbody                    | 92.9 ms                                                      | 96.9 ms: 1.04x slower                                        |
| fannkuch                 | 416 ms                                                       | 437 ms: 1.05x slower                                         |
| pidigits                 | 251 ms                                                       | 268 ms: 1.07x slower                                         |
| Geometric mean           | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (31): sqlite_synth, dask, logging_format, html5lib, genshi_text, scimark_lu, async_tree_cpu_io_mixed, richards, unpack_sequence, telco, aiohttp, deepcopy_memo, sqlalchemy_imperative, hexiom, sqlglot_transpile, xml_etree_process, async_tree_io, deepcopy_reduce, asyncio_tcp, pylint, richards_super, flaskblogging, xml_etree_generate, unpickle_pure_python, unpickle, deltablue, bench_thread_pool, async_tree_none, sqlalchemy_declarative, json_dumps, bench_mp_pool
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 93.80% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x