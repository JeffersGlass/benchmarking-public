# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: darwin-arm64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.89x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 205 ms: 1.33x slower                                                    |
| chameleon      | 4.30 ms                                                | 4.87 ms: 1.13x slower                                                   |
| docutils       | 1.43 sec                                               | 1.53 sec: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.13x slower                                                            |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                    |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                                    |
| async_tree_io_tg           | 724 ms                                                 | 667 ms: 1.09x faster                                                    |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                    |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                                    |
| async_tree_memoization     | 336 ms                                                 | 327 ms: 1.03x faster                                                    |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                            |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                                    |
| float          | 50.8 ms                                                | 53.0 ms: 1.04x slower                                                   |
| nbody          | 61.7 ms                                                | 70.3 ms: 1.14x slower                                                   |
| Geometric mean | (ref)                                                  | 1.06x slower                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.03x slower                                                    |
| regex_effbot   | 2.43 ms                                                | 2.65 ms: 1.09x slower                                                   |
| regex_v8       | 15.1 ms                                                | 17.3 ms: 1.14x slower                                                   |
| regex_compile  | 72.8 ms                                                | 86.8 ms: 1.19x slower                                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.49 ms: 1.16x faster                                                   |
| unpickle_pure_python | 149 us                                                 | 151 us: 1.02x slower                                                    |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.02x slower                                                    |
| pickle               | 6.98 us                                                | 7.32 us: 1.05x slower                                                   |
| xml_etree_parse      | 100 ms                                                 | 106 ms: 1.06x slower                                                    |
| pickle_dict          | 17.1 us                                                | 18.2 us: 1.07x slower                                                   |
| tomli_loads          | 1.27 sec                                               | 1.38 sec: 1.09x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 74.3 ms: 1.09x slower                                                   |
| pickle_list          | 2.70 us                                                | 2.94 us: 1.09x slower                                                   |
| json_loads           | 15.3 us                                                | 17.0 us: 1.11x slower                                                   |
| unpickle             | 8.29 us                                                | 9.21 us: 1.11x slower                                                   |
| unpickle_list        | 2.69 us                                                | 3.05 us: 1.13x slower                                                   |
| xml_etree_process    | 33.6 ms                                                | 39.3 ms: 1.17x slower                                                   |
| xml_etree_generate   | 45.8 ms                                                | 55.7 ms: 1.21x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.07x slower                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 17.9 ms: 1.66x slower                                                   |
| python_startup_no_site | 8.57 ms                                                | 16.3 ms: 1.90x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.78x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 6.80 ms: 1.17x faster                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 71.5 us: 4.21x faster                                                   |
| asyncio_tcp                | 643 ms                                                 | 420 ms: 1.53x faster                                                    |
| chaos                      | 47.4 ms                                                | 40.5 ms: 1.17x faster                                                   |
| mako                       | 7.93 ms                                                | 6.80 ms: 1.17x faster                                                   |
| json_dumps                 | 7.53 ms                                                | 6.49 ms: 1.16x faster                                                   |
| comprehensions             | 14.4 us                                                | 12.8 us: 1.13x faster                                                   |
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                    |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                                    |
| async_tree_io_tg           | 724 ms                                                 | 667 ms: 1.09x faster                                                    |
| deltablue                  | 2.75 ms                                                | 2.55 ms: 1.08x faster                                                   |
| raytrace                   | 206 ms                                                 | 191 ms: 1.07x faster                                                    |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                    |
| generators                 | 30.3 ms                                                | 28.3 ms: 1.07x faster                                                   |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.31 sec: 1.06x faster                                                  |
| sqlglot_parse              | 890 us                                                 | 840 us: 1.06x faster                                                    |
| sympy_sum                  | 80.2 ms                                                | 76.3 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                                    |
| async_tree_memoization     | 336 ms                                                 | 327 ms: 1.03x faster                                                    |
| sqlglot_transpile          | 1.05 ms                                                | 1.02 ms: 1.03x faster                                                   |
| create_gc_cycles           | 711 us                                                 | 712 us: 1.00x slower                                                    |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                                    |
| sympy_str                  | 144 ms                                                 | 144 ms: 1.00x slower                                                    |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                                    |
| gc_traversal               | 2.38 ms                                                | 2.41 ms: 1.01x slower                                                   |
| crypto_pyaes               | 47.5 ms                                                | 48.1 ms: 1.01x slower                                                   |
| unpickle_pure_python       | 149 us                                                 | 151 us: 1.02x slower                                                    |
| sympy_integrate            | 11.3 ms                                                | 11.5 ms: 1.02x slower                                                   |
| deepcopy_memo              | 25.7 us                                                | 26.3 us: 1.02x slower                                                   |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.02x slower                                                    |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.03x slower                                                    |
| logging_simple             | 3.41 us                                                | 3.50 us: 1.03x slower                                                   |
| logging_format             | 3.67 us                                                | 3.79 us: 1.03x slower                                                   |
| float                      | 50.8 ms                                                | 53.0 ms: 1.04x slower                                                   |
| pickle                     | 6.98 us                                                | 7.32 us: 1.05x slower                                                   |
| xml_etree_parse            | 100 ms                                                 | 106 ms: 1.06x slower                                                    |
| meteor_contest             | 71.1 ms                                                | 75.0 ms: 1.06x slower                                                   |
| scimark_monte_carlo        | 43.5 ms                                                | 46.0 ms: 1.06x slower                                                   |
| coroutines                 | 17.2 ms                                                | 18.3 ms: 1.06x slower                                                   |
| deepcopy                   | 215 us                                                 | 230 us: 1.07x slower                                                    |
| pickle_dict                | 17.1 us                                                | 18.2 us: 1.07x slower                                                   |
| docutils                   | 1.43 sec                                               | 1.53 sec: 1.07x slower                                                  |
| sympy_expand               | 229 ms                                                 | 246 ms: 1.07x slower                                                    |
| json                       | 2.75 ms                                                | 2.96 ms: 1.08x slower                                                   |
| pprint_safe_repr           | 478 ms                                                 | 517 ms: 1.08x slower                                                    |
| dulwich_log                | 28.6 ms                                                | 30.9 ms: 1.08x slower                                                   |
| pprint_pformat             | 979 ms                                                 | 1.06 sec: 1.08x slower                                                  |
| logging_silent             | 66.5 ns                                                | 72.2 ns: 1.08x slower                                                   |
| coverage                   | 43.9 ms                                                | 47.6 ms: 1.09x slower                                                   |
| tomli_loads                | 1.27 sec                                               | 1.38 sec: 1.09x slower                                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 74.3 ms: 1.09x slower                                                   |
| pickle_list                | 2.70 us                                                | 2.94 us: 1.09x slower                                                   |
| regex_effbot               | 2.43 ms                                                | 2.65 ms: 1.09x slower                                                   |
| mdp                        | 1.48 sec                                               | 1.63 sec: 1.10x slower                                                  |
| bench_thread_pool          | 465 us                                                 | 511 us: 1.10x slower                                                    |
| pathlib                    | 23.2 ms                                                | 25.5 ms: 1.10x slower                                                   |
| pycparser                  | 659 ms                                                 | 726 ms: 1.10x slower                                                    |
| go                         | 105 ms                                                 | 116 ms: 1.10x slower                                                    |
| json_loads                 | 15.3 us                                                | 17.0 us: 1.11x slower                                                   |
| unpickle                   | 8.29 us                                                | 9.21 us: 1.11x slower                                                   |
| deepcopy_reduce            | 1.79 us                                                | 2.00 us: 1.11x slower                                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.17 ms: 1.13x slower                                                   |
| sqlglot_normalize          | 162 ms                                                 | 183 ms: 1.13x slower                                                    |
| chameleon                  | 4.30 ms                                                | 4.87 ms: 1.13x slower                                                   |
| unpickle_list              | 2.69 us                                                | 3.05 us: 1.13x slower                                                   |
| regex_v8                   | 15.1 ms                                                | 17.3 ms: 1.14x slower                                                   |
| nbody                      | 61.7 ms                                                | 70.3 ms: 1.14x slower                                                   |
| nqueens                    | 55.9 ms                                                | 64.1 ms: 1.15x slower                                                   |
| scimark_fft                | 173 ms                                                 | 200 ms: 1.16x slower                                                    |
| hexiom                     | 4.58 ms                                                | 5.31 ms: 1.16x slower                                                   |
| xml_etree_process          | 33.6 ms                                                | 39.3 ms: 1.17x slower                                                   |
| richards_super             | 37.3 ms                                                | 44.2 ms: 1.19x slower                                                   |
| regex_compile              | 72.8 ms                                                | 86.8 ms: 1.19x slower                                                   |
| sqlglot_optimize           | 29.6 ms                                                | 35.6 ms: 1.20x slower                                                   |
| spectral_norm              | 65.7 ms                                                | 79.3 ms: 1.21x slower                                                   |
| xml_etree_generate         | 45.8 ms                                                | 55.7 ms: 1.21x slower                                                   |
| pyflate                    | 284 ms                                                 | 350 ms: 1.23x slower                                                    |
| sqlite_synth               | 1.26 us                                                | 1.58 us: 1.26x slower                                                   |
| scimark_lu                 | 67.7 ms                                                | 85.7 ms: 1.26x slower                                                   |
| fannkuch                   | 240 ms                                                 | 305 ms: 1.27x slower                                                    |
| bench_mp_pool              | 41.0 ms                                                | 52.6 ms: 1.28x slower                                                   |
| richards                   | 31.1 ms                                                | 40.5 ms: 1.30x slower                                                   |
| 2to3                       | 154 ms                                                 | 205 ms: 1.33x slower                                                    |
| scimark_sor                | 79.2 ms                                                | 113 ms: 1.43x slower                                                    |
| telco                      | 3.17 ms                                                | 4.60 ms: 1.45x slower                                                   |
| dask                       | 219 ms                                                 | 332 ms: 1.52x slower                                                    |
| mypy2                      | 372 ms                                                 | 596 ms: 1.60x slower                                                    |
| async_generators           | 192 ms                                                 | 310 ms: 1.62x slower                                                    |
| python_startup             | 10.8 ms                                                | 17.9 ms: 1.66x slower                                                   |
| python_startup_no_site     | 8.57 ms                                                | 16.3 ms: 1.90x slower                                                   |
| unpack_sequence            | 33.6 ns                                                | 113 ns: 3.37x slower                                                    |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                            |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_io, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.89x