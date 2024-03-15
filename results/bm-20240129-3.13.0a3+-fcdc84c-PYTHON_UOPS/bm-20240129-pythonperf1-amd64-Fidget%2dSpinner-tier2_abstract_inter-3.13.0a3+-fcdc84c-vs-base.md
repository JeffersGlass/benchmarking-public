# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.00x faster
- HPT reliability: 93.41%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 223 ms                                                                      | 224 ms: 1.01x slower                                                                  |
| chameleon      | 5.12 ms                                                                     | 5.05 ms: 1.01x faster                                                                 |
| docutils       | 1.62 sec                                                                    | 1.61 sec: 1.01x faster                                                                |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_io_tg           | 783 ms                                                                      | 770 ms: 1.02x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 489 ms                                                                      | 481 ms: 1.02x faster                                                                  |
| async_tree_none_tg         | 288 ms                                                                      | 284 ms: 1.01x faster                                                                  |
| async_tree_memoization     | 349 ms                                                                      | 355 ms: 1.02x slower                                                                  |
| async_tree_io              | 742 ms                                                                      | 756 ms: 1.02x slower                                                                  |
| Geometric mean             | (ref)                                                                       | 1.00x slower                                                                          |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| nbody          | 78.4 ms                                                                     | 76.8 ms: 1.02x faster                                                                 |
| pidigits       | 147 ms                                                                      | 148 ms: 1.00x slower                                                                  |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_effbot   | 1.56 ms                                                                     | 1.61 ms: 1.03x slower                                                                 |
| regex_dna      | 118 ms                                                                      | 123 ms: 1.04x slower                                                                  |
| regex_v8       | 14.7 ms                                                                     | 15.7 ms: 1.07x slower                                                                 |
| Geometric mean | (ref)                                                                       | 1.04x slower                                                                          |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| xml_etree_parse      | 95.2 ms                                                                     | 94.1 ms: 1.01x faster                                                                 |
| xml_etree_process    | 38.2 ms                                                                     | 37.8 ms: 1.01x faster                                                                 |
| pickle_pure_python   | 183 us                                                                      | 181 us: 1.01x faster                                                                  |
| unpickle_pure_python | 137 us                                                                      | 135 us: 1.01x faster                                                                  |
| xml_etree_generate   | 56.0 ms                                                                     | 55.6 ms: 1.01x faster                                                                 |
| json_loads           | 13.8 us                                                                     | 13.7 us: 1.01x faster                                                                 |
| pickle_dict          | 18.7 us                                                                     | 18.8 us: 1.00x slower                                                                 |
| pickle               | 7.30 us                                                                     | 7.37 us: 1.01x slower                                                                 |
| json_dumps           | 5.70 ms                                                                     | 5.76 ms: 1.01x slower                                                                 |
| unpickle             | 8.35 us                                                                     | 8.48 us: 1.02x slower                                                                 |
| pickle_list          | 2.89 us                                                                     | 2.99 us: 1.03x slower                                                                 |
| unpickle_list        | 2.65 us                                                                     | 2.78 us: 1.05x slower                                                                 |
| Geometric mean       | (ref)                                                                       | 1.01x slower                                                                          |

