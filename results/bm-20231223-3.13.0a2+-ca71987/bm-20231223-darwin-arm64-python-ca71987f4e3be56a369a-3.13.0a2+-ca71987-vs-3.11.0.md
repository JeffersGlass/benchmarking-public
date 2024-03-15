
# Results vs. 3.11.0

- fork: python
- ref: ca71987f4e3be56a369a
- machine: darwin-arm64
- commit hash: ca71987
- commit date: 2023-12-23
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 173 ms: 1.12x slower                                                   |
| chameleon      | 4.30 ms                                                | 4.80 ms: 1.12x slower                                                  |
| docutils       | 1.43 sec                                               | 1.49 sec: 1.04x slower                                                 |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 321 ms: 1.10x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 667 ms: 1.08x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 532 ms: 1.03x faster                                                   |
| async_tree_memoization     | 336 ms                                                 | 327 ms: 1.03x faster                                                   |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 523 ms: 1.01x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 58.2 ms: 1.15x slower                                                  |
| nbody          | 61.7 ms                                                | 78.8 ms: 1.28x slower                                                  |
| Geometric mean | (ref)                                                  | 1.14x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 149 ms: 1.00x slower                                                   |
| regex_compile  | 72.8 ms                                                | 74.4 ms: 1.02x slower                                                  |
| regex_effbot   | 2.43 ms                                                | 2.48 ms: 1.02x slower                                                  |
| regex_v8       | 15.1 ms                                                | 16.9 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.62 ms: 1.14x faster                                                  |
| pickle_pure_python   | 191 us                                                 | 199 us: 1.04x slower                                                   |
| pickle_dict          | 17.1 us                                                | 18.0 us: 1.05x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| unpickle_pure_python | 149 us                                                 | 160 us: 1.07x slower                                                   |
| pickle               | 6.98 us                                                | 7.49 us: 1.07x slower                                                  |
| pickle_list          | 2.70 us                                                | 2.93 us: 1.09x slower                                                  |
| unpickle             | 8.29 us                                                | 9.20 us: 1.11x slower                                                  |
| json_loads           | 15.3 us                                                | 17.2 us: 1.12x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 76.4 ms: 1.12x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 40.5 ms: 1.21x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.58 sec: 1.24x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 57.4 ms: 1.25x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.2 ms: 1.23x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.8 ms: 1.38x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 7.67 ms: 1.03x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231223-darwin-arm64-python-ca71987f4e3be56a369a-3.13.0a2+-ca71987 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 73.9 us: 4.07x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 433 ms: 1.49x faster                                                   |
| unpack_sequence            | 33.6 ns                                                | 26.6 ns: 1.26x faster                                                  |
| generators                 | 30.3 ms                                                | 25.2 ms: 1.20x faster                                                  |
| comprehensions             | 14.4 us                                                | 12.2 us: 1.19x faster                                                  |
| chaos                      | 47.4 ms                                                | 40.0 ms: 1.18x faster                                                  |
| raytrace                   | 206 ms                                                 | 175 ms: 1.18x faster                                                   |
| json_dumps                 | 7.53 ms                                                | 6.62 ms: 1.14x faster                                                  |
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                   |
| deltablue                  | 2.75 ms                                                | 2.47 ms: 1.11x faster                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 321 ms: 1.10x faster                                                   |
| sqlglot_parse              | 890 us                                                 | 819 us: 1.09x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 667 ms: 1.08x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                   |
| sympy_sum                  | 80.2 ms                                                | 75.0 ms: 1.07x faster                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.31 sec: 1.07x faster                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 998 us: 1.05x faster                                                   |
| deepcopy_memo              | 25.7 us                                                | 24.8 us: 1.04x faster                                                  |
| mako                       | 7.93 ms                                                | 7.67 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 532 ms: 1.03x faster                                                   |
| sympy_integrate            | 11.3 ms                                                | 11.0 ms: 1.03x faster                                                  |
| async_tree_memoization     | 336 ms                                                 | 327 ms: 1.03x faster                                                   |
| hexiom                     | 4.58 ms                                                | 4.52 ms: 1.01x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 703 us: 1.01x faster                                                   |
| go                         | 105 ms                                                 | 105 ms: 1.01x faster                                                   |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                                   |
| regex_dna                  | 148 ms                                                 | 149 ms: 1.00x slower                                                   |
| sympy_str                  | 144 ms                                                 | 144 ms: 1.00x slower                                                   |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 523 ms: 1.01x slower                                                   |
| richards_super             | 37.3 ms                                                | 37.6 ms: 1.01x slower                                                  |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                  |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| crypto_pyaes               | 47.5 ms                                                | 48.3 ms: 1.02x slower                                                  |
| regex_compile              | 72.8 ms                                                | 74.4 ms: 1.02x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.48 ms: 1.02x slower                                                  |
| dask                       | 219 ms                                                 | 227 ms: 1.03x slower                                                   |
| dulwich_log                | 28.6 ms                                                | 29.7 ms: 1.04x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 199 us: 1.04x slower                                                   |
| docutils                   | 1.43 sec                                               | 1.49 sec: 1.04x slower                                                 |
| coroutines                 | 17.2 ms                                                | 17.9 ms: 1.04x slower                                                  |
| logging_simple             | 3.41 us                                                | 3.56 us: 1.04x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 74.4 ms: 1.05x slower                                                  |
| pickle_dict                | 17.1 us                                                | 18.0 us: 1.05x slower                                                  |
| logging_format             | 3.67 us                                                | 3.88 us: 1.06x slower                                                  |
| deepcopy                   | 215 us                                                 | 228 us: 1.06x slower                                                   |
| pathlib                    | 23.2 ms                                                | 24.6 ms: 1.06x slower                                                  |
| pycparser                  | 659 ms                                                 | 703 ms: 1.07x slower                                                   |
| logging_silent             | 66.5 ns                                                | 71.2 ns: 1.07x slower                                                  |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| unpickle_pure_python       | 149 us                                                 | 160 us: 1.07x slower                                                   |
| pickle                     | 6.98 us                                                | 7.49 us: 1.07x slower                                                  |
| coverage                   | 43.9 ms                                                | 47.4 ms: 1.08x slower                                                  |
| richards                   | 31.1 ms                                                | 33.6 ms: 1.08x slower                                                  |
| pprint_pformat             | 979 ms                                                 | 1.06 sec: 1.09x slower                                                 |
| nqueens                    | 55.9 ms                                                | 60.8 ms: 1.09x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.93 us: 1.09x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 47.6 ms: 1.09x slower                                                  |
| sympy_expand               | 229 ms                                                 | 251 ms: 1.09x slower                                                   |
| pprint_safe_repr           | 478 ms                                                 | 525 ms: 1.10x slower                                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.10 ms: 1.10x slower                                                  |
| bench_thread_pool          | 465 us                                                 | 513 us: 1.10x slower                                                   |
| unpickle                   | 8.29 us                                                | 9.20 us: 1.11x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.65 sec: 1.11x slower                                                 |
| bench_mp_pool              | 41.0 ms                                                | 45.6 ms: 1.11x slower                                                  |
| regex_v8                   | 15.1 ms                                                | 16.9 ms: 1.11x slower                                                  |
| chameleon                  | 4.30 ms                                                | 4.80 ms: 1.12x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 73.5 ms: 1.12x slower                                                  |
| json_loads                 | 15.3 us                                                | 17.2 us: 1.12x slower                                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 76.4 ms: 1.12x slower                                                  |
| scimark_lu                 | 67.7 ms                                                | 75.9 ms: 1.12x slower                                                  |
| 2to3                       | 154 ms                                                 | 173 ms: 1.12x slower                                                   |
| deepcopy_reduce            | 1.79 us                                                | 2.04 us: 1.14x slower                                                  |
| json                       | 2.75 ms                                                | 3.15 ms: 1.14x slower                                                  |
| float                      | 50.8 ms                                                | 58.2 ms: 1.15x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 186 ms: 1.15x slower                                                   |
| unpickle_list              | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| scimark_fft                | 173 ms                                                 | 203 ms: 1.18x slower                                                   |
| sqlglot_optimize           | 29.6 ms                                                | 35.0 ms: 1.18x slower                                                  |
| pyflate                    | 284 ms                                                 | 341 ms: 1.20x slower                                                   |
| xml_etree_process          | 33.6 ms                                                | 40.5 ms: 1.21x slower                                                  |
| fannkuch                   | 240 ms                                                 | 291 ms: 1.22x slower                                                   |
| python_startup             | 10.8 ms                                                | 13.2 ms: 1.23x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.58 sec: 1.24x slower                                                 |
| xml_etree_generate         | 45.8 ms                                                | 57.4 ms: 1.25x slower                                                  |
| nbody                      | 61.7 ms                                                | 78.8 ms: 1.28x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.65 us: 1.32x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 106 ms: 1.33x slower                                                   |
| python_startup_no_site     | 8.57 ms                                                | 11.8 ms: 1.38x slower                                                  |
| mypy2                      | 372 ms                                                 | 522 ms: 1.40x slower                                                   |
| telco                      | 3.17 ms                                                | 4.72 ms: 1.49x slower                                                  |
| async_generators           | 192 ms                                                 | 303 ms: 1.58x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.02x