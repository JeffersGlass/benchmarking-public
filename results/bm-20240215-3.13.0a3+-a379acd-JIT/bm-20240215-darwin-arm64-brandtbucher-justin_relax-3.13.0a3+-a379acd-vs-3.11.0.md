
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: a379acd
- commit date: 2024-02-15
- overall geometric mean: 1.03x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.18x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 193 ms: 1.25x slower                                                 |
| chameleon      | 4.30 ms                                                | 4.79 ms: 1.11x slower                                                |
| docutils       | 1.43 sec                                               | 1.46 sec: 1.02x slower                                               |
| Geometric mean | (ref)                                                  | 1.10x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 249 ms: 1.13x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 319 ms: 1.11x faster                                                 |
| async_tree_io_tg           | 724 ms                                                 | 658 ms: 1.10x faster                                                 |
| async_tree_none_tg         | 276 ms                                                 | 256 ms: 1.08x faster                                                 |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 527 ms: 1.04x faster                                                 |
| async_tree_memoization     | 336 ms                                                 | 325 ms: 1.04x faster                                                 |
| async_tree_io              | 697 ms                                                 | 692 ms: 1.01x faster                                                 |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                         |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.01x slower                                                 |
| float          | 50.8 ms                                                | 53.1 ms: 1.04x slower                                                |
| nbody          | 61.7 ms                                                | 71.3 ms: 1.16x slower                                                |
| Geometric mean | (ref)                                                  | 1.07x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 72.8 ms                                                | 73.7 ms: 1.01x slower                                                |
| regex_dna      | 148 ms                                                 | 151 ms: 1.02x slower                                                 |
| regex_effbot   | 2.43 ms                                                | 2.55 ms: 1.05x slower                                                |
| regex_v8       | 15.1 ms                                                | 17.0 ms: 1.12x slower                                                |
| Geometric mean | (ref)                                                  | 1.05x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.44 ms: 1.17x faster                                                |
| pickle_pure_python   | 191 us                                                 | 195 us: 1.02x slower                                                 |
| pickle               | 6.98 us                                                | 7.25 us: 1.04x slower                                                |
| xml_etree_parse      | 100 ms                                                 | 106 ms: 1.05x slower                                                 |
| tomli_loads          | 1.27 sec                                               | 1.34 sec: 1.05x slower                                               |
| unpickle_pure_python | 149 us                                                 | 157 us: 1.06x slower                                                 |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                                |
| xml_etree_iterparse  | 68.3 ms                                                | 73.6 ms: 1.08x slower                                                |
| pickle_list          | 2.70 us                                                | 2.95 us: 1.09x slower                                                |
| unpickle             | 8.29 us                                                | 9.15 us: 1.10x slower                                                |
| json_loads           | 15.3 us                                                | 17.1 us: 1.11x slower                                                |
| unpickle_list        | 2.69 us                                                | 3.07 us: 1.14x slower                                                |
| xml_etree_process    | 33.6 ms                                                | 38.3 ms: 1.14x slower                                                |
| xml_etree_generate   | 45.8 ms                                                | 54.9 ms: 1.20x slower                                                |
| Geometric mean       | (ref)                                                  | 1.07x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.5 ms: 1.26x slower                                                |
| python_startup_no_site | 8.57 ms                                                | 12.2 ms: 1.42x slower                                                |
| Geometric mean         | (ref)                                                  | 1.34x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 6.98 ms: 1.14x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 70.0 us: 4.30x faster                                                |
| asyncio_tcp                | 643 ms                                                 | 394 ms: 1.63x faster                                                 |
| comprehensions             | 14.4 us                                                | 12.0 us: 1.20x faster                                                |
| unpack_sequence            | 33.6 ns                                                | 28.4 ns: 1.18x faster                                                |
| chaos                      | 47.4 ms                                                | 40.0 ms: 1.18x faster                                                |
| raytrace                   | 206 ms                                                 | 174 ms: 1.18x faster                                                 |
| json_dumps                 | 7.53 ms                                                | 6.44 ms: 1.17x faster                                                |
| mako                       | 7.93 ms                                                | 6.98 ms: 1.14x faster                                                |
| sqlglot_parse              | 890 us                                                 | 785 us: 1.13x faster                                                 |
| deltablue                  | 2.75 ms                                                | 2.43 ms: 1.13x faster                                                |
| async_tree_none            | 282 ms                                                 | 249 ms: 1.13x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 319 ms: 1.11x faster                                                 |
| async_tree_io_tg           | 724 ms                                                 | 658 ms: 1.10x faster                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 970 us: 1.08x faster                                                 |
| async_tree_none_tg         | 276 ms                                                 | 256 ms: 1.08x faster                                                 |
| generators                 | 30.3 ms                                                | 28.2 ms: 1.07x faster                                                |
| sympy_sum                  | 80.2 ms                                                | 75.0 ms: 1.07x faster                                                |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.31 sec: 1.06x faster                                               |
| richards_super             | 37.3 ms                                                | 35.4 ms: 1.05x faster                                                |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 527 ms: 1.04x faster                                                 |
| async_tree_memoization     | 336 ms                                                 | 325 ms: 1.04x faster                                                 |
| sympy_str                  | 144 ms                                                 | 141 ms: 1.02x faster                                                 |
| create_gc_cycles           | 711 us                                                 | 703 us: 1.01x faster                                                 |
| sympy_integrate            | 11.3 ms                                                | 11.2 ms: 1.01x faster                                                |
| async_tree_io              | 697 ms                                                 | 692 ms: 1.01x faster                                                 |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                                 |
| gc_traversal               | 2.38 ms                                                | 2.39 ms: 1.00x slower                                                |
| pidigits                   | 280 ms                                                 | 282 ms: 1.01x slower                                                 |
| logging_simple             | 3.41 us                                                | 3.43 us: 1.01x slower                                                |
| regex_compile              | 72.8 ms                                                | 73.7 ms: 1.01x slower                                                |
| pickle_pure_python         | 191 us                                                 | 195 us: 1.02x slower                                                 |
| richards                   | 31.1 ms                                                | 31.7 ms: 1.02x slower                                                |
| logging_format             | 3.67 us                                                | 3.75 us: 1.02x slower                                                |
| regex_dna                  | 148 ms                                                 | 151 ms: 1.02x slower                                                 |
| go                         | 105 ms                                                 | 108 ms: 1.02x slower                                                 |
| docutils                   | 1.43 sec                                               | 1.46 sec: 1.02x slower                                               |
| dask                       | 219 ms                                                 | 226 ms: 1.03x slower                                                 |
| dulwich_log                | 28.6 ms                                                | 29.6 ms: 1.04x slower                                                |
| meteor_contest             | 71.1 ms                                                | 73.6 ms: 1.04x slower                                                |
| pickle                     | 6.98 us                                                | 7.25 us: 1.04x slower                                                |
| pycparser                  | 659 ms                                                 | 688 ms: 1.04x slower                                                 |
| float                      | 50.8 ms                                                | 53.1 ms: 1.04x slower                                                |
| deepcopy                   | 215 us                                                 | 225 us: 1.05x slower                                                 |
| hexiom                     | 4.58 ms                                                | 4.79 ms: 1.05x slower                                                |
| pprint_pformat             | 979 ms                                                 | 1.02 sec: 1.05x slower                                               |
| sympy_expand               | 229 ms                                                 | 240 ms: 1.05x slower                                                 |
| pathlib                    | 23.2 ms                                                | 24.3 ms: 1.05x slower                                                |
| regex_effbot               | 2.43 ms                                                | 2.55 ms: 1.05x slower                                                |
| xml_etree_parse            | 100 ms                                                 | 106 ms: 1.05x slower                                                 |
| tomli_loads                | 1.27 sec                                               | 1.34 sec: 1.05x slower                                               |
| unpickle_pure_python       | 149 us                                                 | 157 us: 1.06x slower                                                 |
| logging_silent             | 66.5 ns                                                | 70.3 ns: 1.06x slower                                                |
| pprint_safe_repr           | 478 ms                                                 | 507 ms: 1.06x slower                                                 |
| pickle_dict                | 17.1 us                                                | 18.1 us: 1.06x slower                                                |
| json                       | 2.75 ms                                                | 2.94 ms: 1.07x slower                                                |
| xml_etree_iterparse        | 68.3 ms                                                | 73.6 ms: 1.08x slower                                                |
| mdp                        | 1.48 sec                                               | 1.61 sec: 1.08x slower                                               |
| bench_thread_pool          | 465 us                                                 | 504 us: 1.08x slower                                                 |
| scimark_monte_carlo        | 43.5 ms                                                | 47.3 ms: 1.09x slower                                                |
| coverage                   | 43.9 ms                                                | 47.9 ms: 1.09x slower                                                |
| pickle_list                | 2.70 us                                                | 2.95 us: 1.09x slower                                                |
| nqueens                    | 55.9 ms                                                | 61.1 ms: 1.09x slower                                                |
| fannkuch                   | 240 ms                                                 | 263 ms: 1.10x slower                                                 |
| coroutines                 | 17.2 ms                                                | 18.9 ms: 1.10x slower                                                |
| scimark_lu                 | 67.7 ms                                                | 74.5 ms: 1.10x slower                                                |
| unpickle                   | 8.29 us                                                | 9.15 us: 1.10x slower                                                |
| deepcopy_reduce            | 1.79 us                                                | 1.99 us: 1.11x slower                                                |
| json_loads                 | 15.3 us                                                | 17.1 us: 1.11x slower                                                |
| pyflate                    | 284 ms                                                 | 316 ms: 1.11x slower                                                 |
| chameleon                  | 4.30 ms                                                | 4.79 ms: 1.11x slower                                                |
| sqlglot_normalize          | 162 ms                                                 | 181 ms: 1.12x slower                                                 |
| regex_v8                   | 15.1 ms                                                | 17.0 ms: 1.12x slower                                                |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.17 ms: 1.13x slower                                                |
| unpickle_list              | 2.69 us                                                | 3.07 us: 1.14x slower                                                |
| xml_etree_process          | 33.6 ms                                                | 38.3 ms: 1.14x slower                                                |
| bench_mp_pool              | 41.0 ms                                                | 47.0 ms: 1.15x slower                                                |
| sqlglot_optimize           | 29.6 ms                                                | 34.2 ms: 1.15x slower                                                |
| nbody                      | 61.7 ms                                                | 71.3 ms: 1.16x slower                                                |
| spectral_norm              | 65.7 ms                                                | 77.1 ms: 1.17x slower                                                |
| scimark_fft                | 173 ms                                                 | 205 ms: 1.19x slower                                                 |
| xml_etree_generate         | 45.8 ms                                                | 54.9 ms: 1.20x slower                                                |
| 2to3                       | 154 ms                                                 | 193 ms: 1.25x slower                                                 |
| python_startup             | 10.8 ms                                                | 13.5 ms: 1.26x slower                                                |
| sqlite_synth               | 1.26 us                                                | 1.59 us: 1.26x slower                                                |
| scimark_sor                | 79.2 ms                                                | 105 ms: 1.33x slower                                                 |
| telco                      | 3.17 ms                                                | 4.43 ms: 1.40x slower                                                |
| python_startup_no_site     | 8.57 ms                                                | 12.2 ms: 1.42x slower                                                |
| async_generators           | 192 ms                                                 | 304 ms: 1.58x slower                                                 |
| mypy2                      | 372 ms                                                 | 590 ms: 1.58x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                         |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed, deepcopy_memo, crypto_pyaes, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.18x