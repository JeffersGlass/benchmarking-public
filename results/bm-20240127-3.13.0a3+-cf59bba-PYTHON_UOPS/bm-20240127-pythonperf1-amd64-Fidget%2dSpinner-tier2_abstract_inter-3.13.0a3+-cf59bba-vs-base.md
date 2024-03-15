# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.00x faster
- HPT reliability: 87.39%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 223 ms                                                                      | 229 ms: 1.03x slower                                                                  |
| chameleon      | 5.12 ms                                                                     | 5.05 ms: 1.01x faster                                                                 |
| Geometric mean | (ref)                                                                       | 1.00x slower                                                                          |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_memoization  | 349 ms                                                                      | 343 ms: 1.02x faster                                                                  |
| async_tree_cpu_io_mixed | 472 ms                                                                      | 466 ms: 1.01x faster                                                                  |
| Geometric mean          | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (6): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_none_tg, async_tree_io_tg, async_tree_none, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| nbody          | 78.4 ms                                                                     | 77.0 ms: 1.02x faster                                                                 |
| pidigits       | 147 ms                                                                      | 149 ms: 1.01x slower                                                                  |
| Geometric mean | (ref)                                                                       | 1.00x slower                                                                          |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_effbot   | 1.56 ms                                                                     | 1.60 ms: 1.03x slower                                                                 |
| regex_dna      | 118 ms                                                                      | 122 ms: 1.04x slower                                                                  |
| regex_v8       | 14.7 ms                                                                     | 15.7 ms: 1.07x slower                                                                 |
| Geometric mean | (ref)                                                                       | 1.03x slower                                                                          |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pickle_dict          | 18.7 us                                                                     | 18.4 us: 1.01x faster                                                                 |
| tomli_loads          | 1.42 sec                                                                    | 1.40 sec: 1.01x faster                                                                |
| xml_etree_parse      | 95.2 ms                                                                     | 94.1 ms: 1.01x faster                                                                 |
| pickle               | 7.30 us                                                                     | 7.22 us: 1.01x faster                                                                 |
| xml_etree_generate   | 56.0 ms                                                                     | 55.5 ms: 1.01x faster                                                                 |
| json_dumps           | 5.70 ms                                                                     | 5.66 ms: 1.01x faster                                                                 |
| xml_etree_iterparse  | 68.2 ms                                                                     | 68.9 ms: 1.01x slower                                                                 |
| pickle_pure_python   | 183 us                                                                      | 186 us: 1.02x slower                                                                  |
| unpickle_pure_python | 137 us                                                                      | 139 us: 1.02x slower                                                                  |
| unpickle_list        | 2.65 us                                                                     | 2.73 us: 1.03x slower                                                                 |
| pickle_list          | 2.89 us                                                                     | 2.98 us: 1.03x slower                                                                 |
| Geometric mean       | (ref)                                                                       | 1.00x slower                                                                          |