Benchmark hidden because not significant (2): xml_etree_iterparse, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 20.5 ms                                                                     | 20.8 ms: 1.02x slower                                                                 |
| python_startup_no_site | 18.3 ms                                                                     | 18.8 ms: 1.03x slower                                                                 |
| Geometric mean         | (ref)                                                                       | 1.02x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.24 ms                                                                     | 7.53 ms: 1.04x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| asyncio_tcp_ssl            | 1.90 sec                                                                    | 1.52 sec: 1.25x faster                                                                |
| scimark_sor                | 84.4 ms                                                                     | 79.0 ms: 1.07x faster                                                                 |
| scimark_fft                | 207 ms                                                                      | 195 ms: 1.06x faster                                                                  |
| pycparser                  | 721 ms                                                                      | 687 ms: 1.05x faster                                                                  |
| sqlglot_parse              | 810 us                                                                      | 787 us: 1.03x faster                                                                  |
| generators                 | 22.6 ms                                                                     | 22.0 ms: 1.03x faster                                                                 |
| chaos                      | 44.1 ms                                                                     | 43.1 ms: 1.02x faster                                                                 |
| unpack_sequence            | 39.9 ns                                                                     | 39.0 ns: 1.02x faster                                                                 |
| scimark_lu                 | 59.2 ms                                                                     | 57.9 ms: 1.02x faster                                                                 |
| nbody                      | 78.4 ms                                                                     | 76.8 ms: 1.02x faster                                                                 |
| scimark_monte_carlo        | 47.8 ms                                                                     | 47.0 ms: 1.02x faster                                                                 |
| async_generators           | 232 ms                                                                      | 228 ms: 1.02x faster                                                                  |
| logging_silent             | 56.1 ns                                                                     | 55.2 ns: 1.02x faster                                                                 |
| async_tree_io_tg           | 783 ms                                                                      | 770 ms: 1.02x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 489 ms                                                                      | 481 ms: 1.02x faster                                                                  |
| coroutines                 | 13.2 ms                                                                     | 13.0 ms: 1.02x faster                                                                 |
| create_gc_cycles           | 748 us                                                                      | 737 us: 1.01x faster                                                                  |
| async_tree_none_tg         | 288 ms                                                                      | 284 ms: 1.01x faster                                                                  |
| gc_traversal               | 1.54 ms                                                                     | 1.52 ms: 1.01x faster                                                                 |
| chameleon                  | 5.12 ms                                                                     | 5.05 ms: 1.01x faster                                                                 |
| richards_super             | 31.0 ms                                                                     | 30.6 ms: 1.01x faster                                                                 |
| spectral_norm              | 81.0 ms                                                                     | 80.1 ms: 1.01x faster                                                                 |
| xml_etree_parse            | 95.2 ms                                                                     | 94.1 ms: 1.01x faster                                                                 |
| deltablue                  | 2.68 ms                                                                     | 2.65 ms: 1.01x faster                                                                 |
| pyflate                    | 326 ms                                                                      | 322 ms: 1.01x faster                                                                  |
| richards                   | 27.6 ms                                                                     | 27.3 ms: 1.01x faster                                                                 |
| xml_etree_process          | 38.2 ms                                                                     | 37.8 ms: 1.01x faster                                                                 |
| pickle_pure_python         | 183 us                                                                      | 181 us: 1.01x faster                                                                  |
| deepcopy                   | 228 us                                                                      | 226 us: 1.01x faster                                                                  |
| unpickle_pure_python       | 137 us                                                                      | 135 us: 1.01x faster                                                                  |
| crypto_pyaes               | 48.6 ms                                                                     | 48.1 ms: 1.01x faster                                                                 |
| comprehensions             | 13.0 us                                                                     | 12.8 us: 1.01x faster                                                                 |
| sympy_str                  | 167 ms                                                                      | 166 ms: 1.01x faster                                                                  |
| dulwich_log                | 43.5 ms                                                                     | 43.2 ms: 1.01x faster                                                                 |
| xml_etree_generate         | 56.0 ms                                                                     | 55.6 ms: 1.01x faster                                                                 |
| telco                      | 4.67 ms                                                                     | 4.64 ms: 1.01x faster                                                                 |
| deepcopy_reduce            | 2.01 us                                                                     | 2.00 us: 1.01x faster                                                                 |
| sqlglot_transpile          | 1.02 ms                                                                     | 1.02 ms: 1.01x faster                                                                 |
| pprint_pformat             | 1.08 sec                                                                    | 1.07 sec: 1.01x faster                                                                |
| docutils                   | 1.62 sec                                                                    | 1.61 sec: 1.01x faster                                                                |
| json_loads                 | 13.8 us                                                                     | 13.7 us: 1.01x faster                                                                 |
| sympy_expand               | 285 ms                                                                      | 284 ms: 1.00x faster                                                                  |
| mdp                        | 1.44 sec                                                                    | 1.43 sec: 1.00x faster                                                                |
| nqueens                    | 64.9 ms                                                                     | 64.7 ms: 1.00x faster                                                                 |
| pidigits                   | 147 ms                                                                      | 148 ms: 1.00x slower                                                                  |
| pickle_dict                | 18.7 us                                                                     | 18.8 us: 1.00x slower                                                                 |
| go                         | 92.4 ms                                                                     | 93.0 ms: 1.01x slower                                                                 |
| 2to3                       | 223 ms                                                                      | 224 ms: 1.01x slower                                                                  |
| pathlib                    | 80.5 ms                                                                     | 81.1 ms: 1.01x slower                                                                 |
| mypy2                      | 434 ms                                                                      | 437 ms: 1.01x slower                                                                  |
| sqlite_synth               | 1.58 us                                                                     | 1.59 us: 1.01x slower                                                                 |
| pickle                     | 7.30 us                                                                     | 7.37 us: 1.01x slower                                                                 |
| hexiom                     | 4.85 ms                                                                     | 4.90 ms: 1.01x slower                                                                 |
| json_dumps                 | 5.70 ms                                                                     | 5.76 ms: 1.01x slower                                                                 |
| bench_mp_pool              | 68.2 ms                                                                     | 69.2 ms: 1.01x slower                                                                 |
| meteor_contest             | 75.3 ms                                                                     | 76.5 ms: 1.01x slower                                                                 |
| unpickle                   | 8.35 us                                                                     | 8.48 us: 1.02x slower                                                                 |
| python_startup             | 20.5 ms                                                                     | 20.8 ms: 1.02x slower                                                                 |
| sqlglot_normalize          | 183 ms                                                                      | 186 ms: 1.02x slower                                                                  |
| async_tree_memoization     | 349 ms                                                                      | 355 ms: 1.02x slower                                                                  |
| async_tree_io              | 742 ms                                                                      | 756 ms: 1.02x slower                                                                  |
| fannkuch                   | 264 ms                                                                      | 269 ms: 1.02x slower                                                                  |
| deepcopy_memo              | 23.2 us                                                                     | 23.7 us: 1.02x slower                                                                 |
| python_startup_no_site     | 18.3 ms                                                                     | 18.8 ms: 1.03x slower                                                                 |
| regex_effbot               | 1.56 ms                                                                     | 1.61 ms: 1.03x slower                                                                 |
| pickle_list                | 2.89 us                                                                     | 2.99 us: 1.03x slower                                                                 |
| mako                       | 7.24 ms                                                                     | 7.53 ms: 1.04x slower                                                                 |
| regex_dna                  | 118 ms                                                                      | 123 ms: 1.04x slower                                                                  |
| unpickle_list              | 2.65 us                                                                     | 2.78 us: 1.05x slower                                                                 |
| regex_v8                   | 14.7 ms                                                                     | 15.7 ms: 1.07x slower                                                                 |
| Geometric mean             | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (22): json, scimark_sparse_mat_mult, typing_runtime_protocols, pprint_safe_repr, logging_format, bench_thread_pool, raytrace, tornado_http, sympy_sum, sympy_integrate, async_tree_memoization_tg, coverage, regex_compile, async_tree_cpu_io_mixed, logging_simple, sqlglot_optimize, xml_etree_iterparse, tomli_loads, float, dask, asyncio_tcp, async_tree_none


# HPT report

- Reliability score: 93.41% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown