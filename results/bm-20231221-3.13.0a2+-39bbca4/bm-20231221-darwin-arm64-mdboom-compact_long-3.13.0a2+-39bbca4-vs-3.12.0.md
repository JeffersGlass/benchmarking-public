
# Results vs. 3.12.0

- fork: mdboom
- ref: compact_long
- machine: darwin-arm64
- commit hash: 39bbca4
- commit date: 2023-12-21
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 178 ms: 1.05x slower                                           |
| chameleon      | 4.70 ms                                                | 5.16 ms: 1.10x slower                                          |
| docutils       | 1.50 sec                                               | 1.51 sec: 1.00x slower                                         |
| Geometric mean | (ref)                                                  | 1.04x slower                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 258 ms: 1.03x faster                                           |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 534 ms: 1.02x slower                                           |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 550 ms: 1.03x slower                                           |
| async_tree_io_tg           | 669 ms                                                 | 695 ms: 1.04x slower                                           |
| async_tree_none_tg         | 258 ms                                                 | 270 ms: 1.05x slower                                           |
| async_tree_memoization_tg  | 323 ms                                                 | 339 ms: 1.05x slower                                           |
| async_tree_io              | 668 ms                                                 | 713 ms: 1.07x slower                                           |
| async_tree_memoization     | 312 ms                                                 | 335 ms: 1.07x slower                                           |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 274 ms: 1.03x faster                                           |
| float          | 55.8 ms                                                | 58.5 ms: 1.05x slower                                          |
| nbody          | 68.8 ms                                                | 81.7 ms: 1.19x slower                                          |
| Geometric mean | (ref)                                                  | 1.07x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 149 ms: 1.04x faster                                           |
| regex_effbot   | 2.64 ms                                                | 2.57 ms: 1.03x faster                                          |
| regex_compile  | 77.9 ms                                                | 80.5 ms: 1.03x slower                                          |
| regex_v8       | 16.0 ms                                                | 16.9 ms: 1.06x slower                                          |
| Geometric mean | (ref)                                                  | 1.01x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_loads           | 17.2 us                                                | 17.4 us: 1.01x slower                                          |
| pickle_list          | 2.89 us                                                | 2.92 us: 1.01x slower                                          |
| pickle               | 7.23 us                                                | 7.36 us: 1.02x slower                                          |
| xml_etree_parse      | 106 ms                                                 | 109 ms: 1.02x slower                                           |
| unpickle_list        | 3.02 us                                                | 3.12 us: 1.03x slower                                          |
| xml_etree_iterparse  | 74.0 ms                                                | 77.1 ms: 1.04x slower                                          |
| pickle_pure_python   | 200 us                                                 | 208 us: 1.04x slower                                           |
| xml_etree_process    | 39.7 ms                                                | 42.0 ms: 1.06x slower                                          |
| json_dumps           | 6.22 ms                                                | 6.72 ms: 1.08x slower                                          |
| xml_etree_generate   | 55.8 ms                                                | 60.9 ms: 1.09x slower                                          |
| unpickle_pure_python | 151 us                                                 | 166 us: 1.10x slower                                           |
| tomli_loads          | 1.39 sec                                               | 1.60 sec: 1.15x slower                                         |
| Geometric mean       | (ref)                                                  | 1.05x slower                                                   |

