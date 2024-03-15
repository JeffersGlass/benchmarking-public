# Results vs. base

- fork: mdboom
- ref: faster_negate
- machine: linux-x86_64
- commit hash: 34fc24a
- commit date: 2024-01-04
- overall geometric mean: 1.00x slower
- HPT reliability: 96.40%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 265 ms: 1.01x slower                                            |
| chameleon      | 6.97 ms                                                                | 6.87 ms: 1.01x faster                                           |
| docutils       | 2.61 sec                                                               | 2.59 sec: 1.01x faster                                          |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                    |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io    | 1.18 sec                                                               | 1.17 sec: 1.01x faster                                          |
| async_tree_io_tg | 1.20 sec                                                               | 1.19 sec: 1.00x faster                                          |
| Geometric mean   | (ref)                                                                  | 1.00x faster                                                    |

Benchmark hidden because not significant (6): async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 195 ms                                                                 | 187 ms: 1.04x faster                                            |
| float          | 79.4 ms                                                                | 80.3 ms: 1.01x slower                                           |
| nbody          | 88.9 ms                                                                | 90.1 ms: 1.01x slower                                           |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_effbot   | 3.77 ms                                                                | 3.64 ms: 1.04x faster                                           |
| regex_v8       | 25.3 ms                                                                | 25.0 ms: 1.01x faster                                           |
| regex_dna      | 224 ms                                                                 | 225 ms: 1.01x slower                                            |
| regex_compile  | 129 ms                                                                 | 130 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|----------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle               | 11.5 us                                                                | 11.4 us: 1.01x faster                                           |
| unpickle_list        | 5.13 us                                                                | 5.10 us: 1.00x faster                                           |
| json_dumps           | 10.5 ms                                                                | 10.5 ms: 1.01x slower                                           |
| json_loads           | 28.1 us                                                                | 28.3 us: 1.01x slower                                           |
| xml_etree_process    | 58.5 ms                                                                | 58.9 ms: 1.01x slower                                           |
| xml_etree_iterparse  | 104 ms                                                                 | 105 ms: 1.01x slower                                            |
| xml_etree_generate   | 84.9 ms                                                                | 85.8 ms: 1.01x slower                                           |
| pickle_pure_python   | 300 us                                                                 | 305 us: 1.02x slower                                            |
| pickle_dict          | 33.4 us                                                                | 34.2 us: 1.02x slower                                           |
| unpickle_pure_python | 213 us                                                                 | 219 us: 1.03x slower                                            |
| xml_etree_parse      | 156 ms                                                                 | 160 ms: 1.03x slower                                            |
| tomli_loads          | 2.11 sec                                                               | 2.18 sec: 1.03x slower                                          |
| unpickle             | 15.0 us                                                                | 15.7 us: 1.05x slower                                           |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                    |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                           |
| python_startup_no_site | 8.70 ms                                                                | 8.73 ms: 1.00x slower                                           |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|-----------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako      | 11.1 ms                                                                | 11.2 ms: 1.01x slower                                           |

All benchmarks:
===============

