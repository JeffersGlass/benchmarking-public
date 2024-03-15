
# Results vs. 3.11.0

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: darwin-arm64
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.18x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 174 ms: 1.13x slower                                                   |
| chameleon      | 4.30 ms                                                | 4.82 ms: 1.12x slower                                                  |
| docutils       | 1.43 sec                                               | 1.47 sec: 1.03x slower                                                 |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 251 ms: 1.12x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 321 ms: 1.10x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 661 ms: 1.10x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 528 ms: 1.04x faster                                                   |
| async_tree_memoization     | 336 ms                                                 | 326 ms: 1.03x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 55.6 ms: 1.09x slower                                                  |
| nbody          | 61.7 ms                                                | 76.6 ms: 1.24x slower                                                  |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.02x slower                                                   |
| regex_compile  | 72.8 ms                                                | 75.5 ms: 1.04x slower                                                  |
| regex_effbot   | 2.43 ms                                                | 2.56 ms: 1.05x slower                                                  |
| regex_v8       | 15.1 ms                                                | 17.0 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.47 ms: 1.16x faster                                                  |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.02x slower                                                   |
| pickle               | 6.98 us                                                | 7.32 us: 1.05x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 106 ms: 1.06x slower                                                   |
| pickle_dict          | 17.1 us                                                | 18.2 us: 1.07x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 159 us: 1.07x slower                                                   |
| unpickle             | 8.29 us                                                | 9.16 us: 1.10x slower                                                  |
| json_loads           | 15.3 us                                                | 17.0 us: 1.11x slower                                                  |
| pickle_list          | 2.70 us                                                | 2.98 us: 1.11x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.41 sec: 1.11x slower                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 75.7 ms: 1.11x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.09 us: 1.15x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 38.7 ms: 1.15x slower                                                  |
| xml_etree_generate   | 45.8 ms                                                | 55.2 ms: 1.21x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.3 ms: 1.24x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.9 ms: 1.39x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 7.80 ms: 1.02x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 70.7 us: 4.26x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 427 ms: 1.51x faster                                                   |
| unpack_sequence            | 33.6 ns                                                | 28.5 ns: 1.18x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.47 ms: 1.16x faster                                                  |
| raytrace                   | 206 ms                                                 | 177 ms: 1.16x faster                                                   |
| chaos                      | 47.4 ms                                                | 41.5 ms: 1.14x faster                                                  |
| comprehensions             | 14.4 us                                                | 12.6 us: 1.14x faster                                                  |
| async_tree_none            | 282 ms                                                 | 251 ms: 1.12x faster                                                   |
| sqlglot_parse              | 890 us                                                 | 795 us: 1.12x faster                                                   |
| deltablue                  | 2.75 ms                                                | 2.46 ms: 1.12x faster                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 321 ms: 1.10x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 661 ms: 1.10x faster                                                   |
| generators                 | 30.3 ms                                                | 28.2 ms: 1.08x faster                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.30 sec: 1.08x faster                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 979 us: 1.07x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                   |
| sympy_sum                  | 80.2 ms                                                | 75.5 ms: 1.06x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 528 ms: 1.04x faster                                                   |
| richards_super             | 37.3 ms                                                | 35.8 ms: 1.04x faster                                                  |
| async_tree_memoization     | 336 ms                                                 | 326 ms: 1.03x faster                                                   |
| mako                       | 7.93 ms                                                | 7.80 ms: 1.02x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 706 us: 1.01x faster                                                   |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                                   |
| gc_traversal               | 2.38 ms                                                | 2.39 ms: 1.00x slower                                                  |
| sympy_integrate            | 11.3 ms                                                | 11.3 ms: 1.00x slower                                                  |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| logging_simple             | 3.41 us                                                | 3.45 us: 1.01x slower                                                  |
| deepcopy_memo              | 25.7 us                                                | 26.1 us: 1.01x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.02x slower                                                   |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.02x slower                                                   |
| logging_format             | 3.67 us                                                | 3.78 us: 1.03x slower                                                  |
| dask                       | 219 ms                                                 | 225 ms: 1.03x slower                                                   |
| richards                   | 31.1 ms                                                | 32.0 ms: 1.03x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.47 sec: 1.03x slower                                                 |
| crypto_pyaes               | 47.5 ms                                                | 49.1 ms: 1.03x slower                                                  |
| regex_compile              | 72.8 ms                                                | 75.5 ms: 1.04x slower                                                  |
| go                         | 105 ms                                                 | 109 ms: 1.04x slower                                                   |
| dulwich_log                | 28.6 ms                                                | 29.7 ms: 1.04x slower                                                  |
| deepcopy                   | 215 us                                                 | 224 us: 1.04x slower                                                   |
| pathlib                    | 23.2 ms                                                | 24.3 ms: 1.05x slower                                                  |
| pickle                     | 6.98 us                                                | 7.32 us: 1.05x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 74.7 ms: 1.05x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.56 ms: 1.05x slower                                                  |
| pycparser                  | 659 ms                                                 | 695 ms: 1.05x slower                                                   |
| xml_etree_parse            | 100 ms                                                 | 106 ms: 1.06x slower                                                   |
| logging_silent             | 66.5 ns                                                | 70.5 ns: 1.06x slower                                                  |
| sympy_expand               | 229 ms                                                 | 243 ms: 1.06x slower                                                   |
| pickle_dict                | 17.1 us                                                | 18.2 us: 1.07x slower                                                  |
| pprint_pformat             | 979 ms                                                 | 1.05 sec: 1.07x slower                                                 |
| unpickle_pure_python       | 149 us                                                 | 159 us: 1.07x slower                                                   |
| json                       | 2.75 ms                                                | 2.95 ms: 1.07x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 513 ms: 1.07x slower                                                   |
| coverage                   | 43.9 ms                                                | 47.2 ms: 1.08x slower                                                  |
| coroutines                 | 17.2 ms                                                | 18.5 ms: 1.08x slower                                                  |
| bench_thread_pool          | 465 us                                                 | 503 us: 1.08x slower                                                   |
| float                      | 50.8 ms                                                | 55.6 ms: 1.09x slower                                                  |
| hexiom                     | 4.58 ms                                                | 5.01 ms: 1.10x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.63 sec: 1.10x slower                                                 |
| scimark_lu                 | 67.7 ms                                                | 74.8 ms: 1.10x slower                                                  |
| unpickle                   | 8.29 us                                                | 9.16 us: 1.10x slower                                                  |
| json_loads                 | 15.3 us                                                | 17.0 us: 1.11x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.98 us: 1.11x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.41 sec: 1.11x slower                                                 |
| nqueens                    | 55.9 ms                                                | 62.1 ms: 1.11x slower                                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 75.7 ms: 1.11x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.00 us: 1.12x slower                                                  |
| chameleon                  | 4.30 ms                                                | 4.82 ms: 1.12x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 48.8 ms: 1.12x slower                                                  |
| regex_v8                   | 15.1 ms                                                | 17.0 ms: 1.12x slower                                                  |
| 2to3                       | 154 ms                                                 | 174 ms: 1.13x slower                                                   |
| sqlglot_normalize          | 162 ms                                                 | 183 ms: 1.13x slower                                                   |
| fannkuch                   | 240 ms                                                 | 275 ms: 1.15x slower                                                   |
| bench_mp_pool              | 41.0 ms                                                | 47.0 ms: 1.15x slower                                                  |
| pyflate                    | 284 ms                                                 | 327 ms: 1.15x slower                                                   |
| unpickle_list              | 2.69 us                                                | 3.09 us: 1.15x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 38.7 ms: 1.15x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 34.5 ms: 1.17x slower                                                  |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.33 ms: 1.19x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 55.2 ms: 1.21x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 80.6 ms: 1.23x slower                                                  |
| python_startup             | 10.8 ms                                                | 13.3 ms: 1.24x slower                                                  |
| nbody                      | 61.7 ms                                                | 76.6 ms: 1.24x slower                                                  |
| scimark_fft                | 173 ms                                                 | 218 ms: 1.26x slower                                                   |
| sqlite_synth               | 1.26 us                                                | 1.62 us: 1.29x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 106 ms: 1.34x slower                                                   |
| python_startup_no_site     | 8.57 ms                                                | 11.9 ms: 1.39x slower                                                  |
| mypy2                      | 372 ms                                                 | 525 ms: 1.41x slower                                                   |
| telco                      | 3.17 ms                                                | 4.59 ms: 1.45x slower                                                  |
| async_generators           | 192 ms                                                 | 302 ms: 1.57x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (4): sympy_str, async_tree_cpu_io_mixed, async_tree_io, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.18x