Benchmark hidden because not significant (2): unpickle, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.3 ms: 1.16x slower                                          |
| python_startup_no_site | 9.37 ms                                                | 11.9 ms: 1.27x slower                                          |
| Geometric mean         | (ref)                                                  | 1.22x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.90 ms: 1.02x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231221-darwin-arm64-mdboom-compact_long-3.13.0a2+-39bbca4 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| generators                 | 31.1 ms                                                | 26.3 ms: 1.18x faster                                          |
| typing_runtime_protocols   | 93.0 us                                                | 79.4 us: 1.17x faster                                          |
| comprehensions             | 14.5 us                                                | 12.4 us: 1.17x faster                                          |
| raytrace                   | 212 ms                                                 | 185 ms: 1.14x faster                                           |
| deltablue                  | 2.71 ms                                                | 2.48 ms: 1.09x faster                                          |
| unpack_sequence            | 31.5 ns                                                | 29.5 ns: 1.07x faster                                          |
| logging_silent             | 76.4 ns                                                | 72.0 ns: 1.06x faster                                          |
| regex_dna                  | 154 ms                                                 | 149 ms: 1.04x faster                                           |
| pidigits                   | 282 ms                                                 | 274 ms: 1.03x faster                                           |
| async_tree_none            | 266 ms                                                 | 258 ms: 1.03x faster                                           |
| regex_effbot               | 2.64 ms                                                | 2.57 ms: 1.03x faster                                          |
| deepcopy_memo              | 27.7 us                                                | 27.0 us: 1.02x faster                                          |
| crypto_pyaes               | 51.9 ms                                                | 50.9 ms: 1.02x faster                                          |
| sqlglot_parse              | 848 us                                                 | 837 us: 1.01x faster                                           |
| sympy_sum                  | 77.6 ms                                                | 76.7 ms: 1.01x faster                                          |
| spectral_norm              | 76.4 ms                                                | 75.8 ms: 1.01x faster                                          |
| json                       | 3.09 ms                                                | 3.07 ms: 1.01x faster                                          |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                           |
| docutils                   | 1.50 sec                                               | 1.51 sec: 1.00x slower                                         |
| create_gc_cycles           | 701 us                                                 | 706 us: 1.01x slower                                           |
| json_loads                 | 17.2 us                                                | 17.4 us: 1.01x slower                                          |
| dulwich_log                | 29.8 ms                                                | 30.1 ms: 1.01x slower                                          |
| pickle_list                | 2.89 us                                                | 2.92 us: 1.01x slower                                          |
| async_generators           | 304 ms                                                 | 308 ms: 1.01x slower                                           |
| scimark_lu                 | 76.0 ms                                                | 77.1 ms: 1.01x slower                                          |
| pathlib                    | 24.2 ms                                                | 24.6 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 534 ms: 1.02x slower                                           |
| sympy_str                  | 148 ms                                                 | 150 ms: 1.02x slower                                           |
| coroutines                 | 19.2 ms                                                | 19.5 ms: 1.02x slower                                          |
| logging_format             | 3.98 us                                                | 4.06 us: 1.02x slower                                          |
| pickle                     | 7.23 us                                                | 7.36 us: 1.02x slower                                          |
| logging_simple             | 3.69 us                                                | 3.76 us: 1.02x slower                                          |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.20 ms: 1.02x slower                                          |
| deepcopy                   | 235 us                                                 | 240 us: 1.02x slower                                           |
| nqueens                    | 62.4 ms                                                | 63.8 ms: 1.02x slower                                          |
| bench_mp_pool              | 44.9 ms                                                | 45.9 ms: 1.02x slower                                          |
| chaos                      | 42.5 ms                                                | 43.5 ms: 1.02x slower                                          |
| xml_etree_parse            | 106 ms                                                 | 109 ms: 1.02x slower                                           |
| mako                       | 7.71 ms                                                | 7.90 ms: 1.02x slower                                          |
| deepcopy_reduce            | 2.07 us                                                | 2.12 us: 1.03x slower                                          |
| unpickle_list              | 3.02 us                                                | 3.12 us: 1.03x slower                                          |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 550 ms: 1.03x slower                                           |
| regex_compile              | 77.9 ms                                                | 80.5 ms: 1.03x slower                                          |
| async_tree_io_tg           | 669 ms                                                 | 695 ms: 1.04x slower                                           |
| xml_etree_iterparse        | 74.0 ms                                                | 77.1 ms: 1.04x slower                                          |
| pickle_pure_python         | 200 us                                                 | 208 us: 1.04x slower                                           |
| sqlglot_normalize          | 186 ms                                                 | 194 ms: 1.04x slower                                           |
| bench_thread_pool          | 504 us                                                 | 527 us: 1.05x slower                                           |
| async_tree_none_tg         | 258 ms                                                 | 270 ms: 1.05x slower                                           |
| float                      | 55.8 ms                                                | 58.5 ms: 1.05x slower                                          |
| 2to3                       | 169 ms                                                 | 178 ms: 1.05x slower                                           |
| pycparser                  | 677 ms                                                 | 712 ms: 1.05x slower                                           |
| async_tree_memoization_tg  | 323 ms                                                 | 339 ms: 1.05x slower                                           |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.31 sec: 1.05x slower                                         |
| sqlite_synth               | 1.57 us                                                | 1.66 us: 1.05x slower                                          |
| go                         | 102 ms                                                 | 107 ms: 1.06x slower                                           |
| xml_etree_process          | 39.7 ms                                                | 42.0 ms: 1.06x slower                                          |
| regex_v8                   | 16.0 ms                                                | 16.9 ms: 1.06x slower                                          |
| meteor_contest             | 71.7 ms                                                | 76.3 ms: 1.06x slower                                          |
| sqlglot_optimize           | 34.0 ms                                                | 36.2 ms: 1.06x slower                                          |
| async_tree_io              | 668 ms                                                 | 713 ms: 1.07x slower                                           |
| sympy_expand               | 241 ms                                                 | 258 ms: 1.07x slower                                           |
| async_tree_memoization     | 312 ms                                                 | 335 ms: 1.07x slower                                           |
| json_dumps                 | 6.22 ms                                                | 6.72 ms: 1.08x slower                                          |
| scimark_fft                | 195 ms                                                 | 212 ms: 1.08x slower                                           |
| scimark_monte_carlo        | 45.0 ms                                                | 48.9 ms: 1.09x slower                                          |
| mdp                        | 1.58 sec                                               | 1.72 sec: 1.09x slower                                         |
| xml_etree_generate         | 55.8 ms                                                | 60.9 ms: 1.09x slower                                          |
| pyflate                    | 316 ms                                                 | 346 ms: 1.10x slower                                           |
| pprint_pformat             | 1.01 sec                                               | 1.11 sec: 1.10x slower                                         |
| chameleon                  | 4.70 ms                                                | 5.16 ms: 1.10x slower                                          |
| hexiom                     | 4.54 ms                                                | 5.00 ms: 1.10x slower                                          |
| pprint_safe_repr           | 497 ms                                                 | 547 ms: 1.10x slower                                           |
| unpickle_pure_python       | 151 us                                                 | 166 us: 1.10x slower                                           |
| richards_super             | 36.0 ms                                                | 40.7 ms: 1.13x slower                                          |
| richards                   | 32.1 ms                                                | 36.8 ms: 1.14x slower                                          |
| tomli_loads                | 1.39 sec                                               | 1.60 sec: 1.15x slower                                         |
| fannkuch                   | 248 ms                                                 | 287 ms: 1.16x slower                                           |
| python_startup             | 11.4 ms                                                | 13.3 ms: 1.16x slower                                          |
| nbody                      | 68.8 ms                                                | 81.7 ms: 1.19x slower                                          |
| scimark_sor                | 87.4 ms                                                | 106 ms: 1.22x slower                                           |
| coverage                   | 38.9 ms                                                | 48.3 ms: 1.24x slower                                          |
| python_startup_no_site     | 9.37 ms                                                | 11.9 ms: 1.27x slower                                          |
| telco                      | 3.68 ms                                                | 4.77 ms: 1.30x slower                                          |
| mypy2                      | 380 ms                                                 | 528 ms: 1.39x slower                                           |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                   |

Benchmark hidden because not significant (7): asyncio_tcp, sympy_integrate, sqlglot_transpile, unpickle, pickle_dict, gc_traversal, tornado_http
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.99x