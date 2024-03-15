
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 185 ms: 1.20x slower                                                 |
| chameleon      | 4.30 ms                                                | 4.89 ms: 1.14x slower                                                |
| docutils       | 1.43 sec                                               | 1.51 sec: 1.06x slower                                               |
| Geometric mean | (ref)                                                  | 1.10x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                                 |
| async_tree_io_tg           | 724 ms                                                 | 668 ms: 1.08x faster                                                 |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                 |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                                 |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                         |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.01x slower                                                 |
| float          | 50.8 ms                                                | 53.2 ms: 1.05x slower                                                |
| nbody          | 61.7 ms                                                | 69.9 ms: 1.13x slower                                                |
| Geometric mean | (ref)                                                  | 1.06x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.02x slower                                                 |
| regex_effbot   | 2.43 ms                                                | 2.56 ms: 1.05x slower                                                |
| regex_v8       | 15.1 ms                                                | 17.1 ms: 1.13x slower                                                |
| regex_compile  | 72.8 ms                                                | 84.7 ms: 1.16x slower                                                |
| Geometric mean | (ref)                                                  | 1.09x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.50 ms: 1.16x faster                                                |
| unpickle_pure_python | 149 us                                                 | 149 us: 1.00x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 197 us: 1.03x slower                                                 |
| pickle               | 6.98 us                                                | 7.24 us: 1.04x slower                                                |
| xml_etree_parse      | 100 ms                                                 | 106 ms: 1.06x slower                                                 |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                                |
| tomli_loads          | 1.27 sec                                               | 1.37 sec: 1.07x slower                                               |
| xml_etree_iterparse  | 68.3 ms                                                | 74.7 ms: 1.09x slower                                                |
| unpickle             | 8.29 us                                                | 9.09 us: 1.10x slower                                                |
| pickle_list          | 2.70 us                                                | 2.98 us: 1.10x slower                                                |
| json_loads           | 15.3 us                                                | 17.1 us: 1.11x slower                                                |
| unpickle_list        | 2.69 us                                                | 3.04 us: 1.13x slower                                                |
| xml_etree_process    | 33.6 ms                                                | 38.9 ms: 1.16x slower                                                |
| xml_etree_generate   | 45.8 ms                                                | 55.6 ms: 1.21x slower                                                |
| Geometric mean       | (ref)                                                  | 1.07x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 18.0 ms: 1.67x slower                                                |
| python_startup_no_site | 8.57 ms                                                | 16.5 ms: 1.92x slower                                                |
| Geometric mean         | (ref)                                                  | 1.79x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 6.85 ms: 1.16x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-darwin-arm64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 71.7 us: 4.20x faster                                                |
| asyncio_tcp                | 643 ms                                                 | 413 ms: 1.56x faster                                                 |
| chaos                      | 47.4 ms                                                | 40.2 ms: 1.18x faster                                                |
| json_dumps                 | 7.53 ms                                                | 6.50 ms: 1.16x faster                                                |
| mako                       | 7.93 ms                                                | 6.85 ms: 1.16x faster                                                |
| comprehensions             | 14.4 us                                                | 12.6 us: 1.15x faster                                                |
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                                 |
| async_tree_io_tg           | 724 ms                                                 | 668 ms: 1.08x faster                                                 |
| deltablue                  | 2.75 ms                                                | 2.55 ms: 1.08x faster                                                |
| raytrace                   | 206 ms                                                 | 191 ms: 1.08x faster                                                 |
| sqlglot_parse              | 890 us                                                 | 827 us: 1.08x faster                                                 |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.30 sec: 1.07x faster                                               |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                 |
| generators                 | 30.3 ms                                                | 28.6 ms: 1.06x faster                                                |
| sympy_sum                  | 80.2 ms                                                | 76.6 ms: 1.05x faster                                                |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 1.01 ms: 1.04x faster                                                |
| unpickle_pure_python       | 149 us                                                 | 149 us: 1.00x slower                                                 |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                 |
| pidigits                   | 280 ms                                                 | 282 ms: 1.01x slower                                                 |
| crypto_pyaes               | 47.5 ms                                                | 47.8 ms: 1.01x slower                                                |
| sympy_integrate            | 11.3 ms                                                | 11.5 ms: 1.02x slower                                                |
| create_gc_cycles           | 711 us                                                 | 723 us: 1.02x slower                                                 |
| gc_traversal               | 2.38 ms                                                | 2.43 ms: 1.02x slower                                                |
| deepcopy_memo              | 25.7 us                                                | 26.3 us: 1.02x slower                                                |
| logging_simple             | 3.41 us                                                | 3.49 us: 1.02x slower                                                |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.02x slower                                                 |
| pickle_pure_python         | 191 us                                                 | 197 us: 1.03x slower                                                 |
| logging_format             | 3.67 us                                                | 3.78 us: 1.03x slower                                                |
| pickle                     | 6.98 us                                                | 7.24 us: 1.04x slower                                                |
| meteor_contest             | 71.1 ms                                                | 74.0 ms: 1.04x slower                                                |
| float                      | 50.8 ms                                                | 53.2 ms: 1.05x slower                                                |
| deepcopy                   | 215 us                                                 | 226 us: 1.05x slower                                                 |
| pathlib                    | 23.2 ms                                                | 24.4 ms: 1.05x slower                                                |
| regex_effbot               | 2.43 ms                                                | 2.56 ms: 1.05x slower                                                |
| xml_etree_parse            | 100 ms                                                 | 106 ms: 1.06x slower                                                 |
| docutils                   | 1.43 sec                                               | 1.51 sec: 1.06x slower                                               |
| scimark_monte_carlo        | 43.5 ms                                                | 46.1 ms: 1.06x slower                                                |
| pickle_dict                | 17.1 us                                                | 18.1 us: 1.06x slower                                                |
| logging_silent             | 66.5 ns                                                | 70.7 ns: 1.06x slower                                                |
| dulwich_log                | 28.6 ms                                                | 30.6 ms: 1.07x slower                                                |
| pprint_safe_repr           | 478 ms                                                 | 512 ms: 1.07x slower                                                 |
| json                       | 2.75 ms                                                | 2.95 ms: 1.07x slower                                                |
| tomli_loads                | 1.27 sec                                               | 1.37 sec: 1.07x slower                                               |
| sympy_expand               | 229 ms                                                 | 246 ms: 1.07x slower                                                 |
| pprint_pformat             | 979 ms                                                 | 1.05 sec: 1.07x slower                                               |
| coroutines                 | 17.2 ms                                                | 18.5 ms: 1.08x slower                                                |
| go                         | 105 ms                                                 | 115 ms: 1.09x slower                                                 |
| coverage                   | 43.9 ms                                                | 47.9 ms: 1.09x slower                                                |
| xml_etree_iterparse        | 68.3 ms                                                | 74.7 ms: 1.09x slower                                                |
| unpickle                   | 8.29 us                                                | 9.09 us: 1.10x slower                                                |
| mdp                        | 1.48 sec                                               | 1.63 sec: 1.10x slower                                               |
| pickle_list                | 2.70 us                                                | 2.98 us: 1.10x slower                                                |
| pycparser                  | 659 ms                                                 | 732 ms: 1.11x slower                                                 |
| deepcopy_reduce            | 1.79 us                                                | 1.99 us: 1.11x slower                                                |
| bench_thread_pool          | 465 us                                                 | 517 us: 1.11x slower                                                 |
| json_loads                 | 15.3 us                                                | 17.1 us: 1.11x slower                                                |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.13 ms: 1.11x slower                                                |
| spectral_norm              | 65.7 ms                                                | 74.0 ms: 1.13x slower                                                |
| regex_v8                   | 15.1 ms                                                | 17.1 ms: 1.13x slower                                                |
| nbody                      | 61.7 ms                                                | 69.9 ms: 1.13x slower                                                |
| unpickle_list              | 2.69 us                                                | 3.04 us: 1.13x slower                                                |
| chameleon                  | 4.30 ms                                                | 4.89 ms: 1.14x slower                                                |
| sqlglot_normalize          | 162 ms                                                 | 184 ms: 1.14x slower                                                 |
| hexiom                     | 4.58 ms                                                | 5.27 ms: 1.15x slower                                                |
| nqueens                    | 55.9 ms                                                | 64.5 ms: 1.15x slower                                                |
| scimark_fft                | 173 ms                                                 | 200 ms: 1.16x slower                                                 |
| xml_etree_process          | 33.6 ms                                                | 38.9 ms: 1.16x slower                                                |
| richards_super             | 37.3 ms                                                | 43.3 ms: 1.16x slower                                                |
| regex_compile              | 72.8 ms                                                | 84.7 ms: 1.16x slower                                                |
| pyflate                    | 284 ms                                                 | 339 ms: 1.19x slower                                                 |
| sqlglot_optimize           | 29.6 ms                                                | 35.5 ms: 1.20x slower                                                |
| 2to3                       | 154 ms                                                 | 185 ms: 1.20x slower                                                 |
| xml_etree_generate         | 45.8 ms                                                | 55.6 ms: 1.21x slower                                                |
| sqlite_synth               | 1.26 us                                                | 1.59 us: 1.26x slower                                                |
| richards                   | 31.1 ms                                                | 39.4 ms: 1.27x slower                                                |
| scimark_lu                 | 67.7 ms                                                | 86.7 ms: 1.28x slower                                                |
| fannkuch                   | 240 ms                                                 | 311 ms: 1.30x slower                                                 |
| bench_mp_pool              | 41.0 ms                                                | 53.3 ms: 1.30x slower                                                |
| telco                      | 3.17 ms                                                | 4.55 ms: 1.44x slower                                                |
| scimark_sor                | 79.2 ms                                                | 116 ms: 1.47x slower                                                 |
| async_generators           | 192 ms                                                 | 310 ms: 1.61x slower                                                 |
| mypy2                      | 372 ms                                                 | 603 ms: 1.62x slower                                                 |
| python_startup             | 10.8 ms                                                | 18.0 ms: 1.67x slower                                                |
| python_startup_no_site     | 8.57 ms                                                | 16.5 ms: 1.92x slower                                                |
| unpack_sequence            | 33.6 ns                                                | 115 ns: 3.41x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                         |

Benchmark hidden because not significant (5): async_tree_memoization, sympy_str, asyncio_websockets, async_tree_cpu_io_mixed, tornado_http
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.90x