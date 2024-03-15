# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 6e55480
- commit date: 2024-01-24
- overall geometric mean: 1.01x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 286 ms: 1.01x slower                                                             |
| chameleon      | 7.26 ms                                                                | 7.33 ms: 1.01x slower                                                            |
| docutils       | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io             | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| async_tree_io_tg          | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| async_tree_none_tg        | 457 ms                                                                 | 455 ms: 1.00x faster                                                             |
| async_tree_memoization_tg | 587 ms                                                                 | 599 ms: 1.02x slower                                                             |
| Geometric mean            | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_none, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 119 ms                                                                 | 110 ms: 1.08x faster                                                             |
| float          | 92.8 ms                                                                | 87.8 ms: 1.06x faster                                                            |
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.05x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.71 ms                                                                | 3.64 ms: 1.02x faster                                                            |
| regex_compile  | 152 ms                                                                 | 149 ms: 1.02x faster                                                             |
| regex_v8       | 24.9 ms                                                                | 24.7 ms: 1.01x faster                                                            |
| regex_dna      | 219 ms                                                                 | 223 ms: 1.02x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|---------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| xml_etree_parse     | 160 ms                                                                 | 157 ms: 1.02x faster                                                             |
| xml_etree_iterparse | 111 ms                                                                 | 110 ms: 1.01x faster                                                             |
| unpickle            | 15.0 us                                                                | 14.9 us: 1.01x faster                                                            |
| unpickle_list       | 5.35 us                                                                | 5.31 us: 1.01x faster                                                            |
| json_dumps          | 10.5 ms                                                                | 10.5 ms: 1.01x faster                                                            |
| xml_etree_generate  | 89.0 ms                                                                | 88.5 ms: 1.01x faster                                                            |
| pickle              | 11.6 us                                                                | 11.5 us: 1.01x faster                                                            |
| pickle_pure_python  | 298 us                                                                 | 300 us: 1.01x slower                                                             |
| json_loads          | 28.3 us                                                                | 28.8 us: 1.02x slower                                                            |
| tomli_loads         | 2.42 sec                                                               | 2.47 sec: 1.02x slower                                                           |
| pickle_dict         | 33.8 us                                                                | 34.9 us: 1.03x slower                                                            |
| pickle_list         | 5.02 us                                                                | 5.24 us: 1.04x slower                                                            |
| Geometric mean      | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): xml_etree_process, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| python_startup_no_site | 8.73 ms                                                                | 8.84 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.1 ms                                                                | 13.3 ms: 1.06x faster                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240124-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-6e55480 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpack_sequence           | 49.3 ns                                                                | 39.0 ns: 1.26x faster                                                            |
| scimark_sparse_mat_mult   | 6.09 ms                                                                | 5.57 ms: 1.09x faster                                                            |
| scimark_fft               | 455 ms                                                                 | 419 ms: 1.08x faster                                                             |
| nbody                     | 119 ms                                                                 | 110 ms: 1.08x faster                                                             |
| deltablue                 | 4.72 ms                                                                | 4.42 ms: 1.07x faster                                                            |
| mako                      | 14.1 ms                                                                | 13.3 ms: 1.06x faster                                                            |
| spectral_norm             | 144 ms                                                                 | 136 ms: 1.06x faster                                                             |
| float                     | 92.8 ms                                                                | 87.8 ms: 1.06x faster                                                            |
| chaos                     | 74.1 ms                                                                | 70.5 ms: 1.05x faster                                                            |
| hexiom                    | 8.36 ms                                                                | 7.97 ms: 1.05x faster                                                            |
| asyncio_tcp               | 490 ms                                                                 | 469 ms: 1.04x faster                                                             |
| scimark_sor               | 130 ms                                                                 | 125 ms: 1.04x faster                                                             |
| comprehensions            | 21.3 us                                                                | 20.5 us: 1.04x faster                                                            |
| nqueens                   | 93.5 ms                                                                | 90.5 ms: 1.03x faster                                                            |
| fannkuch                  | 450 ms                                                                 | 437 ms: 1.03x faster                                                             |
| pyflate                   | 529 ms                                                                 | 516 ms: 1.02x faster                                                             |
| scimark_monte_carlo       | 80.5 ms                                                                | 78.8 ms: 1.02x faster                                                            |
| pprint_pformat            | 1.70 sec                                                               | 1.67 sec: 1.02x faster                                                           |
| sympy_str                 | 294 ms                                                                 | 288 ms: 1.02x faster                                                             |
| regex_effbot              | 3.71 ms                                                                | 3.64 ms: 1.02x faster                                                            |
| raytrace                  | 303 ms                                                                 | 297 ms: 1.02x faster                                                             |
| xml_etree_parse           | 160 ms                                                                 | 157 ms: 1.02x faster                                                             |
| regex_compile             | 152 ms                                                                 | 149 ms: 1.02x faster                                                             |
| async_generators          | 464 ms                                                                 | 456 ms: 1.02x faster                                                             |
| richards_super            | 55.4 ms                                                                | 54.5 ms: 1.02x faster                                                            |
| pprint_safe_repr          | 822 ms                                                                 | 811 ms: 1.01x faster                                                             |
| meteor_contest            | 115 ms                                                                 | 114 ms: 1.01x faster                                                             |
| xml_etree_iterparse       | 111 ms                                                                 | 110 ms: 1.01x faster                                                             |
| async_tree_io             | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| unpickle                  | 15.0 us                                                                | 14.9 us: 1.01x faster                                                            |
| asyncio_tcp_ssl           | 1.81 sec                                                               | 1.79 sec: 1.01x faster                                                           |
| async_tree_io_tg          | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| generators                | 29.9 ms                                                                | 29.6 ms: 1.01x faster                                                            |
| regex_v8                  | 24.9 ms                                                                | 24.7 ms: 1.01x faster                                                            |
| sympy_integrate           | 21.1 ms                                                                | 20.9 ms: 1.01x faster                                                            |
| create_gc_cycles          | 1.48 ms                                                                | 1.47 ms: 1.01x faster                                                            |
| richards                  | 48.6 ms                                                                | 48.2 ms: 1.01x faster                                                            |
| deepcopy_memo             | 40.9 us                                                                | 40.6 us: 1.01x faster                                                            |
| dulwich_log               | 69.3 ms                                                                | 68.8 ms: 1.01x faster                                                            |
| unpickle_list             | 5.35 us                                                                | 5.31 us: 1.01x faster                                                            |
| deepcopy_reduce           | 3.19 us                                                                | 3.17 us: 1.01x faster                                                            |
| json_dumps                | 10.5 ms                                                                | 10.5 ms: 1.01x faster                                                            |
| xml_etree_generate        | 89.0 ms                                                                | 88.5 ms: 1.01x faster                                                            |
| pickle                    | 11.6 us                                                                | 11.5 us: 1.01x faster                                                            |
| bench_thread_pool         | 846 us                                                                 | 842 us: 1.00x faster                                                             |
| go                        | 154 ms                                                                 | 153 ms: 1.00x faster                                                             |
| async_tree_none_tg        | 457 ms                                                                 | 455 ms: 1.00x faster                                                             |
| crypto_pyaes              | 82.6 ms                                                                | 82.3 ms: 1.00x faster                                                            |
| docutils                  | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| sqlglot_normalize         | 114 ms                                                                 | 114 ms: 1.00x faster                                                             |
| pidigits                  | 188 ms                                                                 | 188 ms: 1.00x slower                                                             |
| sqlglot_optimize          | 57.6 ms                                                                | 57.8 ms: 1.00x slower                                                            |
| deepcopy                  | 359 us                                                                 | 360 us: 1.00x slower                                                             |
| pickle_pure_python        | 298 us                                                                 | 300 us: 1.01x slower                                                             |
| python_startup            | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| scimark_lu                | 118 ms                                                                 | 119 ms: 1.01x slower                                                             |
| logging_format            | 6.80 us                                                                | 6.86 us: 1.01x slower                                                            |
| chameleon                 | 7.26 ms                                                                | 7.33 ms: 1.01x slower                                                            |
| 2to3                      | 282 ms                                                                 | 286 ms: 1.01x slower                                                             |
| python_startup_no_site    | 8.73 ms                                                                | 8.84 ms: 1.01x slower                                                            |
| coroutines                | 22.0 ms                                                                | 22.3 ms: 1.01x slower                                                            |
| json_loads                | 28.3 us                                                                | 28.8 us: 1.02x slower                                                            |
| tomli_loads               | 2.42 sec                                                               | 2.47 sec: 1.02x slower                                                           |
| pathlib                   | 18.5 ms                                                                | 18.9 ms: 1.02x slower                                                            |
| async_tree_memoization_tg | 587 ms                                                                 | 599 ms: 1.02x slower                                                             |
| regex_dna                 | 219 ms                                                                 | 223 ms: 1.02x slower                                                             |
| gc_traversal              | 3.71 ms                                                                | 3.82 ms: 1.03x slower                                                            |
| pickle_dict               | 33.8 us                                                                | 34.9 us: 1.03x slower                                                            |
| mdp                       | 2.67 sec                                                               | 2.79 sec: 1.04x slower                                                           |
| pickle_list               | 5.02 us                                                                | 5.24 us: 1.04x slower                                                            |
| Geometric mean            | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (23): async_tree_memoization, telco, json, sqlglot_transpile, sqlite_synth, xml_etree_process, async_tree_none, typing_runtime_protocols, sqlglot_parse, asyncio_websockets, async_tree_cpu_io_mixed, dask, bench_mp_pool, sympy_expand, coverage, logging_simple, sympy_sum, unpickle_pure_python, pycparser, async_tree_cpu_io_mixed_tg, tornado_http, mypy2, logging_silent


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x