# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.02x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 289 ms: 1.02x slower                                                             |
| chameleon      | 7.26 ms                                                                | 7.52 ms: 1.04x slower                                                            |
| docutils       | 2.71 sec                                                               | 2.74 sec: 1.01x slower                                                           |
| tornado_http   | 98.7 ms                                                                | 101 ms: 1.03x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io_tg          | 1.21 sec                                                               | 1.22 sec: 1.00x slower                                                           |
| async_tree_none_tg        | 457 ms                                                                 | 462 ms: 1.01x slower                                                             |
| async_tree_memoization_tg | 587 ms                                                                 | 609 ms: 1.04x slower                                                             |
| Geometric mean            | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (5): async_tree_io, async_tree_none, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 189 ms: 1.01x slower                                                             |
| float          | 92.8 ms                                                                | 101 ms: 1.09x slower                                                             |
| nbody          | 119 ms                                                                 | 135 ms: 1.14x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.71 ms                                                                | 3.54 ms: 1.05x faster                                                            |
| regex_v8       | 24.9 ms                                                                | 24.5 ms: 1.02x faster                                                            |
| regex_dna      | 219 ms                                                                 | 220 ms: 1.01x slower                                                             |
| regex_compile  | 152 ms                                                                 | 156 ms: 1.03x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 5.35 us                                                                | 5.06 us: 1.06x faster                                                            |
| xml_etree_parse      | 160 ms                                                                 | 158 ms: 1.01x faster                                                             |
| pickle               | 11.6 us                                                                | 11.6 us: 1.00x slower                                                            |
| xml_etree_process    | 60.9 ms                                                                | 61.5 ms: 1.01x slower                                                            |
| xml_etree_generate   | 89.0 ms                                                                | 90.0 ms: 1.01x slower                                                            |
| pickle_dict          | 33.8 us                                                                | 34.2 us: 1.01x slower                                                            |
| unpickle_pure_python | 234 us                                                                 | 240 us: 1.03x slower                                                             |
| pickle_list          | 5.02 us                                                                | 5.15 us: 1.03x slower                                                            |
| xml_etree_iterparse  | 111 ms                                                                 | 115 ms: 1.03x slower                                                             |
| tomli_loads          | 2.42 sec                                                               | 2.74 sec: 1.13x slower                                                           |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (4): json_loads, json_dumps, pickle_pure_python, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| python_startup_no_site | 8.73 ms                                                                | 8.82 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.1 ms                                                                | 14.8 ms: 1.05x slower                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20240124-linux-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list             | 5.35 us                                                                | 5.06 us: 1.06x faster                                                            |
| regex_effbot              | 3.71 ms                                                                | 3.54 ms: 1.05x faster                                                            |
| unpack_sequence           | 49.3 ns                                                                | 47.8 ns: 1.03x faster                                                            |
| deepcopy_reduce           | 3.19 us                                                                | 3.13 us: 1.02x faster                                                            |
| regex_v8                  | 24.9 ms                                                                | 24.5 ms: 1.02x faster                                                            |
| gc_traversal              | 3.71 ms                                                                | 3.65 ms: 1.01x faster                                                            |
| xml_etree_parse           | 160 ms                                                                 | 158 ms: 1.01x faster                                                             |
| telco                     | 8.76 ms                                                                | 8.66 ms: 1.01x faster                                                            |
| json                      | 5.23 ms                                                                | 5.18 ms: 1.01x faster                                                            |
| async_generators          | 464 ms                                                                 | 460 ms: 1.01x faster                                                             |
| pathlib                   | 18.5 ms                                                                | 18.4 ms: 1.01x faster                                                            |
| create_gc_cycles          | 1.48 ms                                                                | 1.47 ms: 1.01x faster                                                            |
| deepcopy                  | 359 us                                                                 | 357 us: 1.00x faster                                                             |
| scimark_sparse_mat_mult   | 6.09 ms                                                                | 6.06 ms: 1.00x faster                                                            |
| mdp                       | 2.67 sec                                                               | 2.66 sec: 1.00x faster                                                           |
| asyncio_tcp_ssl           | 1.81 sec                                                               | 1.81 sec: 1.00x slower                                                           |
| pickle                    | 11.6 us                                                                | 11.6 us: 1.00x slower                                                            |
| async_tree_io_tg          | 1.21 sec                                                               | 1.22 sec: 1.00x slower                                                           |
| pycparser                 | 1.25 sec                                                               | 1.25 sec: 1.00x slower                                                           |
| pidigits                  | 188 ms                                                                 | 189 ms: 1.01x slower                                                             |
| regex_dna                 | 219 ms                                                                 | 220 ms: 1.01x slower                                                             |
| python_startup            | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| scimark_fft               | 455 ms                                                                 | 459 ms: 1.01x slower                                                             |
| xml_etree_process         | 60.9 ms                                                                | 61.5 ms: 1.01x slower                                                            |
| docutils                  | 2.71 sec                                                               | 2.74 sec: 1.01x slower                                                           |
| python_startup_no_site    | 8.73 ms                                                                | 8.82 ms: 1.01x slower                                                            |
| logging_format            | 6.80 us                                                                | 6.87 us: 1.01x slower                                                            |
| spectral_norm             | 144 ms                                                                 | 145 ms: 1.01x slower                                                             |
| xml_etree_generate        | 89.0 ms                                                                | 90.0 ms: 1.01x slower                                                            |
| bench_thread_pool         | 846 us                                                                 | 855 us: 1.01x slower                                                             |
| async_tree_none_tg        | 457 ms                                                                 | 462 ms: 1.01x slower                                                             |
| pickle_dict               | 33.8 us                                                                | 34.2 us: 1.01x slower                                                            |
| sqlglot_normalize         | 114 ms                                                                 | 116 ms: 1.01x slower                                                             |
| sqlite_synth              | 2.88 us                                                                | 2.92 us: 1.01x slower                                                            |
| logging_silent            | 104 ns                                                                 | 106 ns: 1.02x slower                                                             |
| sqlglot_transpile         | 1.66 ms                                                                | 1.69 ms: 1.02x slower                                                            |
| asyncio_tcp               | 490 ms                                                                 | 500 ms: 1.02x slower                                                             |
| pyflate                   | 529 ms                                                                 | 540 ms: 1.02x slower                                                             |
| scimark_lu                | 118 ms                                                                 | 121 ms: 1.02x slower                                                             |
| meteor_contest            | 115 ms                                                                 | 118 ms: 1.02x slower                                                             |
| 2to3                      | 282 ms                                                                 | 289 ms: 1.02x slower                                                             |
| pprint_safe_repr          | 822 ms                                                                 | 842 ms: 1.02x slower                                                             |
| sqlglot_parse             | 1.32 ms                                                                | 1.35 ms: 1.02x slower                                                            |
| sqlglot_optimize          | 57.6 ms                                                                | 59.0 ms: 1.02x slower                                                            |
| sympy_integrate           | 21.1 ms                                                                | 21.6 ms: 1.02x slower                                                            |
| unpickle_pure_python      | 234 us                                                                 | 240 us: 1.03x slower                                                             |
| pickle_list               | 5.02 us                                                                | 5.15 us: 1.03x slower                                                            |
| pprint_pformat            | 1.70 sec                                                               | 1.75 sec: 1.03x slower                                                           |
| richards_super            | 55.4 ms                                                                | 57.0 ms: 1.03x slower                                                            |
| tornado_http              | 98.7 ms                                                                | 101 ms: 1.03x slower                                                             |
| sympy_sum                 | 159 ms                                                                 | 164 ms: 1.03x slower                                                             |
| regex_compile             | 152 ms                                                                 | 156 ms: 1.03x slower                                                             |
| sympy_str                 | 294 ms                                                                 | 303 ms: 1.03x slower                                                             |
| raytrace                  | 303 ms                                                                 | 312 ms: 1.03x slower                                                             |
| typing_runtime_protocols  | 117 us                                                                 | 121 us: 1.03x slower                                                             |
| xml_etree_iterparse       | 111 ms                                                                 | 115 ms: 1.03x slower                                                             |
| chaos                     | 74.1 ms                                                                | 76.8 ms: 1.04x slower                                                            |
| chameleon                 | 7.26 ms                                                                | 7.52 ms: 1.04x slower                                                            |
| async_tree_memoization_tg | 587 ms                                                                 | 609 ms: 1.04x slower                                                             |
| go                        | 154 ms                                                                 | 160 ms: 1.04x slower                                                             |
| sympy_expand              | 485 ms                                                                 | 504 ms: 1.04x slower                                                             |
| fannkuch                  | 450 ms                                                                 | 468 ms: 1.04x slower                                                             |
| richards                  | 48.6 ms                                                                | 50.6 ms: 1.04x slower                                                            |
| coroutines                | 22.0 ms                                                                | 22.9 ms: 1.04x slower                                                            |
| mako                      | 14.1 ms                                                                | 14.8 ms: 1.05x slower                                                            |
| nqueens                   | 93.5 ms                                                                | 98.6 ms: 1.05x slower                                                            |
| scimark_monte_carlo       | 80.5 ms                                                                | 86.3 ms: 1.07x slower                                                            |
| float                     | 92.8 ms                                                                | 101 ms: 1.09x slower                                                             |
| comprehensions            | 21.3 us                                                                | 23.1 us: 1.09x slower                                                            |
| crypto_pyaes              | 82.6 ms                                                                | 90.4 ms: 1.09x slower                                                            |
| deltablue                 | 4.72 ms                                                                | 5.18 ms: 1.10x slower                                                            |
| hexiom                    | 8.36 ms                                                                | 9.23 ms: 1.11x slower                                                            |
| tomli_loads               | 2.42 sec                                                               | 2.74 sec: 1.13x slower                                                           |
| nbody                     | 119 ms                                                                 | 135 ms: 1.14x slower                                                             |
| Geometric mean            | (ref)                                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (19): json_loads, coverage, json_dumps, dulwich_log, scimark_sor, asyncio_websockets, async_tree_io, bench_mp_pool, generators, deepcopy_memo, dask, async_tree_none, logging_simple, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, pickle_pure_python, unpickle, async_tree_memoization, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x