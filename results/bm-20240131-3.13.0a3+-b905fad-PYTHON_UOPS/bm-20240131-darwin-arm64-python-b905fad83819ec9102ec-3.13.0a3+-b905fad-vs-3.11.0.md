
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 174 ms: 1.13x slower                                                   |
| chameleon      | 4.30 ms                                                | 4.95 ms: 1.15x slower                                                  |
| docutils       | 1.43 sec                                               | 1.50 sec: 1.05x slower                                                 |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 258 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 676 ms: 1.07x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 330 ms: 1.07x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 535 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 525 ms: 1.01x slower                                                   |
| async_tree_io              | 697 ms                                                 | 706 ms: 1.01x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 68.3 ms: 1.34x slower                                                  |
| nbody          | 61.7 ms                                                | 85.3 ms: 1.38x slower                                                  |
| Geometric mean | (ref)                                                  | 1.23x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.02x slower                                                   |
| regex_effbot   | 2.43 ms                                                | 2.56 ms: 1.05x slower                                                  |
| regex_compile  | 72.8 ms                                                | 81.7 ms: 1.12x slower                                                  |
| regex_v8       | 15.1 ms                                                | 17.1 ms: 1.13x slower                                                  |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.57 ms: 1.15x faster                                                  |
| pickle_pure_python   | 191 us                                                 | 198 us: 1.03x slower                                                   |
| pickle               | 6.98 us                                                | 7.22 us: 1.04x slower                                                  |
| pickle_dict          | 17.1 us                                                | 18.2 us: 1.07x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| unpickle_pure_python | 149 us                                                 | 163 us: 1.10x slower                                                   |
| unpickle             | 8.29 us                                                | 9.11 us: 1.10x slower                                                  |
| json_loads           | 15.3 us                                                | 17.0 us: 1.11x slower                                                  |
| pickle_list          | 2.70 us                                                | 2.99 us: 1.11x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.08 us: 1.15x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 80.5 ms: 1.18x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 41.0 ms: 1.22x slower                                                  |
| xml_etree_generate   | 45.8 ms                                                | 58.8 ms: 1.28x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.64 sec: 1.29x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.2 ms: 1.22x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.8 ms: 1.38x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 9.66 ms: 1.22x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 73.2 us: 4.11x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 427 ms: 1.50x faster                                                   |
| unpack_sequence            | 33.6 ns                                                | 29.1 ns: 1.16x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.57 ms: 1.15x faster                                                  |
| raytrace                   | 206 ms                                                 | 185 ms: 1.11x faster                                                   |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.27 sec: 1.10x faster                                                 |
| sqlglot_parse              | 890 us                                                 | 813 us: 1.09x faster                                                   |
| async_tree_none            | 282 ms                                                 | 258 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 676 ms: 1.07x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 330 ms: 1.07x faster                                                   |
| generators                 | 30.3 ms                                                | 28.7 ms: 1.05x faster                                                  |
| sqlglot_transpile          | 1.05 ms                                                | 998 us: 1.05x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                   |
| chaos                      | 47.4 ms                                                | 45.9 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 535 ms: 1.03x faster                                                   |
| sympy_sum                  | 80.2 ms                                                | 79.1 ms: 1.01x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 704 us: 1.01x faster                                                   |
| richards_super             | 37.3 ms                                                | 37.0 ms: 1.01x faster                                                  |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                  |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 525 ms: 1.01x slower                                                   |
| async_tree_io              | 697 ms                                                 | 706 ms: 1.01x slower                                                   |
| sympy_integrate            | 11.3 ms                                                | 11.5 ms: 1.02x slower                                                  |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.02x slower                                                   |
| dask                       | 219 ms                                                 | 224 ms: 1.02x slower                                                   |
| sympy_str                  | 144 ms                                                 | 147 ms: 1.03x slower                                                   |
| pickle_pure_python         | 191 us                                                 | 198 us: 1.03x slower                                                   |
| pickle                     | 6.98 us                                                | 7.22 us: 1.04x slower                                                  |
| deepcopy_memo              | 25.7 us                                                | 26.7 us: 1.04x slower                                                  |
| logging_simple             | 3.41 us                                                | 3.56 us: 1.04x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.50 sec: 1.05x slower                                                 |
| go                         | 105 ms                                                 | 111 ms: 1.05x slower                                                   |
| dulwich_log                | 28.6 ms                                                | 30.1 ms: 1.05x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.56 ms: 1.05x slower                                                  |
| deepcopy                   | 215 us                                                 | 227 us: 1.05x slower                                                   |
| comprehensions             | 14.4 us                                                | 15.2 us: 1.05x slower                                                  |
| logging_format             | 3.67 us                                                | 3.88 us: 1.06x slower                                                  |
| pathlib                    | 23.2 ms                                                | 24.6 ms: 1.06x slower                                                  |
| richards                   | 31.1 ms                                                | 33.0 ms: 1.06x slower                                                  |
| sympy_expand               | 229 ms                                                 | 244 ms: 1.06x slower                                                   |
| pycparser                  | 659 ms                                                 | 702 ms: 1.06x slower                                                   |
| pickle_dict                | 17.1 us                                                | 18.2 us: 1.07x slower                                                  |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| json                       | 2.75 ms                                                | 2.94 ms: 1.07x slower                                                  |
| logging_silent             | 66.5 ns                                                | 71.3 ns: 1.07x slower                                                  |
| coverage                   | 43.9 ms                                                | 47.1 ms: 1.07x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 77.2 ms: 1.09x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.62 sec: 1.09x slower                                                 |
| unpickle_pure_python       | 149 us                                                 | 163 us: 1.10x slower                                                   |
| bench_thread_pool          | 465 us                                                 | 511 us: 1.10x slower                                                   |
| unpickle                   | 8.29 us                                                | 9.11 us: 1.10x slower                                                  |
| json_loads                 | 15.3 us                                                | 17.0 us: 1.11x slower                                                  |
| bench_mp_pool              | 41.0 ms                                                | 45.5 ms: 1.11x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.99 us: 1.11x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.00 us: 1.12x slower                                                  |
| regex_compile              | 72.8 ms                                                | 81.7 ms: 1.12x slower                                                  |
| 2to3                       | 154 ms                                                 | 174 ms: 1.13x slower                                                   |
| regex_v8                   | 15.1 ms                                                | 17.1 ms: 1.13x slower                                                  |
| scimark_lu                 | 67.7 ms                                                | 76.8 ms: 1.13x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 54.0 ms: 1.14x slower                                                  |
| coroutines                 | 17.2 ms                                                | 19.7 ms: 1.15x slower                                                  |
| unpickle_list              | 2.69 us                                                | 3.08 us: 1.15x slower                                                  |
| chameleon                  | 4.30 ms                                                | 4.95 ms: 1.15x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 190 ms: 1.18x slower                                                   |
| xml_etree_iterparse        | 68.3 ms                                                | 80.5 ms: 1.18x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 568 ms: 1.19x slower                                                   |
| pprint_pformat             | 979 ms                                                 | 1.16 sec: 1.19x slower                                                 |
| sqlglot_optimize           | 29.6 ms                                                | 35.8 ms: 1.21x slower                                                  |
| nqueens                    | 55.9 ms                                                | 67.9 ms: 1.21x slower                                                  |
| mako                       | 7.93 ms                                                | 9.66 ms: 1.22x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 41.0 ms: 1.22x slower                                                  |
| python_startup             | 10.8 ms                                                | 13.2 ms: 1.22x slower                                                  |
| hexiom                     | 4.58 ms                                                | 5.85 ms: 1.28x slower                                                  |
| deltablue                  | 2.75 ms                                                | 3.53 ms: 1.28x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 58.8 ms: 1.28x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 56.0 ms: 1.29x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.64 sec: 1.29x slower                                                 |
| pyflate                    | 284 ms                                                 | 366 ms: 1.29x slower                                                   |
| sqlite_synth               | 1.26 us                                                | 1.64 us: 1.31x slower                                                  |
| fannkuch                   | 240 ms                                                 | 319 ms: 1.33x slower                                                   |
| scimark_sor                | 79.2 ms                                                | 106 ms: 1.34x slower                                                   |
| float                      | 50.8 ms                                                | 68.3 ms: 1.34x slower                                                  |
| python_startup_no_site     | 8.57 ms                                                | 11.8 ms: 1.38x slower                                                  |
| nbody                      | 61.7 ms                                                | 85.3 ms: 1.38x slower                                                  |
| mypy2                      | 372 ms                                                 | 524 ms: 1.41x slower                                                   |
| scimark_fft                | 173 ms                                                 | 244 ms: 1.41x slower                                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 4.09 ms: 1.45x slower                                                  |
| telco                      | 3.17 ms                                                | 4.70 ms: 1.48x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 101 ms: 1.54x slower                                                   |
| async_generators           | 192 ms                                                 | 297 ms: 1.55x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                           |

Benchmark hidden because not significant (3): async_tree_memoization, asyncio_websockets, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 1.03x