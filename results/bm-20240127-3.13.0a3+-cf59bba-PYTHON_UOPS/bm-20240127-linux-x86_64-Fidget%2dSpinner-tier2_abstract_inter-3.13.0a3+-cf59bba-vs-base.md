# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 283 ms: 1.00x slower                                                             |
| chameleon      | 7.26 ms                                                                | 7.16 ms: 1.01x faster                                                            |
| docutils       | 2.71 sec                                                               | 2.69 sec: 1.01x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io    | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| async_tree_io_tg | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| Geometric mean   | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (6): async_tree_memoization, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 92.8 ms                                                                | 87.7 ms: 1.06x faster                                                            |
| nbody          | 119 ms                                                                 | 113 ms: 1.05x faster                                                             |
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x faster                                                             |
| Geometric mean | (ref)                                                                  | 1.04x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.71 ms                                                                | 3.56 ms: 1.04x faster                                                            |
| regex_compile  | 152 ms                                                                 | 148 ms: 1.02x faster                                                             |
| regex_dna      | 219 ms                                                                 | 222 ms: 1.02x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|---------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list       | 5.35 us                                                                | 4.94 us: 1.08x faster                                                            |
| tomli_loads         | 2.42 sec                                                               | 2.31 sec: 1.05x faster                                                           |
| xml_etree_parse     | 160 ms                                                                 | 157 ms: 1.02x faster                                                             |
| json_dumps          | 10.5 ms                                                                | 10.4 ms: 1.02x faster                                                            |
| xml_etree_iterparse | 111 ms                                                                 | 110 ms: 1.01x faster                                                             |
| xml_etree_process   | 60.9 ms                                                                | 60.5 ms: 1.01x faster                                                            |
| pickle_dict         | 33.8 us                                                                | 34.8 us: 1.03x slower                                                            |
| pickle_list         | 5.02 us                                                                | 5.23 us: 1.04x slower                                                            |
| Geometric mean      | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (6): pickle_pure_python, unpickle, json_loads, unpickle_pure_python, xml_etree_generate, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                            |
| python_startup_no_site | 8.73 ms                                                                | 8.79 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.1 ms                                                                | 12.9 ms: 1.09x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpack_sequence          | 49.3 ns                                                                | 40.7 ns: 1.21x faster                                                            |
| scimark_sparse_mat_mult  | 6.09 ms                                                                | 5.50 ms: 1.11x faster                                                            |
| scimark_fft              | 455 ms                                                                 | 414 ms: 1.10x faster                                                             |
| mako                     | 14.1 ms                                                                | 12.9 ms: 1.09x faster                                                            |
| spectral_norm            | 144 ms                                                                 | 132 ms: 1.09x faster                                                             |
| unpickle_list            | 5.35 us                                                                | 4.94 us: 1.08x faster                                                            |
| deltablue                | 4.72 ms                                                                | 4.41 ms: 1.07x faster                                                            |
| float                    | 92.8 ms                                                                | 87.7 ms: 1.06x faster                                                            |
| chaos                    | 74.1 ms                                                                | 70.2 ms: 1.06x faster                                                            |
| nbody                    | 119 ms                                                                 | 113 ms: 1.05x faster                                                             |
| tomli_loads              | 2.42 sec                                                               | 2.31 sec: 1.05x faster                                                           |
| fannkuch                 | 450 ms                                                                 | 429 ms: 1.05x faster                                                             |
| hexiom                   | 8.36 ms                                                                | 8.01 ms: 1.04x faster                                                            |
| regex_effbot             | 3.71 ms                                                                | 3.56 ms: 1.04x faster                                                            |
| pyflate                  | 529 ms                                                                 | 508 ms: 1.04x faster                                                             |
| scimark_monte_carlo      | 80.5 ms                                                                | 77.5 ms: 1.04x faster                                                            |
| pycparser                | 1.25 sec                                                               | 1.20 sec: 1.04x faster                                                           |
| comprehensions           | 21.3 us                                                                | 20.6 us: 1.03x faster                                                            |
| raytrace                 | 303 ms                                                                 | 294 ms: 1.03x faster                                                             |
| pprint_pformat           | 1.70 sec                                                               | 1.66 sec: 1.03x faster                                                           |
| regex_compile            | 152 ms                                                                 | 148 ms: 1.02x faster                                                             |
| scimark_sor              | 130 ms                                                                 | 128 ms: 1.02x faster                                                             |
| mdp                      | 2.67 sec                                                               | 2.61 sec: 1.02x faster                                                           |
| pprint_safe_repr         | 822 ms                                                                 | 806 ms: 1.02x faster                                                             |
| coverage                 | 95.3 ms                                                                | 93.5 ms: 1.02x faster                                                            |
| async_generators         | 464 ms                                                                 | 456 ms: 1.02x faster                                                             |
| xml_etree_parse          | 160 ms                                                                 | 157 ms: 1.02x faster                                                             |
| telco                    | 8.76 ms                                                                | 8.62 ms: 1.02x faster                                                            |
| json_dumps               | 10.5 ms                                                                | 10.4 ms: 1.02x faster                                                            |
| nqueens                  | 93.5 ms                                                                | 92.2 ms: 1.01x faster                                                            |
| sympy_str                | 294 ms                                                                 | 290 ms: 1.01x faster                                                             |
| xml_etree_iterparse      | 111 ms                                                                 | 110 ms: 1.01x faster                                                             |
| chameleon                | 7.26 ms                                                                | 7.16 ms: 1.01x faster                                                            |
| meteor_contest           | 115 ms                                                                 | 114 ms: 1.01x faster                                                             |
| json                     | 5.23 ms                                                                | 5.17 ms: 1.01x faster                                                            |
| async_tree_io            | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| sqlglot_normalize        | 114 ms                                                                 | 113 ms: 1.01x faster                                                             |
| typing_runtime_protocols | 117 us                                                                 | 116 us: 1.01x faster                                                             |
| async_tree_io_tg         | 1.21 sec                                                               | 1.20 sec: 1.01x faster                                                           |
| docutils                 | 2.71 sec                                                               | 2.69 sec: 1.01x faster                                                           |
| xml_etree_process        | 60.9 ms                                                                | 60.5 ms: 1.01x faster                                                            |
| dulwich_log              | 69.3 ms                                                                | 68.8 ms: 1.01x faster                                                            |
| asyncio_tcp              | 490 ms                                                                 | 488 ms: 1.01x faster                                                             |
| asyncio_tcp_ssl          | 1.81 sec                                                               | 1.80 sec: 1.01x faster                                                           |
| crypto_pyaes             | 82.6 ms                                                                | 82.2 ms: 1.00x faster                                                            |
| bench_thread_pool        | 846 us                                                                 | 842 us: 1.00x faster                                                             |
| pidigits                 | 188 ms                                                                 | 188 ms: 1.00x faster                                                             |
| 2to3                     | 282 ms                                                                 | 283 ms: 1.00x slower                                                             |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                            |
| gc_traversal             | 3.71 ms                                                                | 3.72 ms: 1.00x slower                                                            |
| richards                 | 48.6 ms                                                                | 48.9 ms: 1.00x slower                                                            |
| sympy_expand             | 485 ms                                                                 | 487 ms: 1.00x slower                                                             |
| deepcopy                 | 359 us                                                                 | 361 us: 1.01x slower                                                             |
| pathlib                  | 18.5 ms                                                                | 18.6 ms: 1.01x slower                                                            |
| go                       | 154 ms                                                                 | 155 ms: 1.01x slower                                                             |
| python_startup_no_site   | 8.73 ms                                                                | 8.79 ms: 1.01x slower                                                            |
| regex_dna                | 219 ms                                                                 | 222 ms: 1.02x slower                                                             |
| scimark_lu               | 118 ms                                                                 | 120 ms: 1.02x slower                                                             |
| pickle_dict              | 33.8 us                                                                | 34.8 us: 1.03x slower                                                            |
| coroutines               | 22.0 ms                                                                | 22.7 ms: 1.03x slower                                                            |
| pickle_list              | 5.02 us                                                                | 5.23 us: 1.04x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (32): logging_format, generators, logging_silent, pickle_pure_python, async_tree_memoization, tornado_http, unpickle, sqlglot_transpile, richards_super, sympy_sum, deepcopy_reduce, async_tree_none_tg, sqlglot_parse, async_tree_cpu_io_mixed, create_gc_cycles, sqlglot_optimize, json_loads, sympy_integrate, regex_v8, deepcopy_memo, dask, asyncio_websockets, async_tree_none, unpickle_pure_python, bench_mp_pool, sqlite_synth, logging_simple, xml_etree_generate, async_tree_cpu_io_mixed_tg, mypy2, pickle, async_tree_memoization_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x