# Results vs. base

- fork: mdboom
- ref: aa_test
- machine: darwin-arm64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.00x slower
- HPT reliability: 99.61%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 173 ms                                                                 | 191 ms: 1.11x slower                                      |
| docutils       | 1.46 sec                                                               | 1.47 sec: 1.00x slower                                    |
| Geometric mean | (ref)                                                                  | 1.03x slower                                              |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none_tg | 258 ms                                                                 | 259 ms: 1.00x slower                                      |
| async_tree_io      | 695 ms                                                                 | 699 ms: 1.01x slower                                      |
| async_tree_io_tg   | 663 ms                                                                 | 667 ms: 1.01x slower                                      |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                              |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| pidigits       | 282 ms                                                                 | 282 ms: 1.00x slower                                      |
| nbody          | 75.8 ms                                                                | 76.0 ms: 1.00x slower                                     |
| Geometric mean | (ref)                                                                  | 1.00x slower                                              |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| regex_v8       | 17.1 ms                                                                | 16.9 ms: 1.01x faster                                     |
| regex_effbot   | 2.46 ms                                                                | 2.46 ms: 1.00x faster                                     |
| regex_compile  | 75.0 ms                                                                | 75.2 ms: 1.00x slower                                     |
| Geometric mean | (ref)                                                                  | 1.00x faster                                              |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| tomli_loads        | 1.42 sec                                                               | 1.41 sec: 1.01x faster                                    |
| pickle_list        | 3.00 us                                                                | 2.99 us: 1.00x faster                                     |
| pickle_pure_python | 196 us                                                                 | 195 us: 1.00x faster                                      |
| xml_etree_generate | 55.6 ms                                                                | 55.7 ms: 1.00x slower                                     |
| json_loads         | 16.9 us                                                                | 17.0 us: 1.01x slower                                     |
| pickle_dict        | 18.1 us                                                                | 18.2 us: 1.01x slower                                     |
| json_dumps         | 6.47 ms                                                                | 6.53 ms: 1.01x slower                                     |
| unpickle           | 9.14 us                                                                | 9.23 us: 1.01x slower                                     |
| xml_etree_process  | 38.9 ms                                                                | 39.3 ms: 1.01x slower                                     |
| unpickle_list      | 3.05 us                                                                | 3.10 us: 1.01x slower                                     |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                              |

Benchmark hidden because not significant (4): unpickle_pure_python, pickle, xml_etree_parse, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------:|
| fannkuch                 | 272 ms                                                                 | 266 ms: 1.02x faster                                      |
| coroutines               | 18.7 ms                                                                | 18.5 ms: 1.01x faster                                     |
| regex_v8                 | 17.1 ms                                                                | 16.9 ms: 1.01x faster                                     |
| tomli_loads              | 1.42 sec                                                               | 1.41 sec: 1.01x faster                                    |
| sympy_integrate          | 11.1 ms                                                                | 11.1 ms: 1.00x faster                                     |
| telco                    | 4.58 ms                                                                | 4.56 ms: 1.00x faster                                     |
| pickle_list              | 3.00 us                                                                | 2.99 us: 1.00x faster                                     |
| go                       | 110 ms                                                                 | 110 ms: 1.00x faster                                      |
| pickle_pure_python       | 196 us                                                                 | 195 us: 1.00x faster                                      |
| sqlglot_normalize        | 184 ms                                                                 | 183 ms: 1.00x faster                                      |
| sqlglot_optimize         | 34.6 ms                                                                | 34.5 ms: 1.00x faster                                     |
| hexiom                   | 4.92 ms                                                                | 4.91 ms: 1.00x faster                                     |
| regex_effbot             | 2.46 ms                                                                | 2.46 ms: 1.00x faster                                     |
| scimark_sor              | 105 ms                                                                 | 105 ms: 1.00x slower                                      |
| scimark_fft              | 213 ms                                                                 | 213 ms: 1.00x slower                                      |
| pidigits                 | 282 ms                                                                 | 282 ms: 1.00x slower                                      |
| regex_compile            | 75.0 ms                                                                | 75.2 ms: 1.00x slower                                     |
| richards                 | 31.9 ms                                                                | 32.0 ms: 1.00x slower                                     |
| mdp                      | 1.61 sec                                                               | 1.61 sec: 1.00x slower                                    |
| nbody                    | 75.8 ms                                                                | 76.0 ms: 1.00x slower                                     |
| docutils                 | 1.46 sec                                                               | 1.47 sec: 1.00x slower                                    |
| asyncio_websockets       | 408 ms                                                                 | 409 ms: 1.00x slower                                      |
| xml_etree_generate       | 55.6 ms                                                                | 55.7 ms: 1.00x slower                                     |
| scimark_lu               | 74.4 ms                                                                | 74.6 ms: 1.00x slower                                     |
| deepcopy_memo            | 26.2 us                                                                | 26.3 us: 1.00x slower                                     |
| comprehensions           | 12.6 us                                                                | 12.7 us: 1.00x slower                                     |
| deepcopy                 | 226 us                                                                 | 227 us: 1.00x slower                                      |
| deepcopy_reduce          | 1.98 us                                                                | 1.99 us: 1.00x slower                                     |
| async_tree_none_tg       | 258 ms                                                                 | 259 ms: 1.00x slower                                      |
| async_tree_io            | 695 ms                                                                 | 699 ms: 1.01x slower                                      |
| async_tree_io_tg         | 663 ms                                                                 | 667 ms: 1.01x slower                                      |
| logging_simple           | 3.45 us                                                                | 3.47 us: 1.01x slower                                     |
| pprint_pformat           | 1.04 sec                                                               | 1.05 sec: 1.01x slower                                    |
| pprint_safe_repr         | 509 ms                                                                 | 513 ms: 1.01x slower                                      |
| json_loads               | 16.9 us                                                                | 17.0 us: 1.01x slower                                     |
| pickle_dict              | 18.1 us                                                                | 18.2 us: 1.01x slower                                     |
| json_dumps               | 6.47 ms                                                                | 6.53 ms: 1.01x slower                                     |
| unpickle                 | 9.14 us                                                                | 9.23 us: 1.01x slower                                     |
| typing_runtime_protocols | 70.8 us                                                                | 71.5 us: 1.01x slower                                     |
| xml_etree_process        | 38.9 ms                                                                | 39.3 ms: 1.01x slower                                     |
| unpickle_list            | 3.05 us                                                                | 3.10 us: 1.01x slower                                     |
| pathlib                  | 23.9 ms                                                                | 24.3 ms: 1.02x slower                                     |
| 2to3                     | 173 ms                                                                 | 191 ms: 1.11x slower                                      |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                              |

Benchmark hidden because not significant (50): asyncio_tcp_ssl, coverage, bench_mp_pool, dask, logging_silent, richards_super, python_startup, bench_thread_pool, logging_format, crypto_pyaes, pyflate, sympy_expand, unpickle_pure_python, scimark_monte_carlo, generators, spectral_norm, meteor_contest, raytrace, mako, scimark_sparse_mat_mult, pickle, create_gc_cycles, gc_traversal, float, unpack_sequence, chameleon, sqlglot_transpile, dulwich_log, async_tree_cpu_io_mixed, regex_dna, async_generators, xml_etree_parse, async_tree_none, deltablue, sympy_str, nqueens, xml_etree_iterparse, tornado_http, sqlite_synth, chaos, sqlglot_parse, pycparser, sympy_sum, async_tree_cpu_io_mixed_tg, json, async_tree_memoization_tg, python_startup_no_site, async_tree_memoization, asyncio_tcp, mypy2


# HPT report

- Reliability score: 99.61% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x