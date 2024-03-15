# Results vs. base

- fork: brandtbucher
- ref: justin_arena
- machine: darwin-arm64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.00x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 189 ms                                                                 | 186 ms: 1.02x faster                                                 |
| chameleon      | 4.83 ms                                                                | 4.82 ms: 1.00x faster                                                |
| docutils       | 1.53 sec                                                               | 1.52 sec: 1.00x faster                                               |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (2): html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io    | 701 ms                                                                 | 697 ms: 1.01x faster                                                 |
| async_tree_io_tg | 668 ms                                                                 | 665 ms: 1.00x faster                                                 |
| Geometric mean   | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (6): async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 53.4 ms                                                                | 53.0 ms: 1.01x faster                                                |
| pidigits       | 282 ms                                                                 | 281 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 152 ms                                                                 | 152 ms: 1.00x faster                                                 |
| regex_effbot   | 2.62 ms                                                                | 2.63 ms: 1.00x slower                                                |
| regex_v8       | 17.2 ms                                                                | 17.2 ms: 1.00x slower                                                |
| regex_compile  | 86.4 ms                                                                | 87.8 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpickle             | 9.27 us                                                                | 9.10 us: 1.02x faster                                                |
| xml_etree_generate   | 56.4 ms                                                                | 55.4 ms: 1.02x faster                                                |
| pickle               | 7.34 us                                                                | 7.26 us: 1.01x faster                                                |
| unpickle_pure_python | 151 us                                                                 | 150 us: 1.00x faster                                                 |
| pickle_list          | 2.95 us                                                                | 2.96 us: 1.00x slower                                                |
| json_dumps           | 6.47 ms                                                                | 6.53 ms: 1.01x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (8): xml_etree_parse, pickle_pure_python, pickle_dict, json_loads, tomli_loads, xml_etree_iterparse, unpickle_list, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 17.0 ms                                                                | 16.4 ms: 1.04x faster                                                |
| python_startup         | 18.7 ms                                                                | 18.0 ms: 1.04x faster                                                |
| Geometric mean         | (ref)                                                                  | 1.04x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| genshi_text    | 15.8 ms                                                                | 15.9 ms: 1.01x slower                                                |
| genshi_xml     | 37.3 ms                                                                | 37.8 ms: 1.01x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (2): django_template, mako

All benchmarks:
===============

