# Results vs. base

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: 472a3d6
- commit date: 2024-02-15
- overall geometric mean: 1.01x faster
- HPT reliability: 99.86%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 276 ms                                                                 | 277 ms: 1.00x slower                                                         |
| chameleon      | 6.90 ms                                                                | 6.84 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                 |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|---------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_memoization_tg | 586 ms                                                                 | 571 ms: 1.03x faster                                                         |
| async_tree_none_tg        | 452 ms                                                                 | 444 ms: 1.02x faster                                                         |
| Geometric mean            | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (6): async_tree_memoization, async_tree_io, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 85.1 ms                                                                | 83.0 ms: 1.03x faster                                                        |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                                         |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 225 ms                                                                 | 219 ms: 1.03x faster                                                         |
| regex_v8       | 25.2 ms                                                                | 24.6 ms: 1.03x faster                                                        |
| regex_compile  | 140 ms                                                                 | 138 ms: 1.01x faster                                                         |
| regex_effbot   | 3.65 ms                                                                | 3.62 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle             | 16.0 us                                                                | 15.1 us: 1.06x faster                                                        |
| pickle               | 11.7 us                                                                | 11.3 us: 1.03x faster                                                        |
| pickle_dict          | 34.3 us                                                                | 33.4 us: 1.03x faster                                                        |
| tomli_loads          | 2.23 sec                                                               | 2.18 sec: 1.02x faster                                                       |
| pickle_list          | 4.98 us                                                                | 4.91 us: 1.01x faster                                                        |
| xml_etree_parse      | 158 ms                                                                 | 156 ms: 1.01x faster                                                         |
| xml_etree_iterparse  | 107 ms                                                                 | 106 ms: 1.01x faster                                                         |
| xml_etree_process    | 58.5 ms                                                                | 58.1 ms: 1.01x faster                                                        |
| unpickle_pure_python | 226 us                                                                 | 225 us: 1.00x faster                                                         |
| json_dumps           | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                        |
| unpickle_list        | 5.10 us                                                                | 5.16 us: 1.01x slower                                                        |
| pickle_pure_python   | 296 us                                                                 | 299 us: 1.01x slower                                                         |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (2): xml_etree_generate, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 8.82 ms                                                                | 8.84 ms: 1.00x slower                                                        |
| python_startup         | 10.2 ms                                                                | 10.2 ms: 1.00x slower                                                        |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 12.3 ms                                                                | 12.1 ms: 1.02x faster                                                        |

All benchmarks:
===============

| Benchmark                 | bm-20240215-linux-x86_64-python-32f8ab1ab65c13ed70f0-3.13.0a3+-32f8ab1 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|---------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| gc_traversal              | 3.85 ms                                                                | 3.47 ms: 1.11x faster                                                        |
| mdp                       | 2.79 sec                                                               | 2.59 sec: 1.08x faster                                                       |
| unpickle                  | 16.0 us                                                                | 15.1 us: 1.06x faster                                                        |
| spectral_norm             | 133 ms                                                                 | 126 ms: 1.05x faster                                                         |
| pycparser                 | 1.22 sec                                                               | 1.18 sec: 1.03x faster                                                       |
| pickle                    | 11.7 us                                                                | 11.3 us: 1.03x faster                                                        |
| regex_dna                 | 225 ms                                                                 | 219 ms: 1.03x faster                                                         |
| pyflate                   | 510 ms                                                                 | 497 ms: 1.03x faster                                                         |
| async_tree_memoization_tg | 586 ms                                                                 | 571 ms: 1.03x faster                                                         |
| pickle_dict               | 34.3 us                                                                | 33.4 us: 1.03x faster                                                        |
| regex_v8                  | 25.2 ms                                                                | 24.6 ms: 1.03x faster                                                        |
| fannkuch                  | 428 ms                                                                 | 417 ms: 1.03x faster                                                         |
| float                     | 85.1 ms                                                                | 83.0 ms: 1.03x faster                                                        |
| tomli_loads               | 2.23 sec                                                               | 2.18 sec: 1.02x faster                                                       |
| hexiom                    | 7.77 ms                                                                | 7.61 ms: 1.02x faster                                                        |
| async_tree_none_tg        | 452 ms                                                                 | 444 ms: 1.02x faster                                                         |
| mako                      | 12.3 ms                                                                | 12.1 ms: 1.02x faster                                                        |
| json                      | 5.15 ms                                                                | 5.06 ms: 1.02x faster                                                        |
| meteor_contest            | 111 ms                                                                 | 109 ms: 1.02x faster                                                         |
| logging_simple            | 5.80 us                                                                | 5.71 us: 1.02x faster                                                        |
| coroutines                | 23.1 ms                                                                | 22.8 ms: 1.01x faster                                                        |
| unpack_sequence           | 52.7 ns                                                                | 52.0 ns: 1.01x faster                                                        |
| pickle_list               | 4.98 us                                                                | 4.91 us: 1.01x faster                                                        |
| comprehensions            | 18.3 us                                                                | 18.0 us: 1.01x faster                                                        |
| typing_runtime_protocols  | 112 us                                                                 | 110 us: 1.01x faster                                                         |
| coverage                  | 96.6 ms                                                                | 95.4 ms: 1.01x faster                                                        |
| deltablue                 | 3.35 ms                                                                | 3.31 ms: 1.01x faster                                                        |
| deepcopy_reduce           | 3.10 us                                                                | 3.07 us: 1.01x faster                                                        |
| regex_compile             | 140 ms                                                                 | 138 ms: 1.01x faster                                                         |
| xml_etree_parse           | 158 ms                                                                 | 156 ms: 1.01x faster                                                         |
| xml_etree_iterparse       | 107 ms                                                                 | 106 ms: 1.01x faster                                                         |
| chameleon                 | 6.90 ms                                                                | 6.84 ms: 1.01x faster                                                        |
| sqlglot_parse             | 1.30 ms                                                                | 1.29 ms: 1.01x faster                                                        |
| regex_effbot              | 3.65 ms                                                                | 3.62 ms: 1.01x faster                                                        |
| sympy_str                 | 282 ms                                                                 | 281 ms: 1.01x faster                                                         |
| xml_etree_process         | 58.5 ms                                                                | 58.1 ms: 1.01x faster                                                        |
| create_gc_cycles          | 1.47 ms                                                                | 1.46 ms: 1.01x faster                                                        |
| dulwich_log               | 68.1 ms                                                                | 67.7 ms: 1.01x faster                                                        |
| go                        | 148 ms                                                                 | 148 ms: 1.00x faster                                                         |
| unpickle_pure_python      | 226 us                                                                 | 225 us: 1.00x faster                                                         |
| asyncio_tcp_ssl           | 1.80 sec                                                               | 1.79 sec: 1.00x faster                                                       |
| asyncio_tcp               | 489 ms                                                                 | 487 ms: 1.00x faster                                                         |
| pidigits                  | 188 ms                                                                 | 187 ms: 1.00x faster                                                         |
| python_startup_no_site    | 8.82 ms                                                                | 8.84 ms: 1.00x slower                                                        |
| python_startup            | 10.2 ms                                                                | 10.2 ms: 1.00x slower                                                        |
| 2to3                      | 276 ms                                                                 | 277 ms: 1.00x slower                                                         |
| raytrace                  | 279 ms                                                                 | 280 ms: 1.00x slower                                                         |
| bench_thread_pool         | 834 us                                                                 | 840 us: 1.01x slower                                                         |
| deepcopy                  | 346 us                                                                 | 349 us: 1.01x slower                                                         |
| richards                  | 44.9 ms                                                                | 45.2 ms: 1.01x slower                                                        |
| json_dumps                | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                        |
| logging_format            | 6.34 us                                                                | 6.39 us: 1.01x slower                                                        |
| unpickle_list             | 5.10 us                                                                | 5.16 us: 1.01x slower                                                        |
| pprint_pformat            | 1.61 sec                                                               | 1.63 sec: 1.01x slower                                                       |
| richards_super            | 50.7 ms                                                                | 51.3 ms: 1.01x slower                                                        |
| pickle_pure_python        | 296 us                                                                 | 299 us: 1.01x slower                                                         |
| logging_silent            | 100 ns                                                                 | 101 ns: 1.01x slower                                                         |
| sqlglot_normalize         | 107 ms                                                                 | 109 ms: 1.01x slower                                                         |
| generators                | 29.5 ms                                                                | 29.9 ms: 1.01x slower                                                        |
| sqlite_synth              | 2.78 us                                                                | 2.83 us: 1.02x slower                                                        |
| scimark_lu                | 112 ms                                                                 | 114 ms: 1.02x slower                                                         |
| Geometric mean            | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (32): scimark_sparse_mat_mult, async_tree_memoization, scimark_monte_carlo, async_tree_io, async_tree_cpu_io_mixed_tg, sqlglot_transpile, mypy2, sympy_expand, sqlglot_optimize, async_tree_io_tg, xml_etree_generate, async_tree_cpu_io_mixed, asyncio_websockets, bench_mp_pool, deepcopy_memo, async_tree_none, sympy_sum, crypto_pyaes, pathlib, json_loads, sympy_integrate, scimark_sor, docutils, pprint_safe_repr, async_generators, dask, scimark_fft, tornado_http, nqueens, nbody, chaos, telco


# HPT report

- Reliability score: 99.86% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x