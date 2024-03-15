# Results vs. base

- fork: faster-cpython
- ref: guarantee_forward_pr
- machine: linux-x86_64
- commit hash: 1501bca
- commit date: 2024-01-08
- overall geometric mean: 1.00x slower
- HPT reliability: 98.85%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2+-b3dba18 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 262 ms                                                                 | 263 ms: 1.01x slower                                                             |
| tornado_http   | 94.5 ms                                                                | 93.8 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (2): chameleon, docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2+-b3dba18 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io      | 1.17 sec                                                               | 1.17 sec: 1.00x faster                                                           |
| async_tree_none_tg | 437 ms                                                                 | 440 ms: 1.01x slower                                                             |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (6): async_tree_io_tg, async_tree_memoization, async_tree_none, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2+-b3dba18 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 80.9 ms                                                                | 80.1 ms: 1.01x faster                                                            |
| nbody          | 87.0 ms                                                                | 88.8 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2+-b3dba18 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 224 ms                                                                 | 219 ms: 1.02x faster                                                             |
| regex_effbot   | 3.70 ms                                                                | 3.65 ms: 1.02x faster                                                            |
| regex_v8       | 25.8 ms                                                                | 26.0 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2+-b3dba18 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_list          | 4.99 us                                                                | 4.89 us: 1.02x faster                                                            |
| pickle_dict          | 35.7 us                                                                | 35.1 us: 1.02x faster                                                            |
| pickle               | 11.5 us                                                                | 11.4 us: 1.01x faster                                                            |
| xml_etree_generate   | 86.4 ms                                                                | 86.0 ms: 1.00x faster                                                            |
| unpickle_pure_python | 212 us                                                                 | 214 us: 1.01x slower                                                             |
| xml_etree_process    | 59.0 ms                                                                | 59.4 ms: 1.01x slower                                                            |
| json_loads           | 28.4 us                                                                | 28.7 us: 1.01x slower                                                            |
| pickle_pure_python   | 296 us                                                                 | 299 us: 1.01x slower                                                             |
| unpickle_list        | 5.03 us                                                                | 5.11 us: 1.01x slower                                                            |
| json_dumps           | 10.6 ms                                                                | 10.7 ms: 1.01x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (4): unpickle, xml_etree_parse, tomli_loads, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2+-b3dba18 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.0 ms                                                                | 10.1 ms: 1.01x slower                                                            |
| python_startup_no_site | 8.67 ms                                                                | 8.73 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2+-b3dba18 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.1 ms                                                                | 11.1 ms: 1.00x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240108-linux-x86_64-python-b3dba18eab96dc956530-3.13.0a2+-b3dba18 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpack_sequence          | 50.9 ns                                                                | 45.2 ns: 1.13x faster                                                            |
| typing_runtime_protocols | 113 us                                                                 | 110 us: 1.03x faster                                                             |
| regex_dna                | 224 ms                                                                 | 219 ms: 1.02x faster                                                             |
| pickle_list              | 4.99 us                                                                | 4.89 us: 1.02x faster                                                            |
| pickle_dict              | 35.7 us                                                                | 35.1 us: 1.02x faster                                                            |
| coverage                 | 96.3 ms                                                                | 94.7 ms: 1.02x faster                                                            |
| comprehensions           | 16.4 us                                                                | 16.1 us: 1.02x faster                                                            |
| telco                    | 8.54 ms                                                                | 8.41 ms: 1.02x faster                                                            |
| regex_effbot             | 3.70 ms                                                                | 3.65 ms: 1.02x faster                                                            |
| logging_simple           | 5.64 us                                                                | 5.57 us: 1.01x faster                                                            |
| float                    | 80.9 ms                                                                | 80.1 ms: 1.01x faster                                                            |
| scimark_monte_carlo      | 68.7 ms                                                                | 68.0 ms: 1.01x faster                                                            |
| json                     | 5.31 ms                                                                | 5.26 ms: 1.01x faster                                                            |
| async_generators         | 442 ms                                                                 | 437 ms: 1.01x faster                                                             |
| sympy_sum                | 148 ms                                                                 | 147 ms: 1.01x faster                                                             |
| tornado_http             | 94.5 ms                                                                | 93.8 ms: 1.01x faster                                                            |
| pickle                   | 11.5 us                                                                | 11.4 us: 1.01x faster                                                            |
| logging_format           | 6.16 us                                                                | 6.13 us: 1.01x faster                                                            |
| scimark_sor              | 128 ms                                                                 | 127 ms: 1.01x faster                                                             |
| xml_etree_generate       | 86.4 ms                                                                | 86.0 ms: 1.00x faster                                                            |
| mako                     | 11.1 ms                                                                | 11.1 ms: 1.00x faster                                                            |
| sqlglot_normalize        | 106 ms                                                                 | 106 ms: 1.00x faster                                                             |
| async_tree_io            | 1.17 sec                                                               | 1.17 sec: 1.00x faster                                                           |
| meteor_contest           | 108 ms                                                                 | 108 ms: 1.00x faster                                                             |
| sympy_integrate          | 19.4 ms                                                                | 19.3 ms: 1.00x faster                                                            |
| asyncio_tcp_ssl          | 1.78 sec                                                               | 1.78 sec: 1.00x faster                                                           |
| bench_thread_pool        | 823 us                                                                 | 826 us: 1.00x slower                                                             |
| deepcopy                 | 345 us                                                                 | 346 us: 1.00x slower                                                             |
| asyncio_tcp              | 480 ms                                                                 | 481 ms: 1.00x slower                                                             |
| sqlglot_optimize         | 53.2 ms                                                                | 53.4 ms: 1.00x slower                                                            |
| crypto_pyaes             | 70.3 ms                                                                | 70.6 ms: 1.00x slower                                                            |
| pprint_safe_repr         | 736 ms                                                                 | 739 ms: 1.00x slower                                                             |
| regex_v8                 | 25.8 ms                                                                | 26.0 ms: 1.01x slower                                                            |
| 2to3                     | 262 ms                                                                 | 263 ms: 1.01x slower                                                             |
| unpickle_pure_python     | 212 us                                                                 | 214 us: 1.01x slower                                                             |
| xml_etree_process        | 59.0 ms                                                                | 59.4 ms: 1.01x slower                                                            |
| python_startup           | 10.0 ms                                                                | 10.1 ms: 1.01x slower                                                            |
| python_startup_no_site   | 8.67 ms                                                                | 8.73 ms: 1.01x slower                                                            |
| async_tree_none_tg       | 437 ms                                                                 | 440 ms: 1.01x slower                                                             |
| scimark_sparse_mat_mult  | 4.96 ms                                                                | 5.00 ms: 1.01x slower                                                            |
| chaos                    | 58.2 ms                                                                | 58.7 ms: 1.01x slower                                                            |
| json_loads               | 28.4 us                                                                | 28.7 us: 1.01x slower                                                            |
| pickle_pure_python       | 296 us                                                                 | 299 us: 1.01x slower                                                             |
| pathlib                  | 18.2 ms                                                                | 18.4 ms: 1.01x slower                                                            |
| fannkuch                 | 390 ms                                                                 | 394 ms: 1.01x slower                                                             |
| richards                 | 47.0 ms                                                                | 47.6 ms: 1.01x slower                                                            |
| logging_silent           | 102 ns                                                                 | 104 ns: 1.01x slower                                                             |
| unpickle_list            | 5.03 us                                                                | 5.11 us: 1.01x slower                                                            |
| json_dumps               | 10.6 ms                                                                | 10.7 ms: 1.01x slower                                                            |
| hexiom                   | 6.00 ms                                                                | 6.09 ms: 1.01x slower                                                            |
| richards_super           | 53.7 ms                                                                | 54.5 ms: 1.02x slower                                                            |
| spectral_norm            | 111 ms                                                                 | 112 ms: 1.02x slower                                                             |
| coroutines               | 21.6 ms                                                                | 22.0 ms: 1.02x slower                                                            |
| deepcopy_memo            | 37.7 us                                                                | 38.4 us: 1.02x slower                                                            |
| pyflate                  | 444 ms                                                                 | 452 ms: 1.02x slower                                                             |
| nbody                    | 87.0 ms                                                                | 88.8 ms: 1.02x slower                                                            |
| mdp                      | 2.55 sec                                                               | 2.60 sec: 1.02x slower                                                           |
| create_gc_cycles         | 1.46 ms                                                                | 1.49 ms: 1.02x slower                                                            |
| deepcopy_reduce          | 3.06 us                                                                | 3.13 us: 1.02x slower                                                            |
| pycparser                | 1.15 sec                                                               | 1.20 sec: 1.04x slower                                                           |
| gc_traversal             | 3.60 ms                                                                | 3.81 ms: 1.06x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (32): unpickle, xml_etree_parse, sympy_str, generators, async_tree_io_tg, scimark_fft, chameleon, scimark_lu, dulwich_log, sqlglot_transpile, pidigits, async_tree_memoization, bench_mp_pool, asyncio_websockets, regex_compile, go, pprint_pformat, mypy2, docutils, raytrace, tomli_loads, nqueens, sqlglot_parse, async_tree_none, sympy_expand, xml_etree_iterparse, deltablue, dask, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, sqlite_synth


# HPT report

- Reliability score: 98.85% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x