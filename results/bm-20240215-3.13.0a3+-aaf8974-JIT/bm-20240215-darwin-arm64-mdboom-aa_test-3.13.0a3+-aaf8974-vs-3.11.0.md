
# Results vs. 3.11.0

- fork: mdboom
- ref: aa_test
- machine: darwin-arm64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 191 ms: 1.24x slower                                      |
| chameleon      | 4.30 ms                                                | 4.82 ms: 1.12x slower                                     |
| docutils       | 1.43 sec                                               | 1.47 sec: 1.03x slower                                    |
| Geometric mean | (ref)                                                  | 1.10x slower                                              |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 250 ms: 1.12x faster                                      |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                      |
| async_tree_io_tg           | 724 ms                                                 | 667 ms: 1.09x faster                                      |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                      |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                      |
| async_tree_memoization     | 336 ms                                                 | 328 ms: 1.03x faster                                      |
| Geometric mean             | (ref)                                                  | 1.05x faster                                              |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.01x slower                                      |
| float          | 50.8 ms                                                | 55.4 ms: 1.09x slower                                     |
| nbody          | 61.7 ms                                                | 76.0 ms: 1.23x slower                                     |
| Geometric mean | (ref)                                                  | 1.11x slower                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 145 ms: 1.02x faster                                      |
| regex_effbot   | 2.43 ms                                                | 2.46 ms: 1.01x slower                                     |
| regex_compile  | 72.8 ms                                                | 75.2 ms: 1.03x slower                                     |
| regex_v8       | 15.1 ms                                                | 16.9 ms: 1.12x slower                                     |
| Geometric mean | (ref)                                                  | 1.03x slower                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.53 ms: 1.15x faster                                     |
| pickle_pure_python   | 191 us                                                 | 195 us: 1.02x slower                                      |
| pickle               | 6.98 us                                                | 7.27 us: 1.04x slower                                     |
| xml_etree_parse      | 100 ms                                                 | 106 ms: 1.05x slower                                      |
| unpickle_pure_python | 149 us                                                 | 158 us: 1.06x slower                                      |
| pickle_dict          | 17.1 us                                                | 18.2 us: 1.07x slower                                     |
| tomli_loads          | 1.27 sec                                               | 1.41 sec: 1.10x slower                                    |
| xml_etree_iterparse  | 68.3 ms                                                | 75.5 ms: 1.11x slower                                     |
| json_loads           | 15.3 us                                                | 17.0 us: 1.11x slower                                     |
| pickle_list          | 2.70 us                                                | 2.99 us: 1.11x slower                                     |
| unpickle             | 8.29 us                                                | 9.23 us: 1.11x slower                                     |
| unpickle_list        | 2.69 us                                                | 3.10 us: 1.15x slower                                     |
| xml_etree_process    | 33.6 ms                                                | 39.3 ms: 1.17x slower                                     |
| xml_etree_generate   | 45.8 ms                                                | 55.7 ms: 1.22x slower                                     |
| Geometric mean       | (ref)                                                  | 1.08x slower                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.6 ms: 1.27x slower                                     |
| python_startup_no_site | 8.57 ms                                                | 12.2 ms: 1.43x slower                                     |
| Geometric mean         | (ref)                                                  | 1.35x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 7.93 ms                                                | 7.78 ms: 1.02x faster                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 71.5 us: 4.21x faster                                     |
| asyncio_tcp                | 643 ms                                                 | 401 ms: 1.60x faster                                      |
| unpack_sequence            | 33.6 ns                                                | 28.4 ns: 1.18x faster                                     |
| raytrace                   | 206 ms                                                 | 176 ms: 1.17x faster                                      |
| json_dumps                 | 7.53 ms                                                | 6.53 ms: 1.15x faster                                     |
| chaos                      | 47.4 ms                                                | 41.1 ms: 1.15x faster                                     |
| comprehensions             | 14.4 us                                                | 12.7 us: 1.14x faster                                     |
| async_tree_none            | 282 ms                                                 | 250 ms: 1.12x faster                                      |
| sqlglot_parse              | 890 us                                                 | 792 us: 1.12x faster                                      |
| deltablue                  | 2.75 ms                                                | 2.45 ms: 1.12x faster                                     |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                      |
| async_tree_io_tg           | 724 ms                                                 | 667 ms: 1.09x faster                                      |
| sqlglot_transpile          | 1.05 ms                                                | 973 us: 1.08x faster                                      |
| generators                 | 30.3 ms                                                | 28.2 ms: 1.07x faster                                     |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                      |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.31 sec: 1.06x faster                                    |
| sympy_sum                  | 80.2 ms                                                | 75.6 ms: 1.06x faster                                     |
| richards_super             | 37.3 ms                                                | 35.7 ms: 1.04x faster                                     |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                      |
| async_tree_memoization     | 336 ms                                                 | 328 ms: 1.03x faster                                      |
| regex_dna                  | 148 ms                                                 | 145 ms: 1.02x faster                                      |
| mako                       | 7.93 ms                                                | 7.78 ms: 1.02x faster                                     |
| sympy_integrate            | 11.3 ms                                                | 11.1 ms: 1.02x faster                                     |
| sympy_str                  | 144 ms                                                 | 141 ms: 1.02x faster                                      |
| create_gc_cycles           | 711 us                                                 | 705 us: 1.01x faster                                      |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                      |
| gc_traversal               | 2.38 ms                                                | 2.39 ms: 1.00x slower                                     |
| pidigits                   | 280 ms                                                 | 282 ms: 1.01x slower                                      |
| regex_effbot               | 2.43 ms                                                | 2.46 ms: 1.01x slower                                     |
| logging_simple             | 3.41 us                                                | 3.47 us: 1.02x slower                                     |
| pickle_pure_python         | 191 us                                                 | 195 us: 1.02x slower                                      |
| dask                       | 219 ms                                                 | 223 ms: 1.02x slower                                      |
| deepcopy_memo              | 25.7 us                                                | 26.3 us: 1.02x slower                                     |
| logging_format             | 3.67 us                                                | 3.76 us: 1.02x slower                                     |
| docutils                   | 1.43 sec                                               | 1.47 sec: 1.03x slower                                    |
| crypto_pyaes               | 47.5 ms                                                | 48.8 ms: 1.03x slower                                     |
| richards                   | 31.1 ms                                                | 32.0 ms: 1.03x slower                                     |
| regex_compile              | 72.8 ms                                                | 75.2 ms: 1.03x slower                                     |
| dulwich_log                | 28.6 ms                                                | 29.7 ms: 1.04x slower                                     |
| pickle                     | 6.98 us                                                | 7.27 us: 1.04x slower                                     |
| go                         | 105 ms                                                 | 110 ms: 1.04x slower                                      |
| pathlib                    | 23.2 ms                                                | 24.3 ms: 1.05x slower                                     |
| meteor_contest             | 71.1 ms                                                | 74.5 ms: 1.05x slower                                     |
| pycparser                  | 659 ms                                                 | 692 ms: 1.05x slower                                      |
| sympy_expand               | 229 ms                                                 | 241 ms: 1.05x slower                                      |
| xml_etree_parse            | 100 ms                                                 | 106 ms: 1.05x slower                                      |
| deepcopy                   | 215 us                                                 | 227 us: 1.05x slower                                      |
| logging_silent             | 66.5 ns                                                | 70.5 ns: 1.06x slower                                     |
| unpickle_pure_python       | 149 us                                                 | 158 us: 1.06x slower                                      |
| pickle_dict                | 17.1 us                                                | 18.2 us: 1.07x slower                                     |
| pprint_pformat             | 979 ms                                                 | 1.05 sec: 1.07x slower                                    |
| hexiom                     | 4.58 ms                                                | 4.91 ms: 1.07x slower                                     |
| json                       | 2.75 ms                                                | 2.95 ms: 1.07x slower                                     |
| pprint_safe_repr           | 478 ms                                                 | 513 ms: 1.07x slower                                      |
| coroutines                 | 17.2 ms                                                | 18.5 ms: 1.08x slower                                     |
| coverage                   | 43.9 ms                                                | 47.4 ms: 1.08x slower                                     |
| bench_thread_pool          | 465 us                                                 | 503 us: 1.08x slower                                      |
| mdp                        | 1.48 sec                                               | 1.61 sec: 1.08x slower                                    |
| float                      | 50.8 ms                                                | 55.4 ms: 1.09x slower                                     |
| scimark_lu                 | 67.7 ms                                                | 74.6 ms: 1.10x slower                                     |
| nqueens                    | 55.9 ms                                                | 61.6 ms: 1.10x slower                                     |
| tomli_loads                | 1.27 sec                                               | 1.41 sec: 1.10x slower                                    |
| xml_etree_iterparse        | 68.3 ms                                                | 75.5 ms: 1.11x slower                                     |
| json_loads                 | 15.3 us                                                | 17.0 us: 1.11x slower                                     |
| pickle_list                | 2.70 us                                                | 2.99 us: 1.11x slower                                     |
| fannkuch                   | 240 ms                                                 | 266 ms: 1.11x slower                                      |
| deepcopy_reduce            | 1.79 us                                                | 1.99 us: 1.11x slower                                     |
| unpickle                   | 8.29 us                                                | 9.23 us: 1.11x slower                                     |
| regex_v8                   | 15.1 ms                                                | 16.9 ms: 1.12x slower                                     |
| scimark_monte_carlo        | 43.5 ms                                                | 48.6 ms: 1.12x slower                                     |
| chameleon                  | 4.30 ms                                                | 4.82 ms: 1.12x slower                                     |
| sqlglot_normalize          | 162 ms                                                 | 183 ms: 1.13x slower                                      |
| pyflate                    | 284 ms                                                 | 326 ms: 1.15x slower                                      |
| unpickle_list              | 2.69 us                                                | 3.10 us: 1.15x slower                                     |
| bench_mp_pool              | 41.0 ms                                                | 47.2 ms: 1.15x slower                                     |
| sqlglot_optimize           | 29.6 ms                                                | 34.5 ms: 1.16x slower                                     |
| xml_etree_process          | 33.6 ms                                                | 39.3 ms: 1.17x slower                                     |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.31 ms: 1.18x slower                                     |
| spectral_norm              | 65.7 ms                                                | 79.0 ms: 1.20x slower                                     |
| xml_etree_generate         | 45.8 ms                                                | 55.7 ms: 1.22x slower                                     |
| nbody                      | 61.7 ms                                                | 76.0 ms: 1.23x slower                                     |
| scimark_fft                | 173 ms                                                 | 213 ms: 1.24x slower                                      |
| 2to3                       | 154 ms                                                 | 191 ms: 1.24x slower                                      |
| python_startup             | 10.8 ms                                                | 13.6 ms: 1.27x slower                                     |
| sqlite_synth               | 1.26 us                                                | 1.59 us: 1.27x slower                                     |
| scimark_sor                | 79.2 ms                                                | 105 ms: 1.33x slower                                      |
| python_startup_no_site     | 8.57 ms                                                | 12.2 ms: 1.43x slower                                     |
| telco                      | 3.17 ms                                                | 4.56 ms: 1.44x slower                                     |
| async_generators           | 192 ms                                                 | 304 ms: 1.58x slower                                      |
| mypy2                      | 372 ms                                                 | 592 ms: 1.59x slower                                      |
| Geometric mean             | (ref)                                                  | 1.04x slower                                              |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_io, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.17x