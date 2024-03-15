# Results vs. base

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.00x faster
- HPT reliability: 77.19%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 301 ms                                                                       | 300 ms: 1.00x faster                                            |
| chameleon      | 7.18 ms                                                                      | 7.22 ms: 1.01x slower                                           |
| docutils       | 2.88 sec                                                                     | 2.87 sec: 1.00x faster                                          |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                    |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------|:----------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io_tg | 1.08 sec                                                                     | 1.08 sec: 1.00x faster                                          |
| Geometric mean   | (ref)                                                                        | 1.00x faster                                                    |

Benchmark hidden because not significant (7): async_tree_none_tg, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 81.7 ms                                                                      | 81.2 ms: 1.01x faster                                           |
| nbody          | 106 ms                                                                       | 107 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_v8       | 26.1 ms                                                                      | 25.2 ms: 1.04x faster                                           |
| regex_dna      | 249 ms                                                                       | 244 ms: 1.02x faster                                            |
| regex_compile  | 146 ms                                                                       | 145 ms: 1.01x faster                                            |
| regex_effbot   | 3.49 ms                                                                      | 3.57 ms: 1.02x slower                                           |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:----------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpickle             | 15.3 us                                                                      | 15.0 us: 1.02x faster                                           |
| pickle_list          | 4.47 us                                                                      | 4.38 us: 1.02x faster                                           |
| xml_etree_process    | 58.5 ms                                                                      | 58.2 ms: 1.01x faster                                           |
| json_loads           | 25.2 us                                                                      | 25.1 us: 1.01x faster                                           |
| unpickle_pure_python | 228 us                                                                       | 227 us: 1.00x faster                                            |
| json_dumps           | 10.5 ms                                                                      | 10.6 ms: 1.01x slower                                           |
| xml_etree_iterparse  | 104 ms                                                                       | 106 ms: 1.01x slower                                            |
| xml_etree_parse      | 147 ms                                                                       | 150 ms: 1.02x slower                                            |
| pickle               | 10.3 us                                                                      | 10.6 us: 1.04x slower                                           |
| pickle_dict          | 30.8 us                                                                      | 32.7 us: 1.06x slower                                           |
| Geometric mean       | (ref)                                                                        | 1.00x slower                                                    |

Benchmark hidden because not significant (4): unpickle_list, tomli_loads, xml_etree_generate, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:----------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 11.1 ms                                                                      | 11.1 ms: 1.00x faster                                           |
| python_startup         | 12.7 ms                                                                      | 12.6 ms: 1.00x faster                                           |
| Geometric mean         | (ref)                                                                        | 1.00x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:----------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 11.9 ms                                                                      | 11.7 ms: 1.02x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-pythonperf2-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:----------------------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpack_sequence          | 44.8 ns                                                                      | 41.2 ns: 1.09x faster                                           |
| gc_traversal             | 3.71 ms                                                                      | 3.43 ms: 1.08x faster                                           |
| async_generators         | 382 ms                                                                       | 363 ms: 1.05x faster                                            |
| regex_v8                 | 26.1 ms                                                                      | 25.2 ms: 1.04x faster                                           |
| logging_format           | 7.43 us                                                                      | 7.18 us: 1.04x faster                                           |
| coverage                 | 79.5 ms                                                                      | 77.6 ms: 1.02x faster                                           |
| unpickle                 | 15.3 us                                                                      | 15.0 us: 1.02x faster                                           |
| regex_dna                | 249 ms                                                                       | 244 ms: 1.02x faster                                            |
| pickle_list              | 4.47 us                                                                      | 4.38 us: 1.02x faster                                           |
| meteor_contest           | 133 ms                                                                       | 130 ms: 1.02x faster                                            |
| create_gc_cycles         | 1.54 ms                                                                      | 1.52 ms: 1.02x faster                                           |
| logging_simple           | 6.66 us                                                                      | 6.55 us: 1.02x faster                                           |
| sqlglot_optimize         | 61.5 ms                                                                      | 60.6 ms: 1.02x faster                                           |
| mako                     | 11.9 ms                                                                      | 11.7 ms: 1.02x faster                                           |
| sqlite_synth             | 2.78 us                                                                      | 2.74 us: 1.01x faster                                           |
| scimark_monte_carlo      | 77.6 ms                                                                      | 76.6 ms: 1.01x faster                                           |
| deepcopy_memo            | 37.0 us                                                                      | 36.6 us: 1.01x faster                                           |
| regex_compile            | 146 ms                                                                       | 145 ms: 1.01x faster                                            |
| nqueens                  | 96.7 ms                                                                      | 95.7 ms: 1.01x faster                                           |
| sqlglot_normalize        | 119 ms                                                                       | 118 ms: 1.01x faster                                            |
| typing_runtime_protocols | 120 us                                                                       | 119 us: 1.01x faster                                            |
| float                    | 81.7 ms                                                                      | 81.2 ms: 1.01x faster                                           |
| richards                 | 50.6 ms                                                                      | 50.3 ms: 1.01x faster                                           |
| asyncio_tcp              | 376 ms                                                                       | 373 ms: 1.01x faster                                            |
| xml_etree_process        | 58.5 ms                                                                      | 58.2 ms: 1.01x faster                                           |
| json_loads               | 25.2 us                                                                      | 25.1 us: 1.01x faster                                           |
| python_startup_no_site   | 11.1 ms                                                                      | 11.1 ms: 1.00x faster                                           |
| unpickle_pure_python     | 228 us                                                                       | 227 us: 1.00x faster                                            |
| 2to3                     | 301 ms                                                                       | 300 ms: 1.00x faster                                            |
| docutils                 | 2.88 sec                                                                     | 2.87 sec: 1.00x faster                                          |
| python_startup           | 12.7 ms                                                                      | 12.6 ms: 1.00x faster                                           |
| async_tree_io_tg         | 1.08 sec                                                                     | 1.08 sec: 1.00x faster                                          |
| sympy_str                | 298 ms                                                                       | 299 ms: 1.00x slower                                            |
| dulwich_log              | 69.0 ms                                                                      | 69.4 ms: 1.00x slower                                           |
| sympy_sum                | 158 ms                                                                       | 158 ms: 1.00x slower                                            |
| chameleon                | 7.18 ms                                                                      | 7.22 ms: 1.01x slower                                           |
| pathlib                  | 18.8 ms                                                                      | 18.9 ms: 1.01x slower                                           |
| hexiom                   | 7.60 ms                                                                      | 7.66 ms: 1.01x slower                                           |
| json_dumps               | 10.5 ms                                                                      | 10.6 ms: 1.01x slower                                           |
| nbody                    | 106 ms                                                                       | 107 ms: 1.01x slower                                            |
| deepcopy                 | 367 us                                                                       | 370 us: 1.01x slower                                            |
| mdp                      | 2.54 sec                                                                     | 2.56 sec: 1.01x slower                                          |
| scimark_fft              | 345 ms                                                                       | 348 ms: 1.01x slower                                            |
| asyncio_websockets       | 386 ms                                                                       | 390 ms: 1.01x slower                                            |
| comprehensions           | 19.2 us                                                                      | 19.4 us: 1.01x slower                                           |
| coroutines               | 22.3 ms                                                                      | 22.5 ms: 1.01x slower                                           |
| dask                     | 404 ms                                                                       | 409 ms: 1.01x slower                                            |
| scimark_sparse_mat_mult  | 4.95 ms                                                                      | 5.01 ms: 1.01x slower                                           |
| deepcopy_reduce          | 3.31 us                                                                      | 3.36 us: 1.01x slower                                           |
| xml_etree_iterparse      | 104 ms                                                                       | 106 ms: 1.01x slower                                            |
| pyflate                  | 538 ms                                                                       | 546 ms: 1.01x slower                                            |
| xml_etree_parse          | 147 ms                                                                       | 150 ms: 1.02x slower                                            |
| spectral_norm            | 111 ms                                                                       | 113 ms: 1.02x slower                                            |
| regex_effbot             | 3.49 ms                                                                      | 3.57 ms: 1.02x slower                                           |
| deltablue                | 3.69 ms                                                                      | 3.78 ms: 1.02x slower                                           |
| pickle                   | 10.3 us                                                                      | 10.6 us: 1.04x slower                                           |
| pickle_dict              | 30.8 us                                                                      | 32.7 us: 1.06x slower                                           |
| Geometric mean           | (ref)                                                                        | 1.00x faster                                                    |

Benchmark hidden because not significant (36): crypto_pyaes, unpickle_list, pprint_safe_repr, telco, async_tree_none_tg, pycparser, async_tree_cpu_io_mixed_tg, pprint_pformat, tomli_loads, json, go, async_tree_memoization_tg, sqlglot_transpile, async_tree_cpu_io_mixed, sympy_integrate, generators, scimark_lu, fannkuch, asyncio_tcp_ssl, async_tree_io, pidigits, sympy_expand, richards_super, async_tree_memoization, xml_etree_generate, mypy2, scimark_sor, pickle_pure_python, async_tree_none, sqlglot_parse, bench_mp_pool, logging_silent, chaos, raytrace, tornado_http, bench_thread_pool


# HPT report

- Reliability score: 77.19% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x