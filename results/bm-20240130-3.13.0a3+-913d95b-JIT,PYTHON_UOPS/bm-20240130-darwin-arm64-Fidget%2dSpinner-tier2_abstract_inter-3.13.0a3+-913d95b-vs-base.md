# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.00x slower
- HPT reliability: 76.26%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 173 ms                                                                 | 175 ms: 1.01x slower                                                             |
| chameleon      | 4.91 ms                                                                | 4.89 ms: 1.00x faster                                                            |
| docutils       | 1.47 sec                                                               | 1.48 sec: 1.00x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_none_tg, async_tree_io, async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 76.7 ms                                                                | 74.8 ms: 1.03x faster                                                            |
| pidigits       | 282 ms                                                                 | 283 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 76.5 ms                                                                | 76.2 ms: 1.00x faster                                                            |
| regex_v8       | 17.2 ms                                                                | 17.2 ms: 1.00x faster                                                            |
| regex_effbot   | 2.55 ms                                                                | 2.57 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 3.12 us                                                                | 3.09 us: 1.01x faster                                                            |
| pickle_pure_python   | 198 us                                                                 | 197 us: 1.01x faster                                                             |
| xml_etree_generate   | 56.0 ms                                                                | 55.7 ms: 1.01x faster                                                            |
| json_loads           | 17.0 us                                                                | 17.1 us: 1.01x slower                                                            |
| unpickle_pure_python | 159 us                                                                 | 160 us: 1.01x slower                                                             |
| json_dumps           | 6.53 ms                                                                | 6.58 ms: 1.01x slower                                                            |
| pickle               | 7.29 us                                                                | 7.36 us: 1.01x slower                                                            |
| pickle_dict          | 18.0 us                                                                | 18.2 us: 1.01x slower                                                            |
| pickle_list          | 2.95 us                                                                | 2.99 us: 1.01x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (5): xml_etree_process, unpickle, xml_etree_parse, tomli_loads, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup | 13.2 ms                                                                | 13.1 ms: 1.00x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20240129-darwin-arm64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mdp                      | 1.69 sec                                                               | 1.63 sec: 1.04x faster                                                           |
| nbody                    | 76.7 ms                                                                | 74.8 ms: 1.03x faster                                                            |
| spectral_norm            | 82.6 ms                                                                | 80.7 ms: 1.02x faster                                                            |
| scimark_fft              | 218 ms                                                                 | 215 ms: 1.02x faster                                                             |
| sqlite_synth             | 1.62 us                                                                | 1.59 us: 1.02x faster                                                            |
| unpickle_list            | 3.12 us                                                                | 3.09 us: 1.01x faster                                                            |
| typing_runtime_protocols | 72.6 us                                                                | 72.0 us: 1.01x faster                                                            |
| scimark_sparse_mat_mult  | 3.34 ms                                                                | 3.32 ms: 1.01x faster                                                            |
| pickle_pure_python       | 198 us                                                                 | 197 us: 1.01x faster                                                             |
| logging_silent           | 70.4 ns                                                                | 70.0 ns: 1.01x faster                                                            |
| xml_etree_generate       | 56.0 ms                                                                | 55.7 ms: 1.01x faster                                                            |
| chameleon                | 4.91 ms                                                                | 4.89 ms: 1.00x faster                                                            |
| regex_compile            | 76.5 ms                                                                | 76.2 ms: 1.00x faster                                                            |
| go                       | 110 ms                                                                 | 110 ms: 1.00x faster                                                             |
| comprehensions           | 12.8 us                                                                | 12.7 us: 1.00x faster                                                            |
| python_startup           | 13.2 ms                                                                | 13.1 ms: 1.00x faster                                                            |
| coroutines               | 19.3 ms                                                                | 19.3 ms: 1.00x faster                                                            |
| logging_simple           | 3.50 us                                                                | 3.49 us: 1.00x faster                                                            |
| regex_v8                 | 17.2 ms                                                                | 17.2 ms: 1.00x faster                                                            |
| sqlglot_normalize        | 185 ms                                                                 | 185 ms: 1.00x faster                                                             |
| asyncio_websockets       | 409 ms                                                                 | 409 ms: 1.00x slower                                                             |
| docutils                 | 1.47 sec                                                               | 1.48 sec: 1.00x slower                                                           |
| gc_traversal             | 2.40 ms                                                                | 2.41 ms: 1.00x slower                                                            |
| deepcopy                 | 225 us                                                                 | 226 us: 1.00x slower                                                             |
| pyflate                  | 327 ms                                                                 | 328 ms: 1.00x slower                                                             |
| sqlglot_optimize         | 34.8 ms                                                                | 34.9 ms: 1.00x slower                                                            |
| pidigits                 | 282 ms                                                                 | 283 ms: 1.00x slower                                                             |
| logging_format           | 3.79 us                                                                | 3.80 us: 1.00x slower                                                            |
| deepcopy_memo            | 25.8 us                                                                | 25.9 us: 1.00x slower                                                            |
| json_loads               | 17.0 us                                                                | 17.1 us: 1.01x slower                                                            |
| deltablue                | 2.51 ms                                                                | 2.52 ms: 1.01x slower                                                            |
| unpickle_pure_python     | 159 us                                                                 | 160 us: 1.01x slower                                                             |
| json                     | 2.95 ms                                                                | 2.97 ms: 1.01x slower                                                            |
| regex_effbot             | 2.55 ms                                                                | 2.57 ms: 1.01x slower                                                            |
| telco                    | 4.55 ms                                                                | 4.59 ms: 1.01x slower                                                            |
| json_dumps               | 6.53 ms                                                                | 6.58 ms: 1.01x slower                                                            |
| pickle                   | 7.29 us                                                                | 7.36 us: 1.01x slower                                                            |
| pickle_dict              | 18.0 us                                                                | 18.2 us: 1.01x slower                                                            |
| pprint_pformat           | 1.06 sec                                                               | 1.07 sec: 1.01x slower                                                           |
| 2to3                     | 173 ms                                                                 | 175 ms: 1.01x slower                                                             |
| pprint_safe_repr         | 519 ms                                                                 | 526 ms: 1.01x slower                                                             |
| hexiom                   | 5.07 ms                                                                | 5.14 ms: 1.01x slower                                                            |
| pickle_list              | 2.95 us                                                                | 2.99 us: 1.01x slower                                                            |
| scimark_sor              | 106 ms                                                                 | 107 ms: 1.01x slower                                                             |
| coverage                 | 46.9 ms                                                                | 48.0 ms: 1.02x slower                                                            |
| fannkuch                 | 270 ms                                                                 | 295 ms: 1.09x slower                                                             |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (47): unpack_sequence, float, crypto_pyaes, async_tree_none_tg, async_generators, raytrace, async_tree_io, asyncio_tcp_ssl, async_tree_cpu_io_mixed, generators, xml_etree_process, sympy_expand, scimark_lu, async_tree_none, unpickle, async_tree_memoization_tg, richards, nqueens, async_tree_cpu_io_mixed_tg, python_startup_no_site, create_gc_cycles, regex_dna, dulwich_log, sympy_integrate, sympy_str, richards_super, async_tree_memoization, pycparser, chaos, sqlglot_transpile, xml_etree_parse, pathlib, meteor_contest, dask, scimark_monte_carlo, mako, bench_thread_pool, sqlglot_parse, sympy_sum, deepcopy_reduce, mypy2, tomli_loads, xml_etree_iterparse, async_tree_io_tg, asyncio_tcp, bench_mp_pool, tornado_http


# HPT report

- Reliability score: 76.26% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x