| Benchmark                | bm-20240305-darwin-arm64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-darwin-arm64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| richards                 | 39.1 ms                                                                | 37.0 ms: 1.06x faster                                                |
| richards_super           | 42.7 ms                                                                | 40.8 ms: 1.05x faster                                                |
| pycparser                | 735 ms                                                                 | 706 ms: 1.04x faster                                                 |
| python_startup_no_site   | 17.0 ms                                                                | 16.4 ms: 1.04x faster                                                |
| python_startup           | 18.7 ms                                                                | 18.0 ms: 1.04x faster                                                |
| go                       | 117 ms                                                                 | 114 ms: 1.02x faster                                                 |
| pprint_pformat           | 1.06 sec                                                               | 1.04 sec: 1.02x faster                                               |
| pprint_safe_repr         | 516 ms                                                                 | 507 ms: 1.02x faster                                                 |
| unpickle                 | 9.27 us                                                                | 9.10 us: 1.02x faster                                                |
| xml_etree_generate       | 56.4 ms                                                                | 55.4 ms: 1.02x faster                                                |
| 2to3                     | 189 ms                                                                 | 186 ms: 1.02x faster                                                 |
| thrift                   | 461 us                                                                 | 455 us: 1.01x faster                                                 |
| pickle                   | 7.34 us                                                                | 7.26 us: 1.01x faster                                                |
| deepcopy                 | 231 us                                                                 | 228 us: 1.01x faster                                                 |
| crypto_pyaes             | 47.7 ms                                                                | 47.2 ms: 1.01x faster                                                |
| chaos                    | 40.5 ms                                                                | 40.2 ms: 1.01x faster                                                |
| json                     | 2.98 ms                                                                | 2.95 ms: 1.01x faster                                                |
| scimark_lu               | 85.8 ms                                                                | 85.0 ms: 1.01x faster                                                |
| deltablue                | 2.54 ms                                                                | 2.52 ms: 1.01x faster                                                |
| typing_runtime_protocols | 72.1 us                                                                | 71.5 us: 1.01x faster                                                |
| sqlglot_normalize        | 184 ms                                                                 | 183 ms: 1.01x faster                                                 |
| logging_silent           | 73.0 ns                                                                | 72.5 ns: 1.01x faster                                                |
| async_tree_io            | 701 ms                                                                 | 697 ms: 1.01x faster                                                 |
| bench_thread_pool        | 516 us                                                                 | 512 us: 1.01x faster                                                 |
| float                    | 53.4 ms                                                                | 53.0 ms: 1.01x faster                                                |
| comprehensions           | 12.7 us                                                                | 12.7 us: 1.00x faster                                                |
| create_gc_cycles         | 714 us                                                                 | 711 us: 1.00x faster                                                 |
| docutils                 | 1.53 sec                                                               | 1.52 sec: 1.00x faster                                               |
| async_tree_io_tg         | 668 ms                                                                 | 665 ms: 1.00x faster                                                 |
| nqueens                  | 63.7 ms                                                                | 63.4 ms: 1.00x faster                                                |
| sympy_integrate          | 11.4 ms                                                                | 11.4 ms: 1.00x faster                                                |
| unpickle_pure_python     | 151 us                                                                 | 150 us: 1.00x faster                                                 |
| regex_dna                | 152 ms                                                                 | 152 ms: 1.00x faster                                                 |
| chameleon                | 4.83 ms                                                                | 4.82 ms: 1.00x faster                                                |
| pidigits                 | 282 ms                                                                 | 281 ms: 1.00x faster                                                 |
| regex_effbot             | 2.62 ms                                                                | 2.63 ms: 1.00x slower                                                |
| regex_v8                 | 17.2 ms                                                                | 17.2 ms: 1.00x slower                                                |
| logging_simple           | 3.47 us                                                                | 3.48 us: 1.00x slower                                                |
| pyflate                  | 344 ms                                                                 | 345 ms: 1.00x slower                                                 |
| fannkuch                 | 312 ms                                                                 | 313 ms: 1.00x slower                                                 |
| pickle_list              | 2.95 us                                                                | 2.96 us: 1.00x slower                                                |
| hexiom                   | 5.26 ms                                                                | 5.29 ms: 1.00x slower                                                |
| logging_format           | 3.77 us                                                                | 3.78 us: 1.00x slower                                                |
| genshi_text              | 15.8 ms                                                                | 15.9 ms: 1.01x slower                                                |
| scimark_sparse_mat_mult  | 3.14 ms                                                                | 3.17 ms: 1.01x slower                                                |
| scimark_monte_carlo      | 45.7 ms                                                                | 46.1 ms: 1.01x slower                                                |
| sqlglot_parse            | 835 us                                                                 | 843 us: 1.01x slower                                                 |
| json_dumps               | 6.47 ms                                                                | 6.53 ms: 1.01x slower                                                |
| sqlite_synth             | 1.58 us                                                                | 1.60 us: 1.01x slower                                                |
| genshi_xml               | 37.3 ms                                                                | 37.8 ms: 1.01x slower                                                |
| regex_compile            | 86.4 ms                                                                | 87.8 ms: 1.02x slower                                                |
| telco                    | 4.46 ms                                                                | 4.54 ms: 1.02x slower                                                |
| scimark_sor              | 112 ms                                                                 | 114 ms: 1.02x slower                                                 |
| spectral_norm            | 74.6 ms                                                                | 78.4 ms: 1.05x slower                                                |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (47): asyncio_tcp, pathlib, tornado_http, mypy2, unpack_sequence, bench_mp_pool, aiohttp, xml_etree_parse, pickle_pure_python, raytrace, async_generators, meteor_contest, deepcopy_reduce, async_tree_memoization, django_template, pickle_dict, sympy_str, async_tree_cpu_io_mixed_tg, sqlglot_optimize, async_tree_none_tg, gc_traversal, pylint, sympy_expand, coroutines, dask, async_tree_memoization_tg, nbody, generators, scimark_fft, deepcopy_memo, mako, asyncio_websockets, sympy_sum, asyncio_tcp_ssl, html5lib, mdp, coverage, dulwich_log, async_tree_cpu_io_mixed, sqlglot_transpile, json_loads, tomli_loads, async_tree_none, xml_etree_iterparse, unpickle_list, xml_etree_process, gunicorn


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x