# Results vs. base

- fork: brandtbucher
- ref: justin_mprotect
- machine: darwin-arm64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.00x slower \*
- HPT reliability: 94.81%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 189 ms                                                                 | 205 ms: 1.08x slower                                                    |
| chameleon      | 4.83 ms                                                                | 4.87 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                            |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_io, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_none_tg, async_tree_none, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 53.4 ms                                                                | 53.0 ms: 1.01x faster                                                   |
| pidigits       | 282 ms                                                                 | 283 ms: 1.01x slower                                                    |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_v8       | 17.2 ms                                                                | 17.3 ms: 1.01x slower                                                   |
| regex_effbot   | 2.62 ms                                                                | 2.65 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                            |

Benchmark hidden because not significant (2): regex_dna, regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| unpickle_list        | 3.11 us                                                                | 3.05 us: 1.02x faster                                                   |
| pickle_pure_python   | 197 us                                                                 | 196 us: 1.01x faster                                                    |
| json_dumps           | 6.47 ms                                                                | 6.49 ms: 1.00x slower                                                   |
| unpickle_pure_python | 151 us                                                                 | 151 us: 1.00x slower                                                    |
| pickle_dict          | 18.1 us                                                                | 18.2 us: 1.00x slower                                                   |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (9): xml_etree_generate, unpickle, xml_etree_iterparse, pickle_list, pickle, xml_etree_parse, json_loads, tomli_loads, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 18.7 ms                                                                | 17.9 ms: 1.05x faster                                                   |
| python_startup_no_site | 17.0 ms                                                                | 16.3 ms: 1.04x faster                                                   |
| Geometric mean         | (ref)                                                                  | 1.05x faster                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 6.82 ms                                                                | 6.80 ms: 1.00x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|--------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup           | 18.7 ms                                                                | 17.9 ms: 1.05x faster                                                   |
| python_startup_no_site   | 17.0 ms                                                                | 16.3 ms: 1.04x faster                                                   |
| fannkuch                 | 312 ms                                                                 | 305 ms: 1.02x faster                                                    |
| unpickle_list            | 3.11 us                                                                | 3.05 us: 1.02x faster                                                   |
| pycparser                | 735 ms                                                                 | 726 ms: 1.01x faster                                                    |
| logging_silent           | 73.0 ns                                                                | 72.2 ns: 1.01x faster                                                   |
| bench_thread_pool        | 516 us                                                                 | 511 us: 1.01x faster                                                    |
| typing_runtime_protocols | 72.1 us                                                                | 71.5 us: 1.01x faster                                                   |
| json                     | 2.98 ms                                                                | 2.96 ms: 1.01x faster                                                   |
| float                    | 53.4 ms                                                                | 53.0 ms: 1.01x faster                                                   |
| pickle_pure_python       | 197 us                                                                 | 196 us: 1.01x faster                                                    |
| coroutines               | 18.3 ms                                                                | 18.3 ms: 1.00x faster                                                   |
| async_generators         | 312 ms                                                                 | 310 ms: 1.00x faster                                                    |
| raytrace                 | 192 ms                                                                 | 191 ms: 1.00x faster                                                    |
| generators               | 28.4 ms                                                                | 28.3 ms: 1.00x faster                                                   |
| create_gc_cycles         | 714 us                                                                 | 712 us: 1.00x faster                                                    |
| mako                     | 6.82 ms                                                                | 6.80 ms: 1.00x faster                                                   |
| sympy_expand             | 245 ms                                                                 | 246 ms: 1.00x slower                                                    |
| deepcopy_memo            | 26.2 us                                                                | 26.3 us: 1.00x slower                                                   |
| asyncio_websockets       | 408 ms                                                                 | 409 ms: 1.00x slower                                                    |
| json_dumps               | 6.47 ms                                                                | 6.49 ms: 1.00x slower                                                   |
| scimark_fft              | 199 ms                                                                 | 200 ms: 1.00x slower                                                    |
| unpickle_pure_python     | 151 us                                                                 | 151 us: 1.00x slower                                                    |
| sympy_integrate          | 11.4 ms                                                                | 11.5 ms: 1.00x slower                                                   |
| pickle_dict              | 18.1 us                                                                | 18.2 us: 1.00x slower                                                   |
| sqlglot_parse            | 835 us                                                                 | 840 us: 1.01x slower                                                    |
| pidigits                 | 282 ms                                                                 | 283 ms: 1.01x slower                                                    |
| regex_v8                 | 17.2 ms                                                                | 17.3 ms: 1.01x slower                                                   |
| mdp                      | 1.62 sec                                                               | 1.63 sec: 1.01x slower                                                  |
| comprehensions           | 12.7 us                                                                | 12.8 us: 1.01x slower                                                   |
| sqlglot_optimize         | 35.4 ms                                                                | 35.6 ms: 1.01x slower                                                   |
| logging_format           | 3.77 us                                                                | 3.79 us: 1.01x slower                                                   |
| nqueens                  | 63.7 ms                                                                | 64.1 ms: 1.01x slower                                                   |
| logging_simple           | 3.47 us                                                                | 3.50 us: 1.01x slower                                                   |
| scimark_sor              | 112 ms                                                                 | 113 ms: 1.01x slower                                                    |
| scimark_monte_carlo      | 45.7 ms                                                                | 46.0 ms: 1.01x slower                                                   |
| scimark_sparse_mat_mult  | 3.14 ms                                                                | 3.17 ms: 1.01x slower                                                   |
| chameleon                | 4.83 ms                                                                | 4.87 ms: 1.01x slower                                                   |
| hexiom                   | 5.26 ms                                                                | 5.31 ms: 1.01x slower                                                   |
| deepcopy_reduce          | 1.98 us                                                                | 2.00 us: 1.01x slower                                                   |
| regex_effbot             | 2.62 ms                                                                | 2.65 ms: 1.01x slower                                                   |
| pathlib                  | 25.2 ms                                                                | 25.5 ms: 1.01x slower                                                   |
| pyflate                  | 344 ms                                                                 | 350 ms: 1.02x slower                                                    |
| telco                    | 4.46 ms                                                                | 4.60 ms: 1.03x slower                                                   |
| richards_super           | 42.7 ms                                                                | 44.2 ms: 1.04x slower                                                   |
| richards                 | 39.1 ms                                                                | 40.5 ms: 1.04x slower                                                   |
| spectral_norm            | 74.6 ms                                                                | 79.3 ms: 1.06x slower                                                   |
| 2to3                     | 189 ms                                                                 | 205 ms: 1.08x slower                                                    |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                            |

Benchmark hidden because not significant (45): bench_mp_pool, xml_etree_generate, unpickle, dask, meteor_contest, nbody, xml_etree_iterparse, pickle_list, sqlglot_normalize, deepcopy, pickle, xml_etree_parse, async_tree_cpu_io_mixed_tg, async_tree_io_tg, json_loads, regex_dna, async_tree_io, scimark_lu, sqlite_synth, sqlglot_transpile, go, chaos, async_tree_memoization, sympy_sum, docutils, gc_traversal, async_tree_cpu_io_mixed, deltablue, pprint_pformat, pprint_safe_repr, unpack_sequence, async_tree_none_tg, sympy_str, dulwich_log, async_tree_none, coverage, async_tree_memoization_tg, regex_compile, asyncio_tcp_ssl, tornado_http, tomli_loads, crypto_pyaes, xml_etree_process, asyncio_tcp, mypy2
Ignored benchmarks (8) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: aiohttp, django_template, genshi_text, genshi_xml, gunicorn, html5lib, pylint, thrift


# HPT report

- Reliability score: 94.81% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x