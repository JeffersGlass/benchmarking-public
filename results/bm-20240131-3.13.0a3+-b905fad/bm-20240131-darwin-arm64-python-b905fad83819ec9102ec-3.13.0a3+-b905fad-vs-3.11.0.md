
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.03x slower
- HPT reliability: 99.98%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 170 ms: 1.10x slower                                                   |
| chameleon      | 4.30 ms                                                | 4.89 ms: 1.14x slower                                                  |
| docutils       | 1.43 sec                                               | 1.45 sec: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 249 ms: 1.13x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 321 ms: 1.10x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 664 ms: 1.09x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 528 ms: 1.04x faster                                                   |
| async_tree_memoization     | 336 ms                                                 | 325 ms: 1.03x faster                                                   |
| async_tree_io              | 697 ms                                                 | 694 ms: 1.00x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 56.4 ms: 1.11x slower                                                  |
| nbody          | 61.7 ms                                                | 75.0 ms: 1.22x slower                                                  |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 72.8 ms                                                | 73.1 ms: 1.00x slower                                                  |
| regex_dna      | 148 ms                                                 | 151 ms: 1.02x slower                                                   |
| regex_effbot   | 2.43 ms                                                | 2.56 ms: 1.05x slower                                                  |
| regex_v8       | 15.1 ms                                                | 17.1 ms: 1.13x slower                                                  |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.49 ms: 1.16x faster                                                  |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.02x slower                                                   |
| unpickle_pure_python | 149 us                                                 | 153 us: 1.03x slower                                                   |
| pickle               | 6.98 us                                                | 7.23 us: 1.04x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 105 ms: 1.05x slower                                                   |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                                  |
| json_loads           | 15.3 us                                                | 16.9 us: 1.10x slower                                                  |
| pickle_list          | 2.70 us                                                | 2.97 us: 1.10x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 75.5 ms: 1.11x slower                                                  |
| unpickle             | 8.29 us                                                | 9.23 us: 1.11x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.09 us: 1.15x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 39.6 ms: 1.18x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.54 sec: 1.21x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 56.1 ms: 1.23x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.09x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.0 ms: 1.21x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.6 ms: 1.36x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.28x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 7.59 ms: 1.05x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 70.8 us: 4.25x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 435 ms: 1.48x faster                                                   |
| comprehensions             | 14.4 us                                                | 11.9 us: 1.21x faster                                                  |
| raytrace                   | 206 ms                                                 | 170 ms: 1.21x faster                                                   |
| chaos                      | 47.4 ms                                                | 39.5 ms: 1.20x faster                                                  |
| unpack_sequence            | 33.6 ns                                                | 28.4 ns: 1.18x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.49 ms: 1.16x faster                                                  |
| deltablue                  | 2.75 ms                                                | 2.43 ms: 1.13x faster                                                  |
| async_tree_none            | 282 ms                                                 | 249 ms: 1.13x faster                                                   |
| sqlglot_parse              | 890 us                                                 | 793 us: 1.12x faster                                                   |
| sympy_sum                  | 80.2 ms                                                | 72.1 ms: 1.11x faster                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.26 sec: 1.11x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 321 ms: 1.10x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 664 ms: 1.09x faster                                                   |
| sqlglot_transpile          | 1.05 ms                                                | 971 us: 1.08x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                   |
| generators                 | 30.3 ms                                                | 28.3 ms: 1.07x faster                                                  |
| sympy_integrate            | 11.3 ms                                                | 10.7 ms: 1.06x faster                                                  |
| mako                       | 7.93 ms                                                | 7.59 ms: 1.05x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 528 ms: 1.04x faster                                                   |
| sympy_str                  | 144 ms                                                 | 139 ms: 1.04x faster                                                   |
| async_tree_memoization     | 336 ms                                                 | 325 ms: 1.03x faster                                                   |
| hexiom                     | 4.58 ms                                                | 4.47 ms: 1.02x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 701 us: 1.01x faster                                                   |
| go                         | 105 ms                                                 | 105 ms: 1.01x faster                                                   |
| async_tree_io              | 697 ms                                                 | 694 ms: 1.00x faster                                                   |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                                   |
| regex_compile              | 72.8 ms                                                | 73.1 ms: 1.00x slower                                                  |
| richards_super             | 37.3 ms                                                | 37.4 ms: 1.00x slower                                                  |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                  |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| logging_simple             | 3.41 us                                                | 3.45 us: 1.01x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.45 sec: 1.02x slower                                                 |
| crypto_pyaes               | 47.5 ms                                                | 48.3 ms: 1.02x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 72.4 ms: 1.02x slower                                                  |
| regex_dna                  | 148 ms                                                 | 151 ms: 1.02x slower                                                   |
| logging_format             | 3.67 us                                                | 3.75 us: 1.02x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.02x slower                                                   |
| dulwich_log                | 28.6 ms                                                | 29.5 ms: 1.03x slower                                                  |
| unpickle_pure_python       | 149 us                                                 | 153 us: 1.03x slower                                                   |
| sympy_expand               | 229 ms                                                 | 237 ms: 1.04x slower                                                   |
| pickle                     | 6.98 us                                                | 7.23 us: 1.04x slower                                                  |
| deepcopy                   | 215 us                                                 | 224 us: 1.04x slower                                                   |
| pycparser                  | 659 ms                                                 | 691 ms: 1.05x slower                                                   |
| mdp                        | 1.48 sec                                               | 1.56 sec: 1.05x slower                                                 |
| xml_etree_parse            | 100 ms                                                 | 105 ms: 1.05x slower                                                   |
| regex_effbot               | 2.43 ms                                                | 2.56 ms: 1.05x slower                                                  |
| logging_silent             | 66.5 ns                                                | 70.1 ns: 1.05x slower                                                  |
| bench_thread_pool          | 465 us                                                 | 491 us: 1.06x slower                                                   |
| pickle_dict                | 17.1 us                                                | 18.1 us: 1.06x slower                                                  |
| pathlib                    | 23.2 ms                                                | 24.6 ms: 1.06x slower                                                  |
| pprint_pformat             | 979 ms                                                 | 1.04 sec: 1.07x slower                                                 |
| json                       | 2.75 ms                                                | 2.94 ms: 1.07x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 513 ms: 1.07x slower                                                   |
| nqueens                    | 55.9 ms                                                | 60.1 ms: 1.07x slower                                                  |
| richards                   | 31.1 ms                                                | 33.5 ms: 1.08x slower                                                  |
| coverage                   | 43.9 ms                                                | 47.6 ms: 1.08x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 47.2 ms: 1.09x slower                                                  |
| bench_mp_pool              | 41.0 ms                                                | 44.7 ms: 1.09x slower                                                  |
| json_loads                 | 15.3 us                                                | 16.9 us: 1.10x slower                                                  |
| 2to3                       | 154 ms                                                 | 170 ms: 1.10x slower                                                   |
| scimark_lu                 | 67.7 ms                                                | 74.7 ms: 1.10x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.97 us: 1.10x slower                                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 75.5 ms: 1.11x slower                                                  |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.11 ms: 1.11x slower                                                  |
| float                      | 50.8 ms                                                | 56.4 ms: 1.11x slower                                                  |
| unpickle                   | 8.29 us                                                | 9.23 us: 1.11x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.00 us: 1.11x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 182 ms: 1.12x slower                                                   |
| regex_v8                   | 15.1 ms                                                | 17.1 ms: 1.13x slower                                                  |
| fannkuch                   | 240 ms                                                 | 271 ms: 1.13x slower                                                   |
| coroutines                 | 17.2 ms                                                | 19.5 ms: 1.14x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 74.7 ms: 1.14x slower                                                  |
| chameleon                  | 4.30 ms                                                | 4.89 ms: 1.14x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 33.7 ms: 1.14x slower                                                  |
| unpickle_list              | 2.69 us                                                | 3.09 us: 1.15x slower                                                  |
| scimark_fft                | 173 ms                                                 | 203 ms: 1.17x slower                                                   |
| pyflate                    | 284 ms                                                 | 334 ms: 1.18x slower                                                   |
| xml_etree_process          | 33.6 ms                                                | 39.6 ms: 1.18x slower                                                  |
| python_startup             | 10.8 ms                                                | 13.0 ms: 1.21x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.54 sec: 1.21x slower                                                 |
| nbody                      | 61.7 ms                                                | 75.0 ms: 1.22x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 56.1 ms: 1.23x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.58 us: 1.26x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 105 ms: 1.32x slower                                                   |
| python_startup_no_site     | 8.57 ms                                                | 11.6 ms: 1.36x slower                                                  |
| mypy2                      | 372 ms                                                 | 511 ms: 1.37x slower                                                   |
| telco                      | 3.17 ms                                                | 4.46 ms: 1.41x slower                                                  |
| async_generators           | 192 ms                                                 | 294 ms: 1.53x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (4): tornado_http, async_tree_cpu_io_mixed, deepcopy_memo, dask
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.98% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.03x