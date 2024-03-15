# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.00x faster
- HPT reliability: 99.73%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.27x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240118-darwin-arm64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 173 ms                                                                 | 175 ms: 1.01x slower                                                             |
| chameleon      | 5.02 ms                                                                | 5.00 ms: 1.00x faster                                                            |
| docutils       | 1.51 sec                                                               | 1.50 sec: 1.01x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240118-darwin-arm64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg | 268 ms                                                                 | 266 ms: 1.01x faster                                                             |
| async_tree_io_tg   | 684 ms                                                                 | 688 ms: 1.01x slower                                                             |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (6): async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_io, async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240118-darwin-arm64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 68.8 ms                                                                | 68.0 ms: 1.01x faster                                                            |
| nbody          | 86.4 ms                                                                | 85.6 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240118-darwin-arm64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 2.79 ms                                                                | 2.75 ms: 1.02x faster                                                            |
| regex_v8       | 18.1 ms                                                                | 17.9 ms: 1.01x faster                                                            |
| regex_dna      | 157 ms                                                                 | 155 ms: 1.01x faster                                                             |
| regex_compile  | 82.2 ms                                                                | 81.8 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240118-darwin-arm64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_list          | 2.99 us                                                                | 2.93 us: 1.02x faster                                                            |
| tomli_loads          | 1.67 sec                                                               | 1.66 sec: 1.01x faster                                                           |
| unpickle             | 9.25 us                                                                | 9.17 us: 1.01x faster                                                            |
| unpickle_list        | 3.06 us                                                                | 3.04 us: 1.01x faster                                                            |
| xml_etree_process    | 41.0 ms                                                                | 40.7 ms: 1.01x faster                                                            |
| unpickle_pure_python | 164 us                                                                 | 164 us: 1.00x faster                                                             |
| xml_etree_generate   | 58.7 ms                                                                | 58.7 ms: 1.00x faster                                                            |
| pickle_pure_python   | 196 us                                                                 | 197 us: 1.00x slower                                                             |
| json_dumps           | 6.55 ms                                                                | 6.57 ms: 1.00x slower                                                            |
| pickle_dict          | 18.1 us                                                                | 18.2 us: 1.00x slower                                                            |
| json_loads           | 17.0 us                                                                | 17.2 us: 1.01x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (3): xml_etree_parse, xml_etree_iterparse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240118-darwin-arm64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup | 12.0 ms                                                                | 11.8 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240118-darwin-arm64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.69 ms                                                                | 9.56 ms: 1.01x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240118-darwin-arm64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| asyncio_tcp              | 429 ms                                                                 | 393 ms: 1.09x faster                                                             |
| spectral_norm            | 105 ms                                                                 | 100 ms: 1.05x faster                                                             |
| scimark_fft              | 248 ms                                                                 | 237 ms: 1.04x faster                                                             |
| asyncio_tcp_ssl          | 1.31 sec                                                               | 1.27 sec: 1.03x faster                                                           |
| fannkuch                 | 324 ms                                                                 | 317 ms: 1.02x faster                                                             |
| pickle_list              | 2.99 us                                                                | 2.93 us: 1.02x faster                                                            |
| pathlib                  | 25.4 ms                                                                | 24.9 ms: 1.02x faster                                                            |
| python_startup           | 12.0 ms                                                                | 11.8 ms: 1.02x faster                                                            |
| regex_effbot             | 2.79 ms                                                                | 2.75 ms: 1.02x faster                                                            |
| mako                     | 9.69 ms                                                                | 9.56 ms: 1.01x faster                                                            |
| crypto_pyaes             | 55.1 ms                                                                | 54.5 ms: 1.01x faster                                                            |
| float                    | 68.8 ms                                                                | 68.0 ms: 1.01x faster                                                            |
| logging_format           | 3.90 us                                                                | 3.86 us: 1.01x faster                                                            |
| nbody                    | 86.4 ms                                                                | 85.6 ms: 1.01x faster                                                            |
| regex_v8                 | 18.1 ms                                                                | 17.9 ms: 1.01x faster                                                            |
| docutils                 | 1.51 sec                                                               | 1.50 sec: 1.01x faster                                                           |
| nqueens                  | 68.2 ms                                                                | 67.6 ms: 1.01x faster                                                            |
| tomli_loads              | 1.67 sec                                                               | 1.66 sec: 1.01x faster                                                           |
| unpickle                 | 9.25 us                                                                | 9.17 us: 1.01x faster                                                            |
| unpickle_list            | 3.06 us                                                                | 3.04 us: 1.01x faster                                                            |
| logging_simple           | 3.59 us                                                                | 3.56 us: 1.01x faster                                                            |
| sqlglot_transpile        | 1.00 ms                                                                | 992 us: 1.01x faster                                                             |
| json                     | 2.99 ms                                                                | 2.96 ms: 1.01x faster                                                            |
| async_tree_none_tg       | 268 ms                                                                 | 266 ms: 1.01x faster                                                             |
| regex_dna                | 157 ms                                                                 | 155 ms: 1.01x faster                                                             |
| telco                    | 4.68 ms                                                                | 4.64 ms: 1.01x faster                                                            |
| xml_etree_process        | 41.0 ms                                                                | 40.7 ms: 1.01x faster                                                            |
| mdp                      | 1.62 sec                                                               | 1.61 sec: 1.01x faster                                                           |
| sympy_integrate          | 11.6 ms                                                                | 11.5 ms: 1.01x faster                                                            |
| regex_compile            | 82.2 ms                                                                | 81.8 ms: 1.01x faster                                                            |
| sqlglot_parse            | 814 us                                                                 | 810 us: 1.01x faster                                                             |
| sympy_str                | 149 ms                                                                 | 148 ms: 1.01x faster                                                             |
| unpickle_pure_python     | 164 us                                                                 | 164 us: 1.00x faster                                                             |
| chameleon                | 5.02 ms                                                                | 5.00 ms: 1.00x faster                                                            |
| deepcopy_reduce          | 1.99 us                                                                | 1.99 us: 1.00x faster                                                            |
| scimark_sor              | 106 ms                                                                 | 106 ms: 1.00x faster                                                             |
| pyflate                  | 371 ms                                                                 | 370 ms: 1.00x faster                                                             |
| raytrace                 | 186 ms                                                                 | 186 ms: 1.00x faster                                                             |
| deepcopy_memo            | 26.9 us                                                                | 26.8 us: 1.00x faster                                                            |
| asyncio_websockets       | 409 ms                                                                 | 408 ms: 1.00x faster                                                             |
| go                       | 111 ms                                                                 | 111 ms: 1.00x faster                                                             |
| scimark_monte_carlo      | 56.8 ms                                                                | 56.7 ms: 1.00x faster                                                            |
| richards                 | 32.7 ms                                                                | 32.6 ms: 1.00x faster                                                            |
| sqlglot_normalize        | 191 ms                                                                 | 190 ms: 1.00x faster                                                             |
| xml_etree_generate       | 58.7 ms                                                                | 58.7 ms: 1.00x faster                                                            |
| sympy_expand             | 245 ms                                                                 | 245 ms: 1.00x slower                                                             |
| dulwich_log              | 30.0 ms                                                                | 30.0 ms: 1.00x slower                                                            |
| pprint_pformat           | 1.18 sec                                                               | 1.18 sec: 1.00x slower                                                           |
| async_generators         | 299 ms                                                                 | 300 ms: 1.00x slower                                                             |
| pickle_pure_python       | 196 us                                                                 | 197 us: 1.00x slower                                                             |
| scimark_lu               | 76.5 ms                                                                | 76.7 ms: 1.00x slower                                                            |
| json_dumps               | 6.55 ms                                                                | 6.57 ms: 1.00x slower                                                            |
| meteor_contest           | 77.1 ms                                                                | 77.4 ms: 1.00x slower                                                            |
| pickle_dict              | 18.1 us                                                                | 18.2 us: 1.00x slower                                                            |
| scimark_sparse_mat_mult  | 4.08 ms                                                                | 4.11 ms: 1.01x slower                                                            |
| async_tree_io_tg         | 684 ms                                                                 | 688 ms: 1.01x slower                                                             |
| richards_super           | 36.5 ms                                                                | 36.7 ms: 1.01x slower                                                            |
| 2to3                     | 173 ms                                                                 | 175 ms: 1.01x slower                                                             |
| json_loads               | 17.0 us                                                                | 17.2 us: 1.01x slower                                                            |
| bench_thread_pool        | 514 us                                                                 | 519 us: 1.01x slower                                                             |
| typing_runtime_protocols | 73.5 us                                                                | 74.7 us: 1.02x slower                                                            |
| bench_mp_pool            | 44.3 ms                                                                | 45.4 ms: 1.02x slower                                                            |
| coverage                 | 48.0 ms                                                                | 50.0 ms: 1.04x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (30): python_startup_no_site, dask, xml_etree_parse, xml_etree_iterparse, pickle, chaos, deltablue, async_tree_cpu_io_mixed, deepcopy, gc_traversal, pidigits, hexiom, mypy2, unpack_sequence, async_tree_memoization_tg, create_gc_cycles, async_tree_io, generators, pprint_safe_repr, sqlite_synth, sqlglot_optimize, logging_silent, async_tree_none, coroutines, async_tree_memoization, async_tree_cpu_io_mixed_tg, comprehensions, sympy_sum, pycparser, tornado_http


# HPT report

- Reliability score: 99.73% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.27x