| Benchmark                | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-mdboom-faster_negate-3.13.0a2+-34fc24a |
|--------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits                 | 195 ms                                                                 | 187 ms: 1.04x faster                                            |
| regex_effbot             | 3.77 ms                                                                | 3.64 ms: 1.04x faster                                           |
| pycparser                | 1.20 sec                                                               | 1.17 sec: 1.03x faster                                          |
| typing_runtime_protocols | 112 us                                                                 | 109 us: 1.03x faster                                            |
| pyflate                  | 464 ms                                                                 | 456 ms: 1.02x faster                                            |
| pathlib                  | 18.5 ms                                                                | 18.2 ms: 1.02x faster                                           |
| chameleon                | 6.97 ms                                                                | 6.87 ms: 1.01x faster                                           |
| pickle                   | 11.5 us                                                                | 11.4 us: 1.01x faster                                           |
| regex_v8                 | 25.3 ms                                                                | 25.0 ms: 1.01x faster                                           |
| docutils                 | 2.61 sec                                                               | 2.59 sec: 1.01x faster                                          |
| async_tree_io            | 1.18 sec                                                               | 1.17 sec: 1.01x faster                                          |
| gc_traversal             | 3.72 ms                                                                | 3.70 ms: 1.01x faster                                           |
| sympy_sum                | 148 ms                                                                 | 148 ms: 1.00x faster                                            |
| dulwich_log              | 65.4 ms                                                                | 65.1 ms: 1.00x faster                                           |
| meteor_contest           | 107 ms                                                                 | 107 ms: 1.00x faster                                            |
| unpickle_list            | 5.13 us                                                                | 5.10 us: 1.00x faster                                           |
| async_tree_io_tg         | 1.20 sec                                                               | 1.19 sec: 1.00x faster                                          |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                           |
| bench_thread_pool        | 828 us                                                                 | 830 us: 1.00x slower                                            |
| raytrace                 | 260 ms                                                                 | 261 ms: 1.00x slower                                            |
| deepcopy                 | 345 us                                                                 | 346 us: 1.00x slower                                            |
| python_startup_no_site   | 8.70 ms                                                                | 8.73 ms: 1.00x slower                                           |
| pprint_pformat           | 1.49 sec                                                               | 1.50 sec: 1.00x slower                                          |
| sympy_integrate          | 19.5 ms                                                                | 19.5 ms: 1.00x slower                                           |
| 2to3                     | 263 ms                                                                 | 265 ms: 1.01x slower                                            |
| deltablue                | 3.23 ms                                                                | 3.25 ms: 1.01x slower                                           |
| create_gc_cycles         | 1.47 ms                                                                | 1.48 ms: 1.01x slower                                           |
| json_dumps               | 10.5 ms                                                                | 10.5 ms: 1.01x slower                                           |
| regex_dna                | 224 ms                                                                 | 225 ms: 1.01x slower                                            |
| crypto_pyaes             | 71.3 ms                                                                | 71.8 ms: 1.01x slower                                           |
| sqlglot_parse            | 1.24 ms                                                                | 1.24 ms: 1.01x slower                                           |
| json_loads               | 28.1 us                                                                | 28.3 us: 1.01x slower                                           |
| xml_etree_process        | 58.5 ms                                                                | 58.9 ms: 1.01x slower                                           |
| fannkuch                 | 400 ms                                                                 | 403 ms: 1.01x slower                                            |
| xml_etree_iterparse      | 104 ms                                                                 | 105 ms: 1.01x slower                                            |
| deepcopy_reduce          | 3.05 us                                                                | 3.08 us: 1.01x slower                                           |
| xml_etree_generate       | 84.9 ms                                                                | 85.8 ms: 1.01x slower                                           |
| regex_compile            | 129 ms                                                                 | 130 ms: 1.01x slower                                            |
| mako                     | 11.1 ms                                                                | 11.2 ms: 1.01x slower                                           |
| json                     | 5.21 ms                                                                | 5.27 ms: 1.01x slower                                           |
| float                    | 79.4 ms                                                                | 80.3 ms: 1.01x slower                                           |
| sqlite_synth             | 2.82 us                                                                | 2.86 us: 1.01x slower                                           |
| telco                    | 8.32 ms                                                                | 8.42 ms: 1.01x slower                                           |
| scimark_sor              | 129 ms                                                                 | 130 ms: 1.01x slower                                            |
| pprint_safe_repr         | 728 ms                                                                 | 737 ms: 1.01x slower                                            |
| scimark_sparse_mat_mult  | 4.93 ms                                                                | 5.00 ms: 1.01x slower                                           |
| nbody                    | 88.9 ms                                                                | 90.1 ms: 1.01x slower                                           |
| spectral_norm            | 114 ms                                                                 | 115 ms: 1.01x slower                                            |
| scimark_lu               | 111 ms                                                                 | 112 ms: 1.01x slower                                            |
| hexiom                   | 6.20 ms                                                                | 6.29 ms: 1.01x slower                                           |
| async_generators         | 438 ms                                                                 | 445 ms: 1.02x slower                                            |
| chaos                    | 59.2 ms                                                                | 60.1 ms: 1.02x slower                                           |
| go                       | 138 ms                                                                 | 141 ms: 1.02x slower                                            |
| pickle_pure_python       | 300 us                                                                 | 305 us: 1.02x slower                                            |
| mdp                      | 2.53 sec                                                               | 2.57 sec: 1.02x slower                                          |
| logging_silent           | 101 ns                                                                 | 103 ns: 1.02x slower                                            |
| deepcopy_memo            | 37.9 us                                                                | 38.6 us: 1.02x slower                                           |
| coroutines               | 21.6 ms                                                                | 22.1 ms: 1.02x slower                                           |
| pickle_dict              | 33.4 us                                                                | 34.2 us: 1.02x slower                                           |
| comprehensions           | 16.0 us                                                                | 16.4 us: 1.03x slower                                           |
| unpickle_pure_python     | 213 us                                                                 | 219 us: 1.03x slower                                            |
| xml_etree_parse          | 156 ms                                                                 | 160 ms: 1.03x slower                                            |
| tomli_loads              | 2.11 sec                                                               | 2.18 sec: 1.03x slower                                          |
| scimark_fft              | 352 ms                                                                 | 364 ms: 1.03x slower                                            |
| unpickle                 | 15.0 us                                                                | 15.7 us: 1.05x slower                                           |
| unpack_sequence          | 40.5 ns                                                                | 44.1 ns: 1.09x slower                                           |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                    |

Benchmark hidden because not significant (27): sympy_str, logging_simple, tornado_http, pickle_list, generators, richards, sqlglot_transpile, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, richards_super, mypy2, async_tree_none, nqueens, asyncio_websockets, bench_mp_pool, asyncio_tcp, async_tree_memoization_tg, asyncio_tcp_ssl, async_tree_none_tg, logging_format, sqlglot_normalize, sympy_expand, sqlglot_optimize, dask, scimark_monte_carlo, coverage


# HPT report

- Reliability score: 96.40% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x