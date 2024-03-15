# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.00x slower
- HPT reliability: 98.64%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 284 ms: 1.00x slower                                                             |
| chameleon      | 7.26 ms                                                                | 7.49 ms: 1.03x slower                                                            |
| docutils       | 2.71 sec                                                               | 2.73 sec: 1.01x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg         | 457 ms                                                                 | 461 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 731 ms                                                                 | 740 ms: 1.01x slower                                                             |
| async_tree_memoization_tg  | 587 ms                                                                 | 611 ms: 1.04x slower                                                             |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (5): async_tree_io, async_tree_io_tg, async_tree_memoization, async_tree_none, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 119 ms                                                                 | 117 ms: 1.02x faster                                                             |
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x slower                                                             |
| float          | 92.8 ms                                                                | 93.3 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.71 ms                                                                | 3.58 ms: 1.04x faster                                                            |
| regex_v8       | 24.9 ms                                                                | 25.1 ms: 1.01x slower                                                            |
| regex_dna      | 219 ms                                                                 | 223 ms: 1.02x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 5.35 us                                                                | 5.05 us: 1.06x faster                                                            |
| tomli_loads          | 2.42 sec                                                               | 2.41 sec: 1.00x faster                                                           |
| pickle_dict          | 33.8 us                                                                | 33.9 us: 1.00x slower                                                            |
| pickle_pure_python   | 298 us                                                                 | 300 us: 1.01x slower                                                             |
| unpickle_pure_python | 234 us                                                                 | 236 us: 1.01x slower                                                             |
| xml_etree_generate   | 89.0 ms                                                                | 89.9 ms: 1.01x slower                                                            |
| xml_etree_process    | 60.9 ms                                                                | 61.6 ms: 1.01x slower                                                            |
| pickle               | 11.6 us                                                                | 11.8 us: 1.02x slower                                                            |
| unpickle             | 15.0 us                                                                | 15.4 us: 1.03x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (5): xml_etree_parse, pickle_list, json_loads, json_dumps, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                                            |
| python_startup_no_site | 8.73 ms                                                                | 8.78 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.1 ms                                                                | 14.1 ms: 1.00x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| scimark_fft                | 455 ms                                                                 | 426 ms: 1.07x faster                                                             |
| unpickle_list              | 5.35 us                                                                | 5.05 us: 1.06x faster                                                            |
| scimark_sor                | 130 ms                                                                 | 125 ms: 1.04x faster                                                             |
| regex_effbot               | 3.71 ms                                                                | 3.58 ms: 1.04x faster                                                            |
| pycparser                  | 1.25 sec                                                               | 1.21 sec: 1.03x faster                                                           |
| spectral_norm              | 144 ms                                                                 | 140 ms: 1.03x faster                                                             |
| scimark_sparse_mat_mult    | 6.09 ms                                                                | 5.97 ms: 1.02x faster                                                            |
| pyflate                    | 529 ms                                                                 | 519 ms: 1.02x faster                                                             |
| deepcopy_reduce            | 3.19 us                                                                | 3.14 us: 1.02x faster                                                            |
| nbody                      | 119 ms                                                                 | 117 ms: 1.02x faster                                                             |
| mdp                        | 2.67 sec                                                               | 2.63 sec: 1.02x faster                                                           |
| json                       | 5.23 ms                                                                | 5.15 ms: 1.02x faster                                                            |
| fannkuch                   | 450 ms                                                                 | 444 ms: 1.01x faster                                                             |
| chaos                      | 74.1 ms                                                                | 73.4 ms: 1.01x faster                                                            |
| raytrace                   | 303 ms                                                                 | 300 ms: 1.01x faster                                                             |
| dulwich_log                | 69.3 ms                                                                | 68.8 ms: 1.01x faster                                                            |
| deepcopy                   | 359 us                                                                 | 357 us: 1.01x faster                                                             |
| scimark_monte_carlo        | 80.5 ms                                                                | 80.1 ms: 1.01x faster                                                            |
| deltablue                  | 4.72 ms                                                                | 4.70 ms: 1.00x faster                                                            |
| tomli_loads                | 2.42 sec                                                               | 2.41 sec: 1.00x faster                                                           |
| meteor_contest             | 115 ms                                                                 | 116 ms: 1.00x slower                                                             |
| pidigits                   | 188 ms                                                                 | 188 ms: 1.00x slower                                                             |
| pickle_dict                | 33.8 us                                                                | 33.9 us: 1.00x slower                                                            |
| asyncio_tcp_ssl            | 1.81 sec                                                               | 1.81 sec: 1.00x slower                                                           |
| bench_thread_pool          | 846 us                                                                 | 848 us: 1.00x slower                                                             |
| mako                       | 14.1 ms                                                                | 14.1 ms: 1.00x slower                                                            |
| pprint_pformat             | 1.70 sec                                                               | 1.71 sec: 1.00x slower                                                           |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.00x slower                                                            |
| sympy_integrate            | 21.1 ms                                                                | 21.1 ms: 1.00x slower                                                            |
| richards                   | 48.6 ms                                                                | 48.9 ms: 1.00x slower                                                            |
| 2to3                       | 282 ms                                                                 | 284 ms: 1.00x slower                                                             |
| sympy_expand               | 485 ms                                                                 | 487 ms: 1.00x slower                                                             |
| float                      | 92.8 ms                                                                | 93.3 ms: 1.01x slower                                                            |
| python_startup_no_site     | 8.73 ms                                                                | 8.78 ms: 1.01x slower                                                            |
| regex_v8                   | 24.9 ms                                                                | 25.1 ms: 1.01x slower                                                            |
| sqlglot_parse              | 1.32 ms                                                                | 1.33 ms: 1.01x slower                                                            |
| docutils                   | 2.71 sec                                                               | 2.73 sec: 1.01x slower                                                           |
| pickle_pure_python         | 298 us                                                                 | 300 us: 1.01x slower                                                             |
| sqlglot_optimize           | 57.6 ms                                                                | 58.2 ms: 1.01x slower                                                            |
| async_tree_none_tg         | 457 ms                                                                 | 461 ms: 1.01x slower                                                             |
| sympy_sum                  | 159 ms                                                                 | 161 ms: 1.01x slower                                                             |
| asyncio_tcp                | 490 ms                                                                 | 495 ms: 1.01x slower                                                             |
| unpickle_pure_python       | 234 us                                                                 | 236 us: 1.01x slower                                                             |
| xml_etree_generate         | 89.0 ms                                                                | 89.9 ms: 1.01x slower                                                            |
| typing_runtime_protocols   | 117 us                                                                 | 118 us: 1.01x slower                                                             |
| xml_etree_process          | 60.9 ms                                                                | 61.6 ms: 1.01x slower                                                            |
| async_tree_cpu_io_mixed_tg | 731 ms                                                                 | 740 ms: 1.01x slower                                                             |
| coroutines                 | 22.0 ms                                                                | 22.3 ms: 1.01x slower                                                            |
| go                         | 154 ms                                                                 | 156 ms: 1.01x slower                                                             |
| regex_dna                  | 219 ms                                                                 | 223 ms: 1.02x slower                                                             |
| pickle                     | 11.6 us                                                                | 11.8 us: 1.02x slower                                                            |
| hexiom                     | 8.36 ms                                                                | 8.51 ms: 1.02x slower                                                            |
| unpickle                   | 15.0 us                                                                | 15.4 us: 1.03x slower                                                            |
| comprehensions             | 21.3 us                                                                | 21.8 us: 1.03x slower                                                            |
| pathlib                    | 18.5 ms                                                                | 19.1 ms: 1.03x slower                                                            |
| chameleon                  | 7.26 ms                                                                | 7.49 ms: 1.03x slower                                                            |
| crypto_pyaes               | 82.6 ms                                                                | 85.6 ms: 1.04x slower                                                            |
| logging_silent             | 104 ns                                                                 | 108 ns: 1.04x slower                                                             |
| async_tree_memoization_tg  | 587 ms                                                                 | 611 ms: 1.04x slower                                                             |
| gc_traversal               | 3.71 ms                                                                | 3.91 ms: 1.05x slower                                                            |
| unpack_sequence            | 49.3 ns                                                                | 53.0 ns: 1.07x slower                                                            |
| Geometric mean             | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (32): sympy_str, xml_etree_parse, scimark_lu, async_generators, richards_super, pickle_list, coverage, async_tree_io, async_tree_io_tg, sqlglot_normalize, bench_mp_pool, sqlite_synth, json_loads, deepcopy_memo, pprint_safe_repr, regex_compile, json_dumps, asyncio_websockets, async_tree_memoization, create_gc_cycles, dask, telco, nqueens, sqlglot_transpile, xml_etree_iterparse, mypy2, async_tree_none, logging_format, generators, tornado_http, logging_simple, async_tree_cpu_io_mixed


# HPT report

- Reliability score: 98.64% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x