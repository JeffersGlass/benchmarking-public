# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 176 ms                                                                 | 174 ms: 1.01x faster                                                             |
| chameleon      | 5.04 ms                                                                | 5.07 ms: 1.01x slower                                                            |
| docutils       | 1.51 sec                                                               | 1.49 sec: 1.01x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg | 268 ms                                                                 | 265 ms: 1.01x faster                                                             |
| async_tree_io      | 714 ms                                                                 | 709 ms: 1.01x faster                                                             |
| async_tree_io_tg   | 679 ms                                                                 | 677 ms: 1.00x faster                                                             |
| Geometric mean     | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (5): async_tree_none, async_tree_memoization_tg, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 97.3 ms                                                                | 81.9 ms: 1.19x faster                                                            |
| float          | 74.6 ms                                                                | 67.0 ms: 1.11x faster                                                            |
| pidigits       | 284 ms                                                                 | 284 ms: 1.00x faster                                                             |
| Geometric mean | (ref)                                                                  | 1.10x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 84.8 ms                                                                | 81.8 ms: 1.04x faster                                                            |
| regex_v8       | 18.1 ms                                                                | 18.0 ms: 1.00x faster                                                            |
| regex_effbot   | 2.78 ms                                                                | 2.78 ms: 1.00x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 1.80 sec                                                               | 1.62 sec: 1.11x faster                                                           |
| xml_etree_iterparse  | 83.2 ms                                                                | 80.8 ms: 1.03x faster                                                            |
| xml_etree_generate   | 60.1 ms                                                                | 58.5 ms: 1.03x faster                                                            |
| xml_etree_process    | 41.6 ms                                                                | 40.6 ms: 1.03x faster                                                            |
| unpickle_pure_python | 167 us                                                                 | 164 us: 1.02x faster                                                             |
| pickle_pure_python   | 198 us                                                                 | 196 us: 1.01x faster                                                             |
| unpickle             | 9.21 us                                                                | 9.17 us: 1.00x faster                                                            |
| pickle_dict          | 18.1 us                                                                | 18.1 us: 1.00x faster                                                            |
| json_dumps           | 6.57 ms                                                                | 6.56 ms: 1.00x faster                                                            |
| Geometric mean       | (ref)                                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (5): unpickle_list, pickle_list, json_loads, pickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 11.4 ms                                                                | 11.5 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.8 ms                                                                | 9.65 ms: 1.12x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| spectral_norm            | 119 ms                                                                 | 96.6 ms: 1.23x faster                                                            |
| nbody                    | 97.3 ms                                                                | 81.9 ms: 1.19x faster                                                            |
| scimark_fft              | 276 ms                                                                 | 233 ms: 1.18x faster                                                             |
| scimark_sparse_mat_mult  | 4.52 ms                                                                | 3.96 ms: 1.14x faster                                                            |
| mako                     | 10.8 ms                                                                | 9.65 ms: 1.12x faster                                                            |
| float                    | 74.6 ms                                                                | 67.0 ms: 1.11x faster                                                            |
| tomli_loads              | 1.80 sec                                                               | 1.62 sec: 1.11x faster                                                           |
| comprehensions           | 16.8 us                                                                | 15.1 us: 1.11x faster                                                            |
| deltablue                | 3.92 ms                                                                | 3.52 ms: 1.11x faster                                                            |
| hexiom                   | 6.47 ms                                                                | 5.87 ms: 1.10x faster                                                            |
| chaos                    | 49.9 ms                                                                | 45.5 ms: 1.10x faster                                                            |
| scimark_monte_carlo      | 60.0 ms                                                                | 56.1 ms: 1.07x faster                                                            |
| nqueens                  | 71.8 ms                                                                | 67.1 ms: 1.07x faster                                                            |
| pyflate                  | 391 ms                                                                 | 367 ms: 1.06x faster                                                             |
| crypto_pyaes             | 58.5 ms                                                                | 55.2 ms: 1.06x faster                                                            |
| pprint_pformat           | 1.22 sec                                                               | 1.16 sec: 1.05x faster                                                           |
| fannkuch                 | 333 ms                                                                 | 318 ms: 1.04x faster                                                             |
| pprint_safe_repr         | 591 ms                                                                 | 567 ms: 1.04x faster                                                             |
| regex_compile            | 84.8 ms                                                                | 81.8 ms: 1.04x faster                                                            |
| scimark_lu               | 78.0 ms                                                                | 75.4 ms: 1.03x faster                                                            |
| go                       | 115 ms                                                                 | 111 ms: 1.03x faster                                                             |
| xml_etree_iterparse      | 83.2 ms                                                                | 80.8 ms: 1.03x faster                                                            |
| typing_runtime_protocols | 75.3 us                                                                | 73.1 us: 1.03x faster                                                            |
| raytrace                 | 189 ms                                                                 | 184 ms: 1.03x faster                                                             |
| meteor_contest           | 79.3 ms                                                                | 77.1 ms: 1.03x faster                                                            |
| telco                    | 4.75 ms                                                                | 4.63 ms: 1.03x faster                                                            |
| xml_etree_generate       | 60.1 ms                                                                | 58.5 ms: 1.03x faster                                                            |
| xml_etree_process        | 41.6 ms                                                                | 40.6 ms: 1.03x faster                                                            |
| logging_format           | 3.94 us                                                                | 3.85 us: 1.02x faster                                                            |
| mdp                      | 1.65 sec                                                               | 1.61 sec: 1.02x faster                                                           |
| coverage                 | 48.1 ms                                                                | 47.1 ms: 1.02x faster                                                            |
| logging_simple           | 3.64 us                                                                | 3.57 us: 1.02x faster                                                            |
| deepcopy_memo            | 27.2 us                                                                | 26.7 us: 1.02x faster                                                            |
| sympy_integrate          | 11.8 ms                                                                | 11.5 ms: 1.02x faster                                                            |
| sympy_str                | 151 ms                                                                 | 149 ms: 1.02x faster                                                             |
| unpickle_pure_python     | 167 us                                                                 | 164 us: 1.02x faster                                                             |
| sympy_sum                | 80.4 ms                                                                | 79.3 ms: 1.01x faster                                                            |
| sqlglot_transpile        | 1.01 ms                                                                | 992 us: 1.01x faster                                                             |
| richards_super           | 36.9 ms                                                                | 36.5 ms: 1.01x faster                                                            |
| json                     | 2.98 ms                                                                | 2.95 ms: 1.01x faster                                                            |
| sqlglot_normalize        | 193 ms                                                                 | 191 ms: 1.01x faster                                                             |
| docutils                 | 1.51 sec                                                               | 1.49 sec: 1.01x faster                                                           |
| async_tree_none_tg       | 268 ms                                                                 | 265 ms: 1.01x faster                                                             |
| sqlglot_optimize         | 36.4 ms                                                                | 36.0 ms: 1.01x faster                                                            |
| sympy_expand             | 248 ms                                                                 | 245 ms: 1.01x faster                                                             |
| richards                 | 33.1 ms                                                                | 32.8 ms: 1.01x faster                                                            |
| sqlglot_parse            | 818 us                                                                 | 810 us: 1.01x faster                                                             |
| 2to3                     | 176 ms                                                                 | 174 ms: 1.01x faster                                                             |
| sqlite_synth             | 1.66 us                                                                | 1.65 us: 1.01x faster                                                            |
| scimark_sor              | 107 ms                                                                 | 106 ms: 1.01x faster                                                             |
| bench_thread_pool        | 514 us                                                                 | 510 us: 1.01x faster                                                             |
| generators               | 28.9 ms                                                                | 28.7 ms: 1.01x faster                                                            |
| pycparser                | 706 ms                                                                 | 701 ms: 1.01x faster                                                             |
| pickle_pure_python       | 198 us                                                                 | 196 us: 1.01x faster                                                             |
| async_tree_io            | 714 ms                                                                 | 709 ms: 1.01x faster                                                             |
| create_gc_cycles         | 709 us                                                                 | 704 us: 1.01x faster                                                             |
| deepcopy                 | 229 us                                                                 | 227 us: 1.01x faster                                                             |
| unpickle                 | 9.21 us                                                                | 9.17 us: 1.00x faster                                                            |
| dulwich_log              | 30.2 ms                                                                | 30.0 ms: 1.00x faster                                                            |
| async_generators         | 298 ms                                                                 | 297 ms: 1.00x faster                                                             |
| async_tree_io_tg         | 679 ms                                                                 | 677 ms: 1.00x faster                                                             |
| regex_v8                 | 18.1 ms                                                                | 18.0 ms: 1.00x faster                                                            |
| deepcopy_reduce          | 2.00 us                                                                | 2.00 us: 1.00x faster                                                            |
| pickle_dict              | 18.1 us                                                                | 18.1 us: 1.00x faster                                                            |
| logging_silent           | 72.5 ns                                                                | 72.3 ns: 1.00x faster                                                            |
| json_dumps               | 6.57 ms                                                                | 6.56 ms: 1.00x faster                                                            |
| pidigits                 | 284 ms                                                                 | 284 ms: 1.00x faster                                                             |
| regex_effbot             | 2.78 ms                                                                | 2.78 ms: 1.00x faster                                                            |
| chameleon                | 5.04 ms                                                                | 5.07 ms: 1.01x slower                                                            |
| python_startup_no_site   | 11.4 ms                                                                | 11.5 ms: 1.01x slower                                                            |
| coroutines               | 19.5 ms                                                                | 19.7 ms: 1.01x slower                                                            |
| unpack_sequence          | 28.3 ns                                                                | 29.2 ns: 1.03x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.03x faster                                                                     |

Benchmark hidden because not significant (21): async_tree_none, async_tree_memoization_tg, async_tree_memoization, async_tree_cpu_io_mixed, pathlib, asyncio_tcp, async_tree_cpu_io_mixed_tg, unpickle_list, mypy2, dask, gc_traversal, pickle_list, json_loads, python_startup, asyncio_websockets, regex_dna, asyncio_tcp_ssl, pickle, bench_mp_pool, tornado_http, xml_etree_parse


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x