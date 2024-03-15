
# Results vs. 3.12.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: darwin-arm64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.07x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 178 ms: 1.05x slower                                                   |
| chameleon      | 4.70 ms                                                | 4.93 ms: 1.05x slower                                                  |
| docutils       | 1.50 sec                                               | 1.53 sec: 1.02x slower                                                 |
| tornado_http   | 69.3 ms                                                | 71.7 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 259 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 531 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 541 ms: 1.02x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 684 ms: 1.02x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 333 ms: 1.03x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 266 ms: 1.03x slower                                                   |
| async_tree_io              | 668 ms                                                 | 715 ms: 1.07x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 337 ms: 1.08x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                                   |
| float          | 55.8 ms                                                | 70.1 ms: 1.26x slower                                                  |
| nbody          | 68.8 ms                                                | 89.3 ms: 1.30x slower                                                  |
| Geometric mean | (ref)                                                  | 1.18x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.49 ms: 1.06x faster                                                  |
| regex_dna      | 154 ms                                                 | 148 ms: 1.04x faster                                                   |
| regex_v8       | 16.0 ms                                                | 17.0 ms: 1.06x slower                                                  |
| regex_compile  | 77.9 ms                                                | 84.4 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle             | 9.12 us                                                | 9.20 us: 1.01x slower                                                  |
| pickle               | 7.23 us                                                | 7.42 us: 1.03x slower                                                  |
| pickle_dict          | 18.1 us                                                | 18.5 us: 1.03x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.18 us: 1.05x slower                                                  |
| xml_etree_process    | 39.7 ms                                                | 41.8 ms: 1.05x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.68 ms: 1.07x slower                                                  |
| xml_etree_generate   | 55.8 ms                                                | 60.1 ms: 1.08x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 81.2 ms: 1.10x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 167 us: 1.11x slower                                                   |
| tomli_loads          | 1.39 sec                                               | 1.69 sec: 1.21x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (4): pickle_list, pickle_pure_python, json_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.2 ms: 1.16x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.8 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.21x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 9.90 ms: 1.28x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| generators                 | 31.1 ms                                                | 24.8 ms: 1.25x faster                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 76.3 us: 1.22x faster                                                  |
| unpack_sequence            | 31.5 ns                                                | 26.4 ns: 1.19x faster                                                  |
| raytrace                   | 212 ms                                                 | 188 ms: 1.13x faster                                                   |
| coroutines                 | 19.2 ms                                                | 17.9 ms: 1.07x faster                                                  |
| regex_effbot               | 2.64 ms                                                | 2.49 ms: 1.06x faster                                                  |
| logging_silent             | 76.4 ns                                                | 72.4 ns: 1.06x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 26.2 us: 1.06x faster                                                  |
| regex_dna                  | 154 ms                                                 | 148 ms: 1.04x faster                                                   |
| json                       | 3.09 ms                                                | 3.00 ms: 1.03x faster                                                  |
| async_tree_none            | 266 ms                                                 | 259 ms: 1.03x faster                                                   |
| logging_simple             | 3.69 us                                                | 3.65 us: 1.01x faster                                                  |
| sqlglot_parse              | 848 us                                                 | 839 us: 1.01x faster                                                   |
| deepcopy                   | 235 us                                                 | 233 us: 1.01x faster                                                   |
| logging_format             | 3.98 us                                                | 3.96 us: 1.00x faster                                                  |
| gc_traversal               | 2.40 ms                                                | 2.41 ms: 1.00x slower                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 1.03 ms: 1.00x slower                                                  |
| pidigits                   | 282 ms                                                 | 284 ms: 1.01x slower                                                   |
| create_gc_cycles           | 701 us                                                 | 707 us: 1.01x slower                                                   |
| unpickle                   | 9.12 us                                                | 9.20 us: 1.01x slower                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 531 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 541 ms: 1.02x slower                                                   |
| dulwich_log                | 29.8 ms                                                | 30.3 ms: 1.02x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.27 sec: 1.02x slower                                                 |
| richards_super             | 36.0 ms                                                | 36.7 ms: 1.02x slower                                                  |
| docutils                   | 1.50 sec                                               | 1.53 sec: 1.02x slower                                                 |
| richards                   | 32.1 ms                                                | 32.7 ms: 1.02x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 684 ms: 1.02x slower                                                   |
| pathlib                    | 24.2 ms                                                | 24.9 ms: 1.03x slower                                                  |
| pickle                     | 7.23 us                                                | 7.42 us: 1.03x slower                                                  |
| pickle_dict                | 18.1 us                                                | 18.5 us: 1.03x slower                                                  |
| bench_mp_pool              | 44.9 ms                                                | 46.2 ms: 1.03x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 333 ms: 1.03x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 266 ms: 1.03x slower                                                   |
| bench_thread_pool          | 504 us                                                 | 521 us: 1.03x slower                                                   |
| scimark_lu                 | 76.0 ms                                                | 78.6 ms: 1.03x slower                                                  |
| tornado_http               | 69.3 ms                                                | 71.7 ms: 1.03x slower                                                  |
| dask                       | 222 ms                                                 | 230 ms: 1.04x slower                                                   |
| pycparser                  | 677 ms                                                 | 708 ms: 1.05x slower                                                   |
| sympy_integrate            | 11.4 ms                                                | 11.9 ms: 1.05x slower                                                  |
| chameleon                  | 4.70 ms                                                | 4.93 ms: 1.05x slower                                                  |
| 2to3                       | 169 ms                                                 | 178 ms: 1.05x slower                                                   |
| unpickle_list              | 3.02 us                                                | 3.18 us: 1.05x slower                                                  |
| xml_etree_process          | 39.7 ms                                                | 41.8 ms: 1.05x slower                                                  |
| sqlglot_normalize          | 186 ms                                                 | 196 ms: 1.06x slower                                                   |
| sympy_str                  | 148 ms                                                 | 156 ms: 1.06x slower                                                   |
| sympy_sum                  | 77.6 ms                                                | 82.5 ms: 1.06x slower                                                  |
| regex_v8                   | 16.0 ms                                                | 17.0 ms: 1.06x slower                                                  |
| async_tree_io              | 668 ms                                                 | 715 ms: 1.07x slower                                                   |
| crypto_pyaes               | 51.9 ms                                                | 55.7 ms: 1.07x slower                                                  |
| json_dumps                 | 6.22 ms                                                | 6.68 ms: 1.07x slower                                                  |
| sympy_expand               | 241 ms                                                 | 259 ms: 1.07x slower                                                   |
| xml_etree_generate         | 55.8 ms                                                | 60.1 ms: 1.08x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 337 ms: 1.08x slower                                                   |
| regex_compile              | 77.9 ms                                                | 84.4 ms: 1.08x slower                                                  |
| sqlite_synth               | 1.57 us                                                | 1.71 us: 1.09x slower                                                  |
| go                         | 102 ms                                                 | 111 ms: 1.09x slower                                                   |
| sqlglot_optimize           | 34.0 ms                                                | 37.2 ms: 1.09x slower                                                  |
| xml_etree_iterparse        | 74.0 ms                                                | 81.2 ms: 1.10x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.74 sec: 1.10x slower                                                 |
| nqueens                    | 62.4 ms                                                | 68.8 ms: 1.10x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 79.2 ms: 1.10x slower                                                  |
| chaos                      | 42.5 ms                                                | 47.1 ms: 1.11x slower                                                  |
| comprehensions             | 14.5 us                                                | 16.1 us: 1.11x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 167 us: 1.11x slower                                                   |
| python_startup             | 11.4 ms                                                | 13.2 ms: 1.16x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 583 ms: 1.17x slower                                                   |
| pprint_pformat             | 1.01 sec                                               | 1.20 sec: 1.19x slower                                                 |
| pyflate                    | 316 ms                                                 | 374 ms: 1.19x slower                                                   |
| tomli_loads                | 1.39 sec                                               | 1.69 sec: 1.21x slower                                                 |
| coverage                   | 38.9 ms                                                | 48.2 ms: 1.24x slower                                                  |
| scimark_sor                | 87.4 ms                                                | 109 ms: 1.24x slower                                                   |
| float                      | 55.8 ms                                                | 70.1 ms: 1.26x slower                                                  |
| python_startup_no_site     | 9.37 ms                                                | 11.8 ms: 1.26x slower                                                  |
| mako                       | 7.71 ms                                                | 9.90 ms: 1.28x slower                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 58.0 ms: 1.29x slower                                                  |
| nbody                      | 68.8 ms                                                | 89.3 ms: 1.30x slower                                                  |
| hexiom                     | 4.54 ms                                                | 5.96 ms: 1.31x slower                                                  |
| scimark_fft                | 195 ms                                                 | 257 ms: 1.31x slower                                                   |
| deltablue                  | 2.71 ms                                                | 3.64 ms: 1.34x slower                                                  |
| telco                      | 3.68 ms                                                | 4.96 ms: 1.35x slower                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 4.30 ms: 1.37x slower                                                  |
| fannkuch                   | 248 ms                                                 | 341 ms: 1.37x slower                                                   |
| mypy2                      | 380 ms                                                 | 533 ms: 1.40x slower                                                   |
| spectral_norm              | 76.4 ms                                                | 110 ms: 1.44x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.07x slower                                                           |

Benchmark hidden because not significant (8): asyncio_tcp, pickle_list, asyncio_websockets, pickle_pure_python, json_loads, async_generators, deepcopy_reduce, xml_etree_parse
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 0.99x