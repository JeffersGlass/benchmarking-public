# Results vs. base

- fork: brandtbucher
- ref: justin_cold
- machine: darwin-arm64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.00x faster
- HPT reliability: 96.66%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 174 ms                                                                 | 177 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (3): chameleon, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_io_tg, async_tree_none_tg, async_tree_none, async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 76.4 ms                                                                | 76.6 ms: 1.00x slower                                               |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (2): float, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_effbot   | 2.55 ms                                                                | 2.56 ms: 1.01x slower                                               |
| regex_compile  | 76.1 ms                                                                | 76.6 ms: 1.01x slower                                               |
| regex_dna      | 151 ms                                                                 | 153 ms: 1.01x slower                                                |
| regex_v8       | 17.1 ms                                                                | 17.2 ms: 1.01x slower                                               |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|---------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| unpickle            | 9.04 us                                                                | 8.99 us: 1.01x faster                                               |
| pickle_pure_python  | 195 us                                                                 | 196 us: 1.00x slower                                                |
| xml_etree_iterparse | 75.7 ms                                                                | 76.0 ms: 1.00x slower                                               |
| xml_etree_generate  | 56.1 ms                                                                | 56.9 ms: 1.01x slower                                               |
| pickle_list         | 2.96 us                                                                | 3.00 us: 1.01x slower                                               |
| Geometric mean      | (ref)                                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (9): unpickle_list, tomli_loads, json_dumps, unpickle_pure_python, json_loads, xml_etree_process, pickle, pickle_dict, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site | 10.4 ms                                                                | 10.2 ms: 1.03x faster                                               |
| python_startup         | 11.9 ms                                                                | 11.6 ms: 1.02x faster                                               |
| Geometric mean         | (ref)                                                                  | 1.02x faster                                                        |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                | bm-20240201-darwin-arm64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|--------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup_no_site   | 10.4 ms                                                                | 10.2 ms: 1.03x faster                                               |
| sqlite_synth             | 1.63 us                                                                | 1.60 us: 1.02x faster                                               |
| python_startup           | 11.9 ms                                                                | 11.6 ms: 1.02x faster                                               |
| hexiom                   | 5.06 ms                                                                | 4.98 ms: 1.02x faster                                               |
| coverage                 | 47.4 ms                                                                | 46.8 ms: 1.01x faster                                               |
| spectral_norm            | 82.0 ms                                                                | 81.1 ms: 1.01x faster                                               |
| go                       | 110 ms                                                                 | 109 ms: 1.01x faster                                                |
| create_gc_cycles         | 707 us                                                                 | 701 us: 1.01x faster                                                |
| json                     | 2.96 ms                                                                | 2.94 ms: 1.01x faster                                               |
| typing_runtime_protocols | 71.7 us                                                                | 71.2 us: 1.01x faster                                               |
| unpickle                 | 9.04 us                                                                | 8.99 us: 1.01x faster                                               |
| raytrace                 | 178 ms                                                                 | 177 ms: 1.00x faster                                                |
| sqlglot_optimize         | 34.8 ms                                                                | 34.7 ms: 1.00x faster                                               |
| sqlglot_normalize        | 185 ms                                                                 | 184 ms: 1.00x faster                                                |
| gc_traversal             | 2.39 ms                                                                | 2.39 ms: 1.00x faster                                               |
| meteor_contest           | 74.2 ms                                                                | 74.1 ms: 1.00x faster                                               |
| deltablue                | 2.51 ms                                                                | 2.51 ms: 1.00x faster                                               |
| logging_silent           | 70.4 ns                                                                | 70.3 ns: 1.00x faster                                               |
| scimark_sor              | 105 ms                                                                 | 105 ms: 1.00x slower                                                |
| chaos                    | 41.7 ms                                                                | 41.8 ms: 1.00x slower                                               |
| fannkuch                 | 277 ms                                                                 | 278 ms: 1.00x slower                                                |
| nbody                    | 76.4 ms                                                                | 76.6 ms: 1.00x slower                                               |
| pyflate                  | 327 ms                                                                 | 328 ms: 1.00x slower                                                |
| pickle_pure_python       | 195 us                                                                 | 196 us: 1.00x slower                                                |
| generators               | 28.3 ms                                                                | 28.4 ms: 1.00x slower                                               |
| comprehensions           | 12.7 us                                                                | 12.7 us: 1.00x slower                                               |
| deepcopy_memo            | 25.9 us                                                                | 26.0 us: 1.00x slower                                               |
| scimark_monte_carlo      | 49.1 ms                                                                | 49.3 ms: 1.00x slower                                               |
| xml_etree_iterparse      | 75.7 ms                                                                | 76.0 ms: 1.00x slower                                               |
| async_generators         | 303 ms                                                                 | 304 ms: 1.01x slower                                                |
| deepcopy                 | 226 us                                                                 | 227 us: 1.01x slower                                                |
| logging_simple           | 3.46 us                                                                | 3.48 us: 1.01x slower                                               |
| scimark_lu               | 74.8 ms                                                                | 75.2 ms: 1.01x slower                                               |
| sympy_integrate          | 11.2 ms                                                                | 11.3 ms: 1.01x slower                                               |
| regex_effbot             | 2.55 ms                                                                | 2.56 ms: 1.01x slower                                               |
| regex_compile            | 76.1 ms                                                                | 76.6 ms: 1.01x slower                                               |
| pprint_safe_repr         | 511 ms                                                                 | 515 ms: 1.01x slower                                                |
| pprint_pformat           | 1.05 sec                                                               | 1.05 sec: 1.01x slower                                              |
| dulwich_log              | 29.8 ms                                                                | 30.0 ms: 1.01x slower                                               |
| regex_dna                | 151 ms                                                                 | 153 ms: 1.01x slower                                                |
| sqlglot_transpile        | 977 us                                                                 | 985 us: 1.01x slower                                                |
| regex_v8                 | 17.1 ms                                                                | 17.2 ms: 1.01x slower                                               |
| sympy_sum                | 75.6 ms                                                                | 76.5 ms: 1.01x slower                                               |
| xml_etree_generate       | 56.1 ms                                                                | 56.9 ms: 1.01x slower                                               |
| pickle_list              | 2.96 us                                                                | 3.00 us: 1.01x slower                                               |
| 2to3                     | 174 ms                                                                 | 177 ms: 1.02x slower                                                |
| telco                    | 4.51 ms                                                                | 4.61 ms: 1.02x slower                                               |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (46): asyncio_tcp, pathlib, tornado_http, logging_format, dask, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, bench_thread_pool, scimark_sparse_mat_mult, chameleon, crypto_pyaes, unpickle_list, async_tree_io_tg, tomli_loads, float, sympy_expand, nqueens, sqlglot_parse, async_tree_none_tg, json_dumps, scimark_fft, unpickle_pure_python, async_tree_none, richards_super, async_tree_cpu_io_mixed, json_loads, mdp, xml_etree_process, pidigits, asyncio_websockets, pickle, pickle_dict, coroutines, richards, pycparser, async_tree_io, mako, docutils, deepcopy_reduce, mypy2, sympy_str, async_tree_memoization, unpack_sequence, asyncio_tcp_ssl, xml_etree_parse, bench_mp_pool


# HPT report

- Reliability score: 96.66% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.06x