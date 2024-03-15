# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 7de4b37
- commit date: 2024-01-26
- overall geometric mean: 1.00x slower
- HPT reliability: 98.29%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 285 ms: 1.01x slower                                                             |
| chameleon      | 7.26 ms                                                                | 7.39 ms: 1.02x slower                                                            |
| docutils       | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg         | 457 ms                                                                 | 460 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 731 ms                                                                 | 739 ms: 1.01x slower                                                             |
| async_tree_memoization_tg  | 587 ms                                                                 | 594 ms: 1.01x slower                                                             |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (5): async_tree_io_tg, async_tree_io, async_tree_memoization, async_tree_none, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 189 ms: 1.01x slower                                                             |
| nbody          | 119 ms                                                                 | 125 ms: 1.05x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.71 ms                                                                | 3.66 ms: 1.01x faster                                                            |
| regex_v8       | 24.9 ms                                                                | 25.9 ms: 1.04x slower                                                            |
| regex_dna      | 219 ms                                                                 | 228 ms: 1.05x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| xml_etree_parse      | 160 ms                                                                 | 159 ms: 1.01x faster                                                             |
| pickle               | 11.6 us                                                                | 11.5 us: 1.01x faster                                                            |
| json_loads           | 28.3 us                                                                | 28.2 us: 1.01x faster                                                            |
| xml_etree_generate   | 89.0 ms                                                                | 89.7 ms: 1.01x slower                                                            |
| xml_etree_process    | 60.9 ms                                                                | 61.4 ms: 1.01x slower                                                            |
| unpickle             | 15.0 us                                                                | 15.2 us: 1.01x slower                                                            |
| unpickle_pure_python | 234 us                                                                 | 236 us: 1.01x slower                                                             |
| pickle_pure_python   | 298 us                                                                 | 303 us: 1.02x slower                                                             |
| unpickle_list        | 5.35 us                                                                | 5.52 us: 1.03x slower                                                            |
| pickle_list          | 5.02 us                                                                | 5.19 us: 1.03x slower                                                            |
| pickle_dict          | 33.8 us                                                                | 35.2 us: 1.04x slower                                                            |
| tomli_loads          | 2.42 sec                                                               | 2.56 sec: 1.06x slower                                                           |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (2): json_dumps, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| python_startup_no_site | 8.73 ms                                                                | 8.82 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.1 ms                                                                | 13.9 ms: 1.01x faster                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpack_sequence            | 49.3 ns                                                                | 40.6 ns: 1.21x faster                                                            |
| scimark_fft                | 455 ms                                                                 | 432 ms: 1.05x faster                                                             |
| pycparser                  | 1.25 sec                                                               | 1.21 sec: 1.03x faster                                                           |
| deepcopy_reduce            | 3.19 us                                                                | 3.10 us: 1.03x faster                                                            |
| telco                      | 8.76 ms                                                                | 8.56 ms: 1.02x faster                                                            |
| scimark_lu                 | 118 ms                                                                 | 115 ms: 1.02x faster                                                             |
| scimark_monte_carlo        | 80.5 ms                                                                | 79.0 ms: 1.02x faster                                                            |
| chaos                      | 74.1 ms                                                                | 72.7 ms: 1.02x faster                                                            |
| scimark_sparse_mat_mult    | 6.09 ms                                                                | 5.98 ms: 1.02x faster                                                            |
| deltablue                  | 4.72 ms                                                                | 4.65 ms: 1.02x faster                                                            |
| mdp                        | 2.67 sec                                                               | 2.63 sec: 1.01x faster                                                           |
| regex_effbot               | 3.71 ms                                                                | 3.66 ms: 1.01x faster                                                            |
| richards_super             | 55.4 ms                                                                | 54.7 ms: 1.01x faster                                                            |
| raytrace                   | 303 ms                                                                 | 299 ms: 1.01x faster                                                             |
| mako                       | 14.1 ms                                                                | 13.9 ms: 1.01x faster                                                            |
| sqlite_synth               | 2.88 us                                                                | 2.85 us: 1.01x faster                                                            |
| pprint_safe_repr           | 822 ms                                                                 | 814 ms: 1.01x faster                                                             |
| async_generators           | 464 ms                                                                 | 460 ms: 1.01x faster                                                             |
| xml_etree_parse            | 160 ms                                                                 | 159 ms: 1.01x faster                                                             |
| pickle                     | 11.6 us                                                                | 11.5 us: 1.01x faster                                                            |
| sqlglot_normalize          | 114 ms                                                                 | 113 ms: 1.01x faster                                                             |
| json_loads                 | 28.3 us                                                                | 28.2 us: 1.01x faster                                                            |
| richards                   | 48.6 ms                                                                | 48.4 ms: 1.01x faster                                                            |
| pprint_pformat             | 1.70 sec                                                               | 1.70 sec: 1.00x faster                                                           |
| scimark_sor                | 130 ms                                                                 | 130 ms: 1.00x faster                                                             |
| dulwich_log                | 69.3 ms                                                                | 69.1 ms: 1.00x faster                                                            |
| asyncio_tcp_ssl            | 1.81 sec                                                               | 1.80 sec: 1.00x faster                                                           |
| docutils                   | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| create_gc_cycles           | 1.48 ms                                                                | 1.49 ms: 1.00x slower                                                            |
| sqlglot_optimize           | 57.6 ms                                                                | 57.9 ms: 1.00x slower                                                            |
| nqueens                    | 93.5 ms                                                                | 94.1 ms: 1.01x slower                                                            |
| sqlglot_parse              | 1.32 ms                                                                | 1.33 ms: 1.01x slower                                                            |
| sympy_integrate            | 21.1 ms                                                                | 21.2 ms: 1.01x slower                                                            |
| logging_format             | 6.80 us                                                                | 6.84 us: 1.01x slower                                                            |
| pidigits                   | 188 ms                                                                 | 189 ms: 1.01x slower                                                             |
| pathlib                    | 18.5 ms                                                                | 18.7 ms: 1.01x slower                                                            |
| xml_etree_generate         | 89.0 ms                                                                | 89.7 ms: 1.01x slower                                                            |
| async_tree_none_tg         | 457 ms                                                                 | 460 ms: 1.01x slower                                                             |
| coroutines                 | 22.0 ms                                                                | 22.1 ms: 1.01x slower                                                            |
| xml_etree_process          | 60.9 ms                                                                | 61.4 ms: 1.01x slower                                                            |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| unpickle                   | 15.0 us                                                                | 15.2 us: 1.01x slower                                                            |
| 2to3                       | 282 ms                                                                 | 285 ms: 1.01x slower                                                             |
| unpickle_pure_python       | 234 us                                                                 | 236 us: 1.01x slower                                                             |
| python_startup_no_site     | 8.73 ms                                                                | 8.82 ms: 1.01x slower                                                            |
| comprehensions             | 21.3 us                                                                | 21.5 us: 1.01x slower                                                            |
| async_tree_cpu_io_mixed_tg | 731 ms                                                                 | 739 ms: 1.01x slower                                                             |
| go                         | 154 ms                                                                 | 156 ms: 1.01x slower                                                             |
| async_tree_memoization_tg  | 587 ms                                                                 | 594 ms: 1.01x slower                                                             |
| pickle_pure_python         | 298 us                                                                 | 303 us: 1.02x slower                                                             |
| hexiom                     | 8.36 ms                                                                | 8.49 ms: 1.02x slower                                                            |
| chameleon                  | 7.26 ms                                                                | 7.39 ms: 1.02x slower                                                            |
| crypto_pyaes               | 82.6 ms                                                                | 84.9 ms: 1.03x slower                                                            |
| gc_traversal               | 3.71 ms                                                                | 3.82 ms: 1.03x slower                                                            |
| pyflate                    | 529 ms                                                                 | 546 ms: 1.03x slower                                                             |
| unpickle_list              | 5.35 us                                                                | 5.52 us: 1.03x slower                                                            |
| logging_silent             | 104 ns                                                                 | 107 ns: 1.03x slower                                                             |
| pickle_list                | 5.02 us                                                                | 5.19 us: 1.03x slower                                                            |
| regex_v8                   | 24.9 ms                                                                | 25.9 ms: 1.04x slower                                                            |
| pickle_dict                | 33.8 us                                                                | 35.2 us: 1.04x slower                                                            |
| regex_dna                  | 219 ms                                                                 | 228 ms: 1.05x slower                                                             |
| nbody                      | 119 ms                                                                 | 125 ms: 1.05x slower                                                             |
| tomli_loads                | 2.42 sec                                                               | 2.56 sec: 1.06x slower                                                           |
| Geometric mean             | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (30): sympy_str, coverage, spectral_norm, json_dumps, dask, deepcopy_memo, json, asyncio_tcp, meteor_contest, float, bench_mp_pool, tornado_http, bench_thread_pool, deepcopy, sqlglot_transpile, async_tree_io_tg, async_tree_io, asyncio_websockets, fannkuch, sympy_sum, logging_simple, sympy_expand, regex_compile, typing_runtime_protocols, generators, async_tree_memoization, async_tree_none, xml_etree_iterparse, mypy2, async_tree_cpu_io_mixed


# HPT report

- Reliability score: 98.29% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x