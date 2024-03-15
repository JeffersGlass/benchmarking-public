
# Results vs. 3.11.0

- fork: mdboom
- ref: compact_long
- machine: darwin-arm64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.07x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 178 ms: 1.15x slower                                           |
| chameleon      | 4.30 ms                                                | 5.16 ms: 1.20x slower                                          |
| docutils       | 1.43 sec                                               | 1.51 sec: 1.06x slower                                         |
| Geometric mean | (ref)                                                  | 1.11x slower                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none           | 282 ms                                                 | 258 ms: 1.09x faster                                           |
| async_tree_io_tg          | 724 ms                                                 | 695 ms: 1.04x faster                                           |
| async_tree_memoization_tg | 352 ms                                                 | 339 ms: 1.04x faster                                           |
| async_tree_none_tg        | 276 ms                                                 | 270 ms: 1.02x faster                                           |
| async_tree_io             | 697 ms                                                 | 713 ms: 1.02x slower                                           |
| async_tree_cpu_io_mixed   | 519 ms                                                 | 534 ms: 1.03x slower                                           |
| Geometric mean            | (ref)                                                  | 1.02x faster                                                   |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 274 ms: 1.03x faster                                           |
| float          | 50.8 ms                                                | 58.5 ms: 1.15x slower                                          |
| nbody          | 61.7 ms                                                | 81.7 ms: 1.32x slower                                          |
| Geometric mean | (ref)                                                  | 1.14x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 149 ms: 1.00x slower                                           |
| regex_effbot   | 2.43 ms                                                | 2.57 ms: 1.06x slower                                          |
| regex_compile  | 72.8 ms                                                | 80.5 ms: 1.10x slower                                          |
| regex_v8       | 15.1 ms                                                | 16.9 ms: 1.12x slower                                          |
| Geometric mean | (ref)                                                  | 1.07x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.72 ms: 1.12x faster                                          |
| pickle               | 6.98 us                                                | 7.36 us: 1.06x slower                                          |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                          |
| pickle_list          | 2.70 us                                                | 2.92 us: 1.08x slower                                          |
| xml_etree_parse      | 100 ms                                                 | 109 ms: 1.09x slower                                           |
| pickle_pure_python   | 191 us                                                 | 208 us: 1.09x slower                                           |
| unpickle             | 8.29 us                                                | 9.13 us: 1.10x slower                                          |
| unpickle_pure_python | 149 us                                                 | 166 us: 1.12x slower                                           |
| xml_etree_iterparse  | 68.3 ms                                                | 77.1 ms: 1.13x slower                                          |
| json_loads           | 15.3 us                                                | 17.4 us: 1.13x slower                                          |
| unpickle_list        | 2.69 us                                                | 3.12 us: 1.16x slower                                          |
| xml_etree_process    | 33.6 ms                                                | 42.0 ms: 1.25x slower                                          |
| tomli_loads          | 1.27 sec                                               | 1.60 sec: 1.26x slower                                         |
| xml_etree_generate   | 45.8 ms                                                | 60.9 ms: 1.33x slower                                          |
| Geometric mean       | (ref)                                                  | 1.12x slower                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.3 ms: 1.23x slower                                          |
| python_startup_no_site | 8.57 ms                                                | 11.9 ms: 1.39x slower                                          |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 7.90 ms: 1.00x faster                                          |

All benchmarks:
===============

