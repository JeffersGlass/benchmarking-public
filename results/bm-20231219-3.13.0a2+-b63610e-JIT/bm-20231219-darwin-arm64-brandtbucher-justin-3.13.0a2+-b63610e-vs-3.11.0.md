
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: darwin-arm64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x slower
- Memory change: 1.19x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 182 ms: 1.18x slower                                           |
| chameleon      | 4.30 ms                                                | 5.12 ms: 1.19x slower                                          |
| docutils       | 1.43 sec                                               | 1.54 sec: 1.07x slower                                         |
| tornado_http   | 69.1 ms                                                | 72.8 ms: 1.05x slower                                          |
| Geometric mean | (ref)                                                  | 1.12x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 258 ms: 1.09x faster                                           |
| async_tree_io_tg           | 724 ms                                                 | 679 ms: 1.07x faster                                           |
| async_tree_memoization_tg  | 352 ms                                                 | 331 ms: 1.06x faster                                           |
| async_tree_none_tg         | 276 ms                                                 | 264 ms: 1.05x faster                                           |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 539 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 530 ms: 1.02x slower                                           |
| async_tree_io              | 697 ms                                                 | 714 ms: 1.02x slower                                           |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                   |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 284 ms: 1.01x slower                                           |
| float          | 50.8 ms                                                | 58.3 ms: 1.15x slower                                          |
| nbody          | 61.7 ms                                                | 79.4 ms: 1.29x slower                                          |
| Geometric mean | (ref)                                                  | 1.14x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 153 ms: 1.03x slower                                           |
| regex_compile  | 72.8 ms                                                | 80.6 ms: 1.11x slower                                          |
| regex_effbot   | 2.43 ms                                                | 2.71 ms: 1.12x slower                                          |
| regex_v8       | 15.1 ms                                                | 17.8 ms: 1.17x slower                                          |
| Geometric mean | (ref)                                                  | 1.11x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.68 ms: 1.13x faster                                          |
| pickle_dict          | 17.1 us                                                | 17.9 us: 1.05x slower                                          |
| pickle               | 6.98 us                                                | 7.51 us: 1.08x slower                                          |
| xml_etree_parse      | 100 ms                                                 | 109 ms: 1.08x slower                                           |
| pickle_pure_python   | 191 us                                                 | 207 us: 1.08x slower                                           |
| pickle_list          | 2.70 us                                                | 2.93 us: 1.09x slower                                          |
| unpickle             | 8.29 us                                                | 9.16 us: 1.11x slower                                          |
| json_loads           | 15.3 us                                                | 17.3 us: 1.12x slower                                          |
| unpickle_pure_python | 149 us                                                 | 169 us: 1.14x slower                                           |
| xml_etree_iterparse  | 68.3 ms                                                | 77.6 ms: 1.14x slower                                          |
| unpickle_list        | 2.69 us                                                | 3.11 us: 1.16x slower                                          |
| tomli_loads          | 1.27 sec                                               | 1.53 sec: 1.20x slower                                         |
| xml_etree_process    | 33.6 ms                                                | 41.3 ms: 1.23x slower                                          |
| xml_etree_generate   | 45.8 ms                                                | 58.6 ms: 1.28x slower                                          |
| Geometric mean       | (ref)                                                  | 1.11x slower                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.3 ms: 1.24x slower                                          |
| python_startup_no_site | 8.57 ms                                                | 12.0 ms: 1.40x slower                                          |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 8.10 ms: 1.02x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 75.8 us: 3.97x faster                                          |
| asyncio_tcp                | 643 ms                                                 | 430 ms: 1.50x faster                                           |
| generators                 | 30.3 ms                                                | 25.7 ms: 1.18x faster                                          |
| unpack_sequence            | 33.6 ns                                                | 29.0 ns: 1.16x faster                                          |
| json_dumps                 | 7.53 ms                                                | 6.68 ms: 1.13x faster                                          |
| async_tree_none            | 282 ms                                                 | 258 ms: 1.09x faster                                           |
| raytrace                   | 206 ms                                                 | 188 ms: 1.09x faster                                           |
| chaos                      | 47.4 ms                                                | 43.6 ms: 1.09x faster                                          |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.31 sec: 1.07x faster                                         |
| async_tree_io_tg           | 724 ms                                                 | 679 ms: 1.07x faster                                           |
| async_tree_memoization_tg  | 352 ms                                                 | 331 ms: 1.06x faster                                           |
| comprehensions             | 14.4 us                                                | 13.7 us: 1.06x faster                                          |
| deltablue                  | 2.75 ms                                                | 2.62 ms: 1.05x faster                                          |
| async_tree_none_tg         | 276 ms                                                 | 264 ms: 1.05x faster                                           |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 539 ms: 1.02x faster                                           |
| sqlglot_parse              | 890 us                                                 | 878 us: 1.01x faster                                           |
| create_gc_cycles           | 711 us                                                 | 704 us: 1.01x faster                                           |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                          |
| sympy_sum                  | 80.2 ms                                                | 80.8 ms: 1.01x slower                                          |
| pidigits                   | 280 ms                                                 | 284 ms: 1.01x slower                                           |
| sqlglot_transpile          | 1.05 ms                                                | 1.07 ms: 1.01x slower                                          |
| richards_super             | 37.3 ms                                                | 38.0 ms: 1.02x slower                                          |
| mako                       | 7.93 ms                                                | 8.10 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 530 ms: 1.02x slower                                           |
| async_tree_io              | 697 ms                                                 | 714 ms: 1.02x slower                                           |
| regex_dna                  | 148 ms                                                 | 153 ms: 1.03x slower                                           |
| deepcopy_memo              | 25.7 us                                                | 26.5 us: 1.03x slower                                          |
| pickle_dict                | 17.1 us                                                | 17.9 us: 1.05x slower                                          |
| tornado_http               | 69.1 ms                                                | 72.8 ms: 1.05x slower                                          |
| sympy_str                  | 144 ms                                                 | 153 ms: 1.07x slower                                           |
| dulwich_log                | 28.6 ms                                                | 30.5 ms: 1.07x slower                                          |
| sympy_integrate            | 11.3 ms                                                | 12.0 ms: 1.07x slower                                          |
| dask                       | 219 ms                                                 | 234 ms: 1.07x slower                                           |
| crypto_pyaes               | 47.5 ms                                                | 50.9 ms: 1.07x slower                                          |
| pathlib                    | 23.2 ms                                                | 24.9 ms: 1.07x slower                                          |
| docutils                   | 1.43 sec                                               | 1.54 sec: 1.07x slower                                         |
| pickle                     | 6.98 us                                                | 7.51 us: 1.08x slower                                          |
| xml_etree_parse            | 100 ms                                                 | 109 ms: 1.08x slower                                           |
| pickle_pure_python         | 191 us                                                 | 207 us: 1.08x slower                                           |
| logging_simple             | 3.41 us                                                | 3.69 us: 1.08x slower                                          |
| pickle_list                | 2.70 us                                                | 2.93 us: 1.09x slower                                          |
| meteor_contest             | 71.1 ms                                                | 77.4 ms: 1.09x slower                                          |
| logging_format             | 3.67 us                                                | 4.00 us: 1.09x slower                                          |
| coverage                   | 43.9 ms                                                | 47.8 ms: 1.09x slower                                          |
| go                         | 105 ms                                                 | 115 ms: 1.09x slower                                           |
| json                       | 2.75 ms                                                | 3.02 ms: 1.10x slower                                          |
| richards                   | 31.1 ms                                                | 34.1 ms: 1.10x slower                                          |
| pycparser                  | 659 ms                                                 | 725 ms: 1.10x slower                                           |
| unpickle                   | 8.29 us                                                | 9.16 us: 1.11x slower                                          |
| regex_compile              | 72.8 ms                                                | 80.6 ms: 1.11x slower                                          |
| coroutines                 | 17.2 ms                                                | 19.0 ms: 1.11x slower                                          |
| deepcopy                   | 215 us                                                 | 238 us: 1.11x slower                                           |
| logging_silent             | 66.5 ns                                                | 73.6 ns: 1.11x slower                                          |
| regex_effbot               | 2.43 ms                                                | 2.71 ms: 1.12x slower                                          |
| json_loads                 | 15.3 us                                                | 17.3 us: 1.12x slower                                          |
| pprint_pformat             | 979 ms                                                 | 1.11 sec: 1.14x slower                                         |
| unpickle_pure_python       | 149 us                                                 | 169 us: 1.14x slower                                           |
| sympy_expand               | 229 ms                                                 | 260 ms: 1.14x slower                                           |
| xml_etree_iterparse        | 68.3 ms                                                | 77.6 ms: 1.14x slower                                          |
| pprint_safe_repr           | 478 ms                                                 | 546 ms: 1.14x slower                                           |
| bench_thread_pool          | 465 us                                                 | 531 us: 1.14x slower                                           |
| mdp                        | 1.48 sec                                               | 1.70 sec: 1.15x slower                                         |
| float                      | 50.8 ms                                                | 58.3 ms: 1.15x slower                                          |
| unpickle_list              | 2.69 us                                                | 3.11 us: 1.16x slower                                          |
| bench_mp_pool              | 41.0 ms                                                | 47.8 ms: 1.17x slower                                          |
| regex_v8                   | 15.1 ms                                                | 17.8 ms: 1.17x slower                                          |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.31 ms: 1.18x slower                                          |
| 2to3                       | 154 ms                                                 | 182 ms: 1.18x slower                                           |
| nqueens                    | 55.9 ms                                                | 66.2 ms: 1.18x slower                                          |
| scimark_lu                 | 67.7 ms                                                | 80.4 ms: 1.19x slower                                          |
| hexiom                     | 4.58 ms                                                | 5.43 ms: 1.19x slower                                          |
| deepcopy_reduce            | 1.79 us                                                | 2.13 us: 1.19x slower                                          |
| chameleon                  | 4.30 ms                                                | 5.12 ms: 1.19x slower                                          |
| scimark_monte_carlo        | 43.5 ms                                                | 52.1 ms: 1.20x slower                                          |
| tomli_loads                | 1.27 sec                                               | 1.53 sec: 1.20x slower                                         |
| sqlglot_normalize          | 162 ms                                                 | 195 ms: 1.20x slower                                           |
| xml_etree_process          | 33.6 ms                                                | 41.3 ms: 1.23x slower                                          |
| pyflate                    | 284 ms                                                 | 351 ms: 1.24x slower                                           |
| python_startup             | 10.8 ms                                                | 13.3 ms: 1.24x slower                                          |
| sqlglot_optimize           | 29.6 ms                                                | 36.9 ms: 1.25x slower                                          |
| spectral_norm              | 65.7 ms                                                | 82.8 ms: 1.26x slower                                          |
| fannkuch                   | 240 ms                                                 | 302 ms: 1.26x slower                                           |
| xml_etree_generate         | 45.8 ms                                                | 58.6 ms: 1.28x slower                                          |
| scimark_fft                | 173 ms                                                 | 222 ms: 1.29x slower                                           |
| nbody                      | 61.7 ms                                                | 79.4 ms: 1.29x slower                                          |
| sqlite_synth               | 1.26 us                                                | 1.67 us: 1.33x slower                                          |
| scimark_sor                | 79.2 ms                                                | 109 ms: 1.38x slower                                           |
| python_startup_no_site     | 8.57 ms                                                | 12.0 ms: 1.40x slower                                          |
| mypy2                      | 372 ms                                                 | 545 ms: 1.46x slower                                           |
| telco                      | 3.17 ms                                                | 4.69 ms: 1.48x slower                                          |
| async_generators           | 192 ms                                                 | 315 ms: 1.64x slower                                           |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                   |

Benchmark hidden because not significant (2): async_tree_memoization, asyncio_websockets
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.07x
- 95% likely to have a slowdown of 1.07x
- 99% likely to have a slowdown of 1.06x


# Memory

- memory change: 1.19x