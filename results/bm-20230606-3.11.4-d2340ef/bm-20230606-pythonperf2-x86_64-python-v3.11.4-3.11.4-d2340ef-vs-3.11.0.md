
# Results vs. 3.11.0

- fork: python
- ref: v3.11.4
- machine: linux-x86_64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.00x faster \*
- HPT reliability: 60.29%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 285 ms: 1.00x faster                                         |
| chameleon      | 7.92 ms                                                      | 7.63 ms: 1.04x faster                                        |
| docutils       | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                       |
| tornado_http   | 124 ms                                                       | 121 ms: 1.03x faster                                         |
| Geometric mean | (ref)                                                        | 1.02x faster                                                 |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_none | 518 ms                                                       | 522 ms: 1.01x slower                                         |
| Geometric mean  | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (3): async_tree_io, async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 73.8 ms: 1.02x faster                                        |
| pidigits       | 251 ms                                                       | 252 ms: 1.00x slower                                         |
| nbody          | 92.9 ms                                                      | 95.6 ms: 1.03x slower                                        |
| Geometric mean | (ref)                                                        | 1.00x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 155 ms: 1.01x faster                                         |
| regex_v8       | 24.4 ms                                                      | 24.5 ms: 1.00x slower                                        |
| regex_dna      | 227 ms                                                       | 231 ms: 1.01x slower                                         |
| regex_effbot   | 3.34 ms                                                      | 3.46 ms: 1.04x slower                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_dict          | 32.3 us                                                      | 29.7 us: 1.09x faster                                        |
| pickle_list          | 3.94 us                                                      | 3.70 us: 1.06x faster                                        |
| unpickle             | 13.3 us                                                      | 13.0 us: 1.02x faster                                        |
| xml_etree_iterparse  | 107 ms                                                       | 105 ms: 1.02x faster                                         |
| json_loads           | 28.9 us                                                      | 28.4 us: 1.02x faster                                        |
| xml_etree_process    | 55.9 ms                                                      | 56.3 ms: 1.01x slower                                        |
| tomli_loads          | 2.25 sec                                                     | 2.27 sec: 1.01x slower                                       |
| json_dumps           | 13.3 ms                                                      | 13.4 ms: 1.01x slower                                        |
| pickle_pure_python   | 316 us                                                       | 321 us: 1.01x slower                                         |
| xml_etree_generate   | 79.7 ms                                                      | 81.0 ms: 1.02x slower                                        |
| unpickle_list        | 4.60 us                                                      | 4.69 us: 1.02x slower                                        |
| unpickle_pure_python | 238 us                                                       | 243 us: 1.02x slower                                         |
| xml_etree_parse      | 155 ms                                                       | 159 ms: 1.03x slower                                         |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.7 ms: 1.01x faster                                        |
| python_startup_no_site | 7.73 ms                                                      | 7.72 ms: 1.00x faster                                        |
| Geometric mean         | (ref)                                                        | 1.00x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.8 ms: 1.02x faster                                        |
| django_template | 39.3 ms                                                      | 39.7 ms: 1.01x slower                                        |
| genshi_xml      | 57.1 ms                                                      | 57.9 ms: 1.02x slower                                        |
| Geometric mean  | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| gc_traversal             | 4.15 ms                                                      | 3.70 ms: 1.12x faster                                        |
| pickle_dict              | 32.3 us                                                      | 29.7 us: 1.09x faster                                        |
| pickle_list              | 3.94 us                                                      | 3.70 us: 1.06x faster                                        |
| nqueens                  | 103 ms                                                       | 98.5 ms: 1.04x faster                                        |
| chameleon                | 7.92 ms                                                      | 7.63 ms: 1.04x faster                                        |
| pprint_pformat           | 1.67 sec                                                     | 1.62 sec: 1.03x faster                                       |
| tornado_http             | 124 ms                                                       | 121 ms: 1.03x faster                                         |
| logging_simple           | 7.24 us                                                      | 7.05 us: 1.03x faster                                        |
| pprint_safe_repr         | 805 ms                                                       | 784 ms: 1.03x faster                                         |
| bench_mp_pool            | 4.70 ms                                                      | 4.58 ms: 1.03x faster                                        |
| unpickle                 | 13.3 us                                                      | 13.0 us: 1.02x faster                                        |
| thrift                   | 931 us                                                       | 912 us: 1.02x faster                                         |
| mako                     | 11.0 ms                                                      | 10.8 ms: 1.02x faster                                        |
| pycparser                | 1.31 sec                                                     | 1.28 sec: 1.02x faster                                       |
| xml_etree_iterparse      | 107 ms                                                       | 105 ms: 1.02x faster                                         |
| dask                     | 410 ms                                                       | 402 ms: 1.02x faster                                         |
| json                     | 5.58 ms                                                      | 5.48 ms: 1.02x faster                                        |
| json_loads               | 28.9 us                                                      | 28.4 us: 1.02x faster                                        |
| logging_format           | 7.71 us                                                      | 7.58 us: 1.02x faster                                        |
| sqlite_synth             | 2.52 us                                                      | 2.48 us: 1.02x faster                                        |
| float                    | 74.9 ms                                                      | 73.8 ms: 1.02x faster                                        |
| sympy_sum                | 186 ms                                                       | 183 ms: 1.01x faster                                         |
| scimark_sparse_mat_mult  | 4.06 ms                                                      | 4.01 ms: 1.01x faster                                        |
| typing_runtime_protocols | 532 us                                                       | 525 us: 1.01x faster                                         |
| deepcopy                 | 391 us                                                       | 387 us: 1.01x faster                                         |
| spectral_norm            | 95.1 ms                                                      | 94.1 ms: 1.01x faster                                        |
| sympy_str                | 337 ms                                                       | 334 ms: 1.01x faster                                         |
| telco                    | 6.81 ms                                                      | 6.75 ms: 1.01x faster                                        |
| python_startup           | 10.7 ms                                                      | 10.7 ms: 1.01x faster                                        |
| sympy_integrate          | 25.8 ms                                                      | 25.6 ms: 1.01x faster                                        |
| docutils                 | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                       |
| scimark_lu               | 114 ms                                                       | 113 ms: 1.01x faster                                         |
| regex_compile            | 156 ms                                                       | 155 ms: 1.01x faster                                         |
| sqlalchemy_imperative    | 19.8 ms                                                      | 19.6 ms: 1.01x faster                                        |
| comprehensions           | 25.1 us                                                      | 24.9 us: 1.01x faster                                        |
| aiohttp                  | 986 us                                                       | 980 us: 1.01x faster                                         |
| sympy_expand             | 553 ms                                                       | 550 ms: 1.01x faster                                         |
| 2to3                     | 287 ms                                                       | 285 ms: 1.00x faster                                         |
| meteor_contest           | 131 ms                                                       | 130 ms: 1.00x faster                                         |
| sqlglot_optimize         | 59.0 ms                                                      | 58.7 ms: 1.00x faster                                        |
| python_startup_no_site   | 7.73 ms                                                      | 7.72 ms: 1.00x faster                                        |
| asyncio_tcp_ssl          | 3.07 sec                                                     | 3.07 sec: 1.00x slower                                       |
| pidigits                 | 251 ms                                                       | 252 ms: 1.00x slower                                         |
| regex_v8                 | 24.4 ms                                                      | 24.5 ms: 1.00x slower                                        |
| asyncio_tcp              | 747 ms                                                       | 751 ms: 1.01x slower                                         |
| logging_silent           | 100 ns                                                       | 101 ns: 1.01x slower                                         |
| xml_etree_process        | 55.9 ms                                                      | 56.3 ms: 1.01x slower                                        |
| async_tree_none          | 518 ms                                                       | 522 ms: 1.01x slower                                         |
| tomli_loads              | 2.25 sec                                                     | 2.27 sec: 1.01x slower                                       |
| json_dumps               | 13.3 ms                                                      | 13.4 ms: 1.01x slower                                        |
| django_template          | 39.3 ms                                                      | 39.7 ms: 1.01x slower                                        |
| hexiom                   | 6.98 ms                                                      | 7.06 ms: 1.01x slower                                        |
| deepcopy_memo            | 37.5 us                                                      | 38.1 us: 1.01x slower                                        |
| regex_dna                | 227 ms                                                       | 231 ms: 1.01x slower                                         |
| pickle_pure_python       | 316 us                                                       | 321 us: 1.01x slower                                         |
| genshi_xml               | 57.1 ms                                                      | 57.9 ms: 1.02x slower                                        |
| gunicorn                 | 966 us                                                       | 981 us: 1.02x slower                                         |
| xml_etree_generate       | 79.7 ms                                                      | 81.0 ms: 1.02x slower                                        |
| pyflate                  | 449 ms                                                       | 458 ms: 1.02x slower                                         |
| unpickle_list            | 4.60 us                                                      | 4.69 us: 1.02x slower                                        |
| unpickle_pure_python     | 238 us                                                       | 243 us: 1.02x slower                                         |
| sqlglot_parse            | 1.51 ms                                                      | 1.55 ms: 1.02x slower                                        |
| deltablue                | 3.97 ms                                                      | 4.06 ms: 1.02x slower                                        |
| richards_super           | 63.6 ms                                                      | 65.2 ms: 1.02x slower                                        |
| xml_etree_parse          | 155 ms                                                       | 159 ms: 1.03x slower                                         |
| nbody                    | 92.9 ms                                                      | 95.6 ms: 1.03x slower                                        |
| create_gc_cycles         | 1.58 ms                                                      | 1.63 ms: 1.03x slower                                        |
| mdp                      | 2.77 sec                                                     | 2.86 sec: 1.03x slower                                       |
| regex_effbot             | 3.34 ms                                                      | 3.46 ms: 1.04x slower                                        |
| scimark_sor              | 110 ms                                                       | 115 ms: 1.05x slower                                         |
| richards                 | 49.7 ms                                                      | 52.2 ms: 1.05x slower                                        |
| fannkuch                 | 416 ms                                                       | 441 ms: 1.06x slower                                         |
| go                       | 158 ms                                                       | 170 ms: 1.08x slower                                         |
| Geometric mean           | (ref)                                                        | 1.00x faster                                                 |

Benchmark hidden because not significant (24): html5lib, pylint, bench_thread_pool, scimark_monte_carlo, flaskblogging, unpack_sequence, crypto_pyaes, deepcopy_reduce, sqlglot_normalize, pathlib, sqlalchemy_declarative, chaos, generators, sqlglot_transpile, coroutines, async_tree_io, async_generators, scimark_fft, async_tree_memoization, dulwich_log, raytrace, async_tree_cpu_io_mixed, genshi_text, pickle
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 60.29% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.02x