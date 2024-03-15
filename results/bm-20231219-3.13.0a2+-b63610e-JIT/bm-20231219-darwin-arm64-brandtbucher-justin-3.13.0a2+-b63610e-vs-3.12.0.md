
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: darwin-arm64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 182 ms: 1.08x slower                                           |
| chameleon      | 4.70 ms                                                | 5.12 ms: 1.09x slower                                          |
| docutils       | 1.50 sec                                               | 1.54 sec: 1.02x slower                                         |
| tornado_http   | 69.3 ms                                                | 72.8 ms: 1.05x slower                                          |
| Geometric mean | (ref)                                                  | 1.06x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 258 ms: 1.03x faster                                           |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 539 ms: 1.01x slower                                           |
| async_tree_io_tg           | 669 ms                                                 | 679 ms: 1.01x slower                                           |
| async_tree_none_tg         | 258 ms                                                 | 264 ms: 1.03x slower                                           |
| async_tree_memoization_tg  | 323 ms                                                 | 331 ms: 1.03x slower                                           |
| async_tree_memoization     | 312 ms                                                 | 334 ms: 1.07x slower                                           |
| async_tree_io              | 668 ms                                                 | 714 ms: 1.07x slower                                           |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                           |
| float          | 55.8 ms                                                | 58.3 ms: 1.04x slower                                          |
| nbody          | 68.8 ms                                                | 79.4 ms: 1.15x slower                                          |
| Geometric mean | (ref)                                                  | 1.07x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 153 ms: 1.01x faster                                           |
| regex_effbot   | 2.64 ms                                                | 2.71 ms: 1.03x slower                                          |
| regex_compile  | 77.9 ms                                                | 80.6 ms: 1.03x slower                                          |
| regex_v8       | 16.0 ms                                                | 17.8 ms: 1.11x slower                                          |
| Geometric mean | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_dict          | 18.1 us                                                | 17.9 us: 1.01x faster                                          |
| unpickle             | 9.12 us                                                | 9.16 us: 1.01x slower                                          |
| pickle_list          | 2.89 us                                                | 2.93 us: 1.01x slower                                          |
| xml_etree_parse      | 106 ms                                                 | 109 ms: 1.02x slower                                           |
| unpickle_list        | 3.02 us                                                | 3.11 us: 1.03x slower                                          |
| pickle_pure_python   | 200 us                                                 | 207 us: 1.04x slower                                           |
| pickle               | 7.23 us                                                | 7.51 us: 1.04x slower                                          |
| xml_etree_process    | 39.7 ms                                                | 41.3 ms: 1.04x slower                                          |
| xml_etree_iterparse  | 74.0 ms                                                | 77.6 ms: 1.05x slower                                          |
| xml_etree_generate   | 55.8 ms                                                | 58.6 ms: 1.05x slower                                          |
| json_dumps           | 6.22 ms                                                | 6.68 ms: 1.07x slower                                          |
| tomli_loads          | 1.39 sec                                               | 1.53 sec: 1.10x slower                                         |
| unpickle_pure_python | 151 us                                                 | 169 us: 1.12x slower                                           |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                   |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.3 ms: 1.17x slower                                          |
| python_startup_no_site | 9.37 ms                                                | 12.0 ms: 1.28x slower                                          |
| Geometric mean         | (ref)                                                  | 1.22x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 8.10 ms: 1.05x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 75.8 us: 1.23x faster                                          |
| generators                 | 31.1 ms                                                | 25.7 ms: 1.21x faster                                          |
| raytrace                   | 212 ms                                                 | 188 ms: 1.12x faster                                           |
| unpack_sequence            | 31.5 ns                                                | 29.0 ns: 1.09x faster                                          |
| comprehensions             | 14.5 us                                                | 13.7 us: 1.06x faster                                          |
| deepcopy_memo              | 27.7 us                                                | 26.5 us: 1.04x faster                                          |
| logging_silent             | 76.4 ns                                                | 73.6 ns: 1.04x faster                                          |
| deltablue                  | 2.71 ms                                                | 2.62 ms: 1.03x faster                                          |
| async_tree_none            | 266 ms                                                 | 258 ms: 1.03x faster                                           |
| json                       | 3.09 ms                                                | 3.02 ms: 1.02x faster                                          |
| crypto_pyaes               | 51.9 ms                                                | 50.9 ms: 1.02x faster                                          |
| coroutines                 | 19.2 ms                                                | 19.0 ms: 1.01x faster                                          |
| regex_dna                  | 154 ms                                                 | 153 ms: 1.01x faster                                           |
| pickle_dict                | 18.1 us                                                | 17.9 us: 1.01x faster                                          |
| asyncio_websockets         | 409 ms                                                 | 409 ms: 1.00x faster                                           |
| gc_traversal               | 2.40 ms                                                | 2.40 ms: 1.00x faster                                          |
| logging_simple             | 3.69 us                                                | 3.69 us: 1.00x slower                                          |
| create_gc_cycles           | 701 us                                                 | 704 us: 1.00x slower                                           |
| unpickle                   | 9.12 us                                                | 9.16 us: 1.01x slower                                          |
| logging_format             | 3.98 us                                                | 4.00 us: 1.01x slower                                          |
| pidigits                   | 282 ms                                                 | 284 ms: 1.01x slower                                           |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 539 ms: 1.01x slower                                           |
| pickle_list                | 2.89 us                                                | 2.93 us: 1.01x slower                                          |
| async_tree_io_tg           | 669 ms                                                 | 679 ms: 1.01x slower                                           |
| deepcopy                   | 235 us                                                 | 238 us: 1.02x slower                                           |
| xml_etree_parse            | 106 ms                                                 | 109 ms: 1.02x slower                                           |
| docutils                   | 1.50 sec                                               | 1.54 sec: 1.02x slower                                         |
| dulwich_log                | 29.8 ms                                                | 30.5 ms: 1.02x slower                                          |
| chaos                      | 42.5 ms                                                | 43.6 ms: 1.02x slower                                          |
| async_tree_none_tg         | 258 ms                                                 | 264 ms: 1.03x slower                                           |
| async_tree_memoization_tg  | 323 ms                                                 | 331 ms: 1.03x slower                                           |
| regex_effbot               | 2.64 ms                                                | 2.71 ms: 1.03x slower                                          |
| pathlib                    | 24.2 ms                                                | 24.9 ms: 1.03x slower                                          |
| deepcopy_reduce            | 2.07 us                                                | 2.13 us: 1.03x slower                                          |
| unpickle_list              | 3.02 us                                                | 3.11 us: 1.03x slower                                          |
| regex_compile              | 77.9 ms                                                | 80.6 ms: 1.03x slower                                          |
| sqlglot_parse              | 848 us                                                 | 878 us: 1.04x slower                                           |
| async_generators           | 304 ms                                                 | 315 ms: 1.04x slower                                           |
| pickle_pure_python         | 200 us                                                 | 207 us: 1.04x slower                                           |
| sympy_str                  | 148 ms                                                 | 153 ms: 1.04x slower                                           |
| pickle                     | 7.23 us                                                | 7.51 us: 1.04x slower                                          |
| xml_etree_process          | 39.7 ms                                                | 41.3 ms: 1.04x slower                                          |
| sympy_sum                  | 77.6 ms                                                | 80.8 ms: 1.04x slower                                          |
| sqlglot_transpile          | 1.02 ms                                                | 1.07 ms: 1.04x slower                                          |
| float                      | 55.8 ms                                                | 58.3 ms: 1.04x slower                                          |
| xml_etree_iterparse        | 74.0 ms                                                | 77.6 ms: 1.05x slower                                          |
| sqlglot_normalize          | 186 ms                                                 | 195 ms: 1.05x slower                                           |
| xml_etree_generate         | 55.8 ms                                                | 58.6 ms: 1.05x slower                                          |
| mako                       | 7.71 ms                                                | 8.10 ms: 1.05x slower                                          |
| tornado_http               | 69.3 ms                                                | 72.8 ms: 1.05x slower                                          |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.31 sec: 1.05x slower                                         |
| dask                       | 222 ms                                                 | 234 ms: 1.05x slower                                           |
| bench_thread_pool          | 504 us                                                 | 531 us: 1.05x slower                                           |
| richards_super             | 36.0 ms                                                | 38.0 ms: 1.06x slower                                          |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.31 ms: 1.06x slower                                          |
| sympy_integrate            | 11.4 ms                                                | 12.0 ms: 1.06x slower                                          |
| scimark_lu                 | 76.0 ms                                                | 80.4 ms: 1.06x slower                                          |
| nqueens                    | 62.4 ms                                                | 66.2 ms: 1.06x slower                                          |
| richards                   | 32.1 ms                                                | 34.1 ms: 1.06x slower                                          |
| sqlite_synth               | 1.57 us                                                | 1.67 us: 1.06x slower                                          |
| bench_mp_pool              | 44.9 ms                                                | 47.8 ms: 1.07x slower                                          |
| async_tree_memoization     | 312 ms                                                 | 334 ms: 1.07x slower                                           |
| async_tree_io              | 668 ms                                                 | 714 ms: 1.07x slower                                           |
| pycparser                  | 677 ms                                                 | 725 ms: 1.07x slower                                           |
| json_dumps                 | 6.22 ms                                                | 6.68 ms: 1.07x slower                                          |
| 2to3                       | 169 ms                                                 | 182 ms: 1.08x slower                                           |
| mdp                        | 1.58 sec                                               | 1.70 sec: 1.08x slower                                         |
| meteor_contest             | 71.7 ms                                                | 77.4 ms: 1.08x slower                                          |
| sympy_expand               | 241 ms                                                 | 260 ms: 1.08x slower                                           |
| spectral_norm              | 76.4 ms                                                | 82.8 ms: 1.08x slower                                          |
| sqlglot_optimize           | 34.0 ms                                                | 36.9 ms: 1.08x slower                                          |
| chameleon                  | 4.70 ms                                                | 5.12 ms: 1.09x slower                                          |
| pprint_safe_repr           | 497 ms                                                 | 546 ms: 1.10x slower                                           |
| tomli_loads                | 1.39 sec                                               | 1.53 sec: 1.10x slower                                         |
| pprint_pformat             | 1.01 sec                                               | 1.11 sec: 1.10x slower                                         |
| pyflate                    | 316 ms                                                 | 351 ms: 1.11x slower                                           |
| regex_v8                   | 16.0 ms                                                | 17.8 ms: 1.11x slower                                          |
| unpickle_pure_python       | 151 us                                                 | 169 us: 1.12x slower                                           |
| go                         | 102 ms                                                 | 115 ms: 1.13x slower                                           |
| scimark_fft                | 195 ms                                                 | 222 ms: 1.14x slower                                           |
| nbody                      | 68.8 ms                                                | 79.4 ms: 1.15x slower                                          |
| scimark_monte_carlo        | 45.0 ms                                                | 52.1 ms: 1.16x slower                                          |
| python_startup             | 11.4 ms                                                | 13.3 ms: 1.17x slower                                          |
| hexiom                     | 4.54 ms                                                | 5.43 ms: 1.20x slower                                          |
| fannkuch                   | 248 ms                                                 | 302 ms: 1.22x slower                                           |
| coverage                   | 38.9 ms                                                | 47.8 ms: 1.23x slower                                          |
| scimark_sor                | 87.4 ms                                                | 109 ms: 1.25x slower                                           |
| telco                      | 3.68 ms                                                | 4.69 ms: 1.27x slower                                          |
| python_startup_no_site     | 9.37 ms                                                | 12.0 ms: 1.28x slower                                          |
| mypy2                      | 380 ms                                                 | 545 ms: 1.43x slower                                           |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                   |

Benchmark hidden because not significant (3): asyncio_tcp, json_loads, async_tree_cpu_io_mixed
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.15x