| Benchmark                 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols  | 301 us                                                 | 79.4 us: 3.79x faster                                          |
| asyncio_tcp               | 643 ms                                                 | 424 ms: 1.52x faster                                           |
| comprehensions            | 14.4 us                                                | 12.4 us: 1.16x faster                                          |
| generators                | 30.3 ms                                                | 26.3 ms: 1.15x faster                                          |
| unpack_sequence           | 33.6 ns                                                | 29.5 ns: 1.14x faster                                          |
| json_dumps                | 7.53 ms                                                | 6.72 ms: 1.12x faster                                          |
| raytrace                  | 206 ms                                                 | 185 ms: 1.11x faster                                           |
| deltablue                 | 2.75 ms                                                | 2.48 ms: 1.11x faster                                          |
| async_tree_none           | 282 ms                                                 | 258 ms: 1.09x faster                                           |
| chaos                     | 47.4 ms                                                | 43.5 ms: 1.09x faster                                          |
| asyncio_tcp_ssl           | 1.40 sec                                               | 1.31 sec: 1.07x faster                                         |
| sqlglot_parse             | 890 us                                                 | 837 us: 1.06x faster                                           |
| sympy_sum                 | 80.2 ms                                                | 76.7 ms: 1.05x faster                                          |
| async_tree_io_tg          | 724 ms                                                 | 695 ms: 1.04x faster                                           |
| async_tree_memoization_tg | 352 ms                                                 | 339 ms: 1.04x faster                                           |
| sqlglot_transpile         | 1.05 ms                                                | 1.02 ms: 1.03x faster                                          |
| pidigits                  | 280 ms                                                 | 274 ms: 1.03x faster                                           |
| async_tree_none_tg        | 276 ms                                                 | 270 ms: 1.02x faster                                           |
| create_gc_cycles          | 711 us                                                 | 706 us: 1.01x faster                                           |
| mako                      | 7.93 ms                                                | 7.90 ms: 1.00x faster                                          |
| regex_dna                 | 148 ms                                                 | 149 ms: 1.00x slower                                           |
| sympy_integrate           | 11.3 ms                                                | 11.3 ms: 1.01x slower                                          |
| gc_traversal              | 2.38 ms                                                | 2.40 ms: 1.01x slower                                          |
| go                        | 105 ms                                                 | 107 ms: 1.02x slower                                           |
| async_tree_io             | 697 ms                                                 | 713 ms: 1.02x slower                                           |
| async_tree_cpu_io_mixed   | 519 ms                                                 | 534 ms: 1.03x slower                                           |
| sympy_str                 | 144 ms                                                 | 150 ms: 1.04x slower                                           |
| deepcopy_memo             | 25.7 us                                                | 27.0 us: 1.05x slower                                          |
| dulwich_log               | 28.6 ms                                                | 30.1 ms: 1.05x slower                                          |
| docutils                  | 1.43 sec                                               | 1.51 sec: 1.06x slower                                         |
| pickle                    | 6.98 us                                                | 7.36 us: 1.06x slower                                          |
| pickle_dict               | 17.1 us                                                | 18.1 us: 1.06x slower                                          |
| regex_effbot              | 2.43 ms                                                | 2.57 ms: 1.06x slower                                          |
| pathlib                   | 23.2 ms                                                | 24.6 ms: 1.06x slower                                          |
| crypto_pyaes              | 47.5 ms                                                | 50.9 ms: 1.07x slower                                          |
| meteor_contest            | 71.1 ms                                                | 76.3 ms: 1.07x slower                                          |
| pycparser                 | 659 ms                                                 | 712 ms: 1.08x slower                                           |
| logging_silent            | 66.5 ns                                                | 72.0 ns: 1.08x slower                                          |
| pickle_list               | 2.70 us                                                | 2.92 us: 1.08x slower                                          |
| xml_etree_parse           | 100 ms                                                 | 109 ms: 1.09x slower                                           |
| pickle_pure_python        | 191 us                                                 | 208 us: 1.09x slower                                           |
| richards_super            | 37.3 ms                                                | 40.7 ms: 1.09x slower                                          |
| hexiom                    | 4.58 ms                                                | 5.00 ms: 1.09x slower                                          |
| unpickle                  | 8.29 us                                                | 9.13 us: 1.10x slower                                          |
| coverage                  | 43.9 ms                                                | 48.3 ms: 1.10x slower                                          |
| logging_simple            | 3.41 us                                                | 3.76 us: 1.10x slower                                          |
| logging_format            | 3.67 us                                                | 4.06 us: 1.10x slower                                          |
| regex_compile             | 72.8 ms                                                | 80.5 ms: 1.10x slower                                          |
| deepcopy                  | 215 us                                                 | 240 us: 1.11x slower                                           |
| json                      | 2.75 ms                                                | 3.07 ms: 1.11x slower                                          |
| regex_v8                  | 15.1 ms                                                | 16.9 ms: 1.12x slower                                          |
| unpickle_pure_python      | 149 us                                                 | 166 us: 1.12x slower                                           |
| bench_mp_pool             | 41.0 ms                                                | 45.9 ms: 1.12x slower                                          |
| scimark_monte_carlo       | 43.5 ms                                                | 48.9 ms: 1.12x slower                                          |
| sympy_expand              | 229 ms                                                 | 258 ms: 1.13x slower                                           |
| xml_etree_iterparse       | 68.3 ms                                                | 77.1 ms: 1.13x slower                                          |
| json_loads                | 15.3 us                                                | 17.4 us: 1.13x slower                                          |
| pprint_pformat            | 979 ms                                                 | 1.11 sec: 1.13x slower                                         |
| bench_thread_pool         | 465 us                                                 | 527 us: 1.13x slower                                           |
| scimark_lu                | 67.7 ms                                                | 77.1 ms: 1.14x slower                                          |
| coroutines                | 17.2 ms                                                | 19.5 ms: 1.14x slower                                          |
| scimark_sparse_mat_mult   | 2.81 ms                                                | 3.20 ms: 1.14x slower                                          |
| nqueens                   | 55.9 ms                                                | 63.8 ms: 1.14x slower                                          |
| pprint_safe_repr          | 478 ms                                                 | 547 ms: 1.14x slower                                           |
| float                     | 50.8 ms                                                | 58.5 ms: 1.15x slower                                          |
| 2to3                      | 154 ms                                                 | 178 ms: 1.15x slower                                           |
| spectral_norm             | 65.7 ms                                                | 75.8 ms: 1.15x slower                                          |
| mdp                       | 1.48 sec                                               | 1.72 sec: 1.16x slower                                         |
| unpickle_list             | 2.69 us                                                | 3.12 us: 1.16x slower                                          |
| deepcopy_reduce           | 1.79 us                                                | 2.12 us: 1.18x slower                                          |
| richards                  | 31.1 ms                                                | 36.8 ms: 1.18x slower                                          |
| sqlglot_normalize         | 162 ms                                                 | 194 ms: 1.20x slower                                           |
| fannkuch                  | 240 ms                                                 | 287 ms: 1.20x slower                                           |
| chameleon                 | 4.30 ms                                                | 5.16 ms: 1.20x slower                                          |
| pyflate                   | 284 ms                                                 | 346 ms: 1.22x slower                                           |
| sqlglot_optimize          | 29.6 ms                                                | 36.2 ms: 1.22x slower                                          |
| scimark_fft               | 173 ms                                                 | 212 ms: 1.23x slower                                           |
| python_startup            | 10.8 ms                                                | 13.3 ms: 1.23x slower                                          |
| xml_etree_process         | 33.6 ms                                                | 42.0 ms: 1.25x slower                                          |
| tomli_loads               | 1.27 sec                                               | 1.60 sec: 1.26x slower                                         |
| sqlite_synth              | 1.26 us                                                | 1.66 us: 1.32x slower                                          |
| nbody                     | 61.7 ms                                                | 81.7 ms: 1.32x slower                                          |
| xml_etree_generate        | 45.8 ms                                                | 60.9 ms: 1.33x slower                                          |
| scimark_sor               | 79.2 ms                                                | 106 ms: 1.34x slower                                           |
| python_startup_no_site    | 8.57 ms                                                | 11.9 ms: 1.39x slower                                          |
| mypy2                     | 372 ms                                                 | 528 ms: 1.42x slower                                           |
| telco                     | 3.17 ms                                                | 4.77 ms: 1.51x slower                                          |
| async_generators          | 192 ms                                                 | 308 ms: 1.60x slower                                           |
| Geometric mean            | (ref)                                                  | 1.07x slower                                                   |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_cpu_io_mixed_tg, asyncio_websockets, tornado_http
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 1.03x