Benchmark hidden because not significant (3): unpickle, xml_etree_process, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 20.5 ms                                                                     | 20.8 ms: 1.01x slower                                                                 |
| python_startup_no_site | 18.3 ms                                                                     | 18.9 ms: 1.03x slower                                                                 |
| Geometric mean         | (ref)                                                                       | 1.02x slower                                                                          |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|--------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| asyncio_tcp_ssl          | 1.90 sec                                                                    | 1.72 sec: 1.11x faster                                                                |
| spectral_norm            | 81.0 ms                                                                     | 76.2 ms: 1.06x faster                                                                 |
| scimark_sparse_mat_mult  | 3.05 ms                                                                     | 2.91 ms: 1.05x faster                                                                 |
| scimark_fft              | 207 ms                                                                      | 198 ms: 1.05x faster                                                                  |
| sqlglot_parse            | 810 us                                                                      | 780 us: 1.04x faster                                                                  |
| comprehensions           | 13.0 us                                                                     | 12.5 us: 1.03x faster                                                                 |
| deltablue                | 2.68 ms                                                                     | 2.61 ms: 1.03x faster                                                                 |
| unpack_sequence          | 39.9 ns                                                                     | 39.1 ns: 1.02x faster                                                                 |
| sqlglot_optimize         | 35.6 ms                                                                     | 34.9 ms: 1.02x faster                                                                 |
| nbody                    | 78.4 ms                                                                     | 77.0 ms: 1.02x faster                                                                 |
| nqueens                  | 64.9 ms                                                                     | 63.8 ms: 1.02x faster                                                                 |
| async_tree_memoization   | 349 ms                                                                      | 343 ms: 1.02x faster                                                                  |
| logging_format           | 6.69 us                                                                     | 6.59 us: 1.02x faster                                                                 |
| chameleon                | 5.12 ms                                                                     | 5.05 ms: 1.01x faster                                                                 |
| sqlglot_transpile        | 1.02 ms                                                                     | 1.01 ms: 1.01x faster                                                                 |
| hexiom                   | 4.85 ms                                                                     | 4.78 ms: 1.01x faster                                                                 |
| async_tree_cpu_io_mixed  | 472 ms                                                                      | 466 ms: 1.01x faster                                                                  |
| pickle_dict              | 18.7 us                                                                     | 18.4 us: 1.01x faster                                                                 |
| chaos                    | 44.1 ms                                                                     | 43.5 ms: 1.01x faster                                                                 |
| tomli_loads              | 1.42 sec                                                                    | 1.40 sec: 1.01x faster                                                                |
| xml_etree_parse          | 95.2 ms                                                                     | 94.1 ms: 1.01x faster                                                                 |
| typing_runtime_protocols | 75.7 us                                                                     | 74.8 us: 1.01x faster                                                                 |
| pickle                   | 7.30 us                                                                     | 7.22 us: 1.01x faster                                                                 |
| crypto_pyaes             | 48.6 ms                                                                     | 48.1 ms: 1.01x faster                                                                 |
| xml_etree_generate       | 56.0 ms                                                                     | 55.5 ms: 1.01x faster                                                                 |
| json_dumps               | 5.70 ms                                                                     | 5.66 ms: 1.01x faster                                                                 |
| scimark_sor              | 84.4 ms                                                                     | 83.8 ms: 1.01x faster                                                                 |
| sqlglot_normalize        | 183 ms                                                                      | 182 ms: 1.01x faster                                                                  |
| mypy2                    | 434 ms                                                                      | 432 ms: 1.01x faster                                                                  |
| pprint_safe_repr         | 525 ms                                                                      | 523 ms: 1.00x faster                                                                  |
| sympy_expand             | 285 ms                                                                      | 284 ms: 1.00x faster                                                                  |
| scimark_monte_carlo      | 47.8 ms                                                                     | 48.0 ms: 1.00x slower                                                                 |
| logging_silent           | 56.1 ns                                                                     | 56.3 ns: 1.00x slower                                                                 |
| dulwich_log              | 43.5 ms                                                                     | 43.7 ms: 1.00x slower                                                                 |
| raytrace                 | 174 ms                                                                      | 176 ms: 1.01x slower                                                                  |
| xml_etree_iterparse      | 68.2 ms                                                                     | 68.9 ms: 1.01x slower                                                                 |
| telco                    | 4.67 ms                                                                     | 4.73 ms: 1.01x slower                                                                 |
| pidigits                 | 147 ms                                                                      | 149 ms: 1.01x slower                                                                  |
| python_startup           | 20.5 ms                                                                     | 20.8 ms: 1.01x slower                                                                 |
| async_generators         | 232 ms                                                                      | 236 ms: 1.01x slower                                                                  |
| go                       | 92.4 ms                                                                     | 93.7 ms: 1.02x slower                                                                 |
| pickle_pure_python       | 183 us                                                                      | 186 us: 1.02x slower                                                                  |
| unpickle_pure_python     | 137 us                                                                      | 139 us: 1.02x slower                                                                  |
| meteor_contest           | 75.3 ms                                                                     | 77.0 ms: 1.02x slower                                                                 |
| regex_effbot             | 1.56 ms                                                                     | 1.60 ms: 1.03x slower                                                                 |
| fannkuch                 | 264 ms                                                                      | 272 ms: 1.03x slower                                                                  |
| unpickle_list            | 2.65 us                                                                     | 2.73 us: 1.03x slower                                                                 |
| 2to3                     | 223 ms                                                                      | 229 ms: 1.03x slower                                                                  |
| coroutines               | 13.2 ms                                                                     | 13.6 ms: 1.03x slower                                                                 |
| pickle_list              | 2.89 us                                                                     | 2.98 us: 1.03x slower                                                                 |
| python_startup_no_site   | 18.3 ms                                                                     | 18.9 ms: 1.03x slower                                                                 |
| regex_dna                | 118 ms                                                                      | 122 ms: 1.04x slower                                                                  |
| bench_mp_pool            | 68.2 ms                                                                     | 70.8 ms: 1.04x slower                                                                 |
| deepcopy_memo            | 23.2 us                                                                     | 24.4 us: 1.05x slower                                                                 |
| scimark_lu               | 59.2 ms                                                                     | 62.6 ms: 1.06x slower                                                                 |
| regex_v8                 | 14.7 ms                                                                     | 15.7 ms: 1.07x slower                                                                 |
| Geometric mean           | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (36): json, pycparser, create_gc_cycles, tornado_http, unpickle, logging_simple, deepcopy, async_tree_cpu_io_mixed_tg, richards_super, xml_etree_process, mako, dask, sympy_integrate, sympy_str, sqlite_synth, sympy_sum, asyncio_tcp, async_tree_memoization_tg, async_tree_none_tg, pyflate, richards, pprint_pformat, mdp, deepcopy_reduce, json_loads, gc_traversal, async_tree_io_tg, async_tree_none, generators, regex_compile, coverage, pathlib, docutils, async_tree_io, float, bench_thread_pool


# HPT report

- Reliability score: 87.39% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown