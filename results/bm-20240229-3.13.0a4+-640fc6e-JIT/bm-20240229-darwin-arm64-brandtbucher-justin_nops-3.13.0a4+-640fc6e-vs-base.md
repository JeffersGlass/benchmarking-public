# Results vs. base

- fork: brandtbucher
- ref: justin_nops
- machine: darwin-arm64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.00x slower
- HPT reliability: 82.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 189 ms                                                                 | 188 ms: 1.01x faster                                                |
| chameleon      | 4.83 ms                                                                | 4.82 ms: 1.00x faster                                               |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (3): docutils, html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_io, async_tree_cpu_io_mixed, async_tree_none_tg, async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| float          | 53.4 ms                                                                | 53.1 ms: 1.01x faster                                               |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (2): pidigits, nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_v8       | 17.2 ms                                                                | 17.2 ms: 1.00x slower                                               |
| regex_compile  | 86.4 ms                                                                | 86.8 ms: 1.00x slower                                               |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (2): regex_dna, regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| unpickle             | 9.27 us                                                                | 9.13 us: 1.02x faster                                               |
| unpickle_list        | 3.11 us                                                                | 3.07 us: 1.01x faster                                               |
| pickle               | 7.34 us                                                                | 7.29 us: 1.01x faster                                               |
| pickle_list          | 2.95 us                                                                | 2.93 us: 1.01x faster                                               |
| pickle_pure_python   | 197 us                                                                 | 196 us: 1.00x faster                                                |
| pickle_dict          | 18.1 us                                                                | 18.2 us: 1.00x slower                                               |
| json_dumps           | 6.47 ms                                                                | 6.50 ms: 1.01x slower                                               |
| unpickle_pure_python | 151 us                                                                 | 155 us: 1.03x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (6): xml_etree_generate, tomli_loads, xml_etree_parse, json_loads, xml_etree_iterparse, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup | 18.7 ms                                                                | 18.4 ms: 1.02x faster                                               |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                        |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| genshi_text    | 15.8 ms                                                                | 15.7 ms: 1.01x faster                                               |
| genshi_xml     | 37.3 ms                                                                | 37.1 ms: 1.00x faster                                               |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (2): django_template, mako

All benchmarks:
===============

| Benchmark                | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup           | 18.7 ms                                                                | 18.4 ms: 1.02x faster                                               |
| thrift                   | 461 us                                                                 | 454 us: 1.02x faster                                                |
| unpickle                 | 9.27 us                                                                | 9.13 us: 1.02x faster                                               |
| unpickle_list            | 3.11 us                                                                | 3.07 us: 1.01x faster                                               |
| pycparser                | 735 ms                                                                 | 727 ms: 1.01x faster                                                |
| json                     | 2.98 ms                                                                | 2.95 ms: 1.01x faster                                               |
| typing_runtime_protocols | 72.1 us                                                                | 71.3 us: 1.01x faster                                               |
| coroutines               | 18.3 ms                                                                | 18.1 ms: 1.01x faster                                               |
| deepcopy                 | 231 us                                                                 | 228 us: 1.01x faster                                                |
| genshi_text              | 15.8 ms                                                                | 15.7 ms: 1.01x faster                                               |
| 2to3                     | 189 ms                                                                 | 188 ms: 1.01x faster                                                |
| pickle                   | 7.34 us                                                                | 7.29 us: 1.01x faster                                               |
| pickle_list              | 2.95 us                                                                | 2.93 us: 1.01x faster                                               |
| float                    | 53.4 ms                                                                | 53.1 ms: 1.01x faster                                               |
| pickle_pure_python       | 197 us                                                                 | 196 us: 1.00x faster                                                |
| genshi_xml               | 37.3 ms                                                                | 37.1 ms: 1.00x faster                                               |
| coverage                 | 47.5 ms                                                                | 47.2 ms: 1.00x faster                                               |
| deepcopy_memo            | 26.2 us                                                                | 26.1 us: 1.00x faster                                               |
| deltablue                | 2.54 ms                                                                | 2.54 ms: 1.00x faster                                               |
| generators               | 28.4 ms                                                                | 28.4 ms: 1.00x faster                                               |
| chameleon                | 4.83 ms                                                                | 4.82 ms: 1.00x faster                                               |
| regex_v8                 | 17.2 ms                                                                | 17.2 ms: 1.00x slower                                               |
| deepcopy_reduce          | 1.98 us                                                                | 1.98 us: 1.00x slower                                               |
| scimark_fft              | 199 ms                                                                 | 200 ms: 1.00x slower                                                |
| pickle_dict              | 18.1 us                                                                | 18.2 us: 1.00x slower                                               |
| sqlite_synth             | 1.58 us                                                                | 1.59 us: 1.00x slower                                               |
| logging_simple           | 3.47 us                                                                | 3.49 us: 1.00x slower                                               |
| mdp                      | 1.62 sec                                                               | 1.63 sec: 1.00x slower                                              |
| regex_compile            | 86.4 ms                                                                | 86.8 ms: 1.00x slower                                               |
| dulwich_log              | 30.8 ms                                                                | 31.0 ms: 1.00x slower                                               |
| json_dumps               | 6.47 ms                                                                | 6.50 ms: 1.01x slower                                               |
| pyflate                  | 344 ms                                                                 | 346 ms: 1.01x slower                                                |
| sympy_str                | 144 ms                                                                 | 145 ms: 1.01x slower                                                |
| sympy_expand             | 245 ms                                                                 | 247 ms: 1.01x slower                                                |
| nqueens                  | 63.7 ms                                                                | 64.1 ms: 1.01x slower                                               |
| richards                 | 39.1 ms                                                                | 39.3 ms: 1.01x slower                                               |
| sympy_integrate          | 11.4 ms                                                                | 11.5 ms: 1.01x slower                                               |
| scimark_monte_carlo      | 45.7 ms                                                                | 46.0 ms: 1.01x slower                                               |
| sympy_sum                | 76.3 ms                                                                | 76.9 ms: 1.01x slower                                               |
| logging_format           | 3.77 us                                                                | 3.80 us: 1.01x slower                                               |
| hexiom                   | 5.26 ms                                                                | 5.32 ms: 1.01x slower                                               |
| comprehensions           | 12.7 us                                                                | 13.0 us: 1.02x slower                                               |
| richards_super           | 42.7 ms                                                                | 43.5 ms: 1.02x slower                                               |
| unpickle_pure_python     | 151 us                                                                 | 155 us: 1.03x slower                                                |
| fannkuch                 | 312 ms                                                                 | 323 ms: 1.04x slower                                                |
| spectral_norm            | 74.6 ms                                                                | 81.6 ms: 1.09x slower                                               |
| Geometric mean           | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (55): gunicorn, python_startup_no_site, xml_etree_generate, bench_mp_pool, asyncio_tcp, meteor_contest, tomli_loads, bench_thread_pool, raytrace, xml_etree_parse, logging_silent, mypy2, sqlglot_normalize, json_loads, async_tree_cpu_io_mixed_tg, pprint_safe_repr, docutils, go, async_tree_io_tg, xml_etree_iterparse, sqlglot_parse, chaos, dask, scimark_lu, async_generators, pprint_pformat, gc_traversal, django_template, async_tree_memoization_tg, mako, async_tree_io, async_tree_cpu_io_mixed, html5lib, regex_dna, pidigits, regex_effbot, asyncio_websockets, async_tree_none_tg, aiohttp, scimark_sparse_mat_mult, crypto_pyaes, pylint, async_tree_none, asyncio_tcp_ssl, telco, tornado_http, create_gc_cycles, sqlglot_transpile, async_tree_memoization, unpack_sequence, sqlglot_optimize, pathlib, scimark_sor, nbody, xml_etree_process


# HPT report

- Reliability score: 82.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x