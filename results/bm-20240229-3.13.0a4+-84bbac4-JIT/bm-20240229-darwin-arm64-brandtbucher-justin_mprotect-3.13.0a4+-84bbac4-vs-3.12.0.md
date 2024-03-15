# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: darwin-arm64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.05x slower \*
- HPT reliability: 99.80%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.82x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 205 ms: 1.21x slower                                                    |
| chameleon      | 4.70 ms                                                | 4.87 ms: 1.04x slower                                                   |
| docutils       | 1.50 sec                                               | 1.53 sec: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                                            |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 252 ms: 1.06x faster                                                    |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 519 ms: 1.01x faster                                                    |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 529 ms: 1.01x faster                                                    |
| async_tree_io_tg           | 669 ms                                                 | 667 ms: 1.00x faster                                                    |
| async_tree_memoization     | 312 ms                                                 | 327 ms: 1.05x slower                                                    |
| async_tree_io              | 668 ms                                                 | 700 ms: 1.05x slower                                                    |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                            |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.0 ms: 1.05x faster                                                   |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                    |
| nbody          | 68.8 ms                                                | 70.3 ms: 1.02x slower                                                   |
| Geometric mean | (ref)                                                  | 1.01x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                    |
| regex_effbot   | 2.64 ms                                                | 2.65 ms: 1.01x slower                                                   |
| regex_v8       | 16.0 ms                                                | 17.3 ms: 1.08x slower                                                   |
| regex_compile  | 77.9 ms                                                | 86.8 ms: 1.12x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                    |
| json_loads           | 17.2 us                                                | 17.0 us: 1.01x faster                                                   |
| xml_etree_generate   | 55.8 ms                                                | 55.7 ms: 1.00x faster                                                   |
| unpickle_pure_python | 151 us                                                 | 151 us: 1.00x slower                                                    |
| unpickle_list        | 3.02 us                                                | 3.05 us: 1.01x slower                                                   |
| pickle_dict          | 18.1 us                                                | 18.2 us: 1.01x slower                                                   |
| unpickle             | 9.12 us                                                | 9.21 us: 1.01x slower                                                   |
| pickle               | 7.23 us                                                | 7.32 us: 1.01x slower                                                   |
| pickle_list          | 2.89 us                                                | 2.94 us: 1.02x slower                                                   |
| json_dumps           | 6.22 ms                                                | 6.49 ms: 1.04x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                            |

Benchmark hidden because not significant (4): xml_etree_process, tomli_loads, xml_etree_parse, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 17.9 ms: 1.57x slower                                                   |
| python_startup_no_site | 9.37 ms                                                | 16.3 ms: 1.74x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.65x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 6.80 ms: 1.13x faster                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 71.5 us: 1.30x faster                                                   |
| comprehensions             | 14.5 us                                                | 12.8 us: 1.13x faster                                                   |
| mako                       | 7.71 ms                                                | 6.80 ms: 1.13x faster                                                   |
| raytrace                   | 212 ms                                                 | 191 ms: 1.11x faster                                                    |
| generators                 | 31.1 ms                                                | 28.3 ms: 1.10x faster                                                   |
| crypto_pyaes               | 51.9 ms                                                | 48.1 ms: 1.08x faster                                                   |
| asyncio_tcp                | 449 ms                                                 | 420 ms: 1.07x faster                                                    |
| deltablue                  | 2.71 ms                                                | 2.55 ms: 1.06x faster                                                   |
| logging_silent             | 76.4 ns                                                | 72.2 ns: 1.06x faster                                                   |
| async_tree_none            | 266 ms                                                 | 252 ms: 1.06x faster                                                    |
| coroutines                 | 19.2 ms                                                | 18.3 ms: 1.05x faster                                                   |
| deepcopy_memo              | 27.7 us                                                | 26.3 us: 1.05x faster                                                   |
| logging_simple             | 3.69 us                                                | 3.50 us: 1.05x faster                                                   |
| float                      | 55.8 ms                                                | 53.0 ms: 1.05x faster                                                   |
| logging_format             | 3.98 us                                                | 3.79 us: 1.05x faster                                                   |
| chaos                      | 42.5 ms                                                | 40.5 ms: 1.05x faster                                                   |
| json                       | 3.09 ms                                                | 2.96 ms: 1.04x faster                                                   |
| deepcopy_reduce            | 2.07 us                                                | 2.00 us: 1.04x faster                                                   |
| sympy_str                  | 148 ms                                                 | 144 ms: 1.02x faster                                                    |
| deepcopy                   | 235 us                                                 | 230 us: 1.02x faster                                                    |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                                    |
| sympy_sum                  | 77.6 ms                                                | 76.3 ms: 1.02x faster                                                   |
| regex_dna                  | 154 ms                                                 | 152 ms: 1.02x faster                                                    |
| sqlglot_normalize          | 186 ms                                                 | 183 ms: 1.01x faster                                                    |
| json_loads                 | 17.2 us                                                | 17.0 us: 1.01x faster                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 519 ms: 1.01x faster                                                    |
| sqlglot_parse              | 848 us                                                 | 840 us: 1.01x faster                                                    |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 529 ms: 1.01x faster                                                    |
| async_tree_io_tg           | 669 ms                                                 | 667 ms: 1.00x faster                                                    |
| xml_etree_generate         | 55.8 ms                                                | 55.7 ms: 1.00x faster                                                   |
| gc_traversal               | 2.40 ms                                                | 2.41 ms: 1.00x slower                                                   |
| sqlglot_transpile          | 1.02 ms                                                | 1.02 ms: 1.00x slower                                                   |
| unpickle_pure_python       | 151 us                                                 | 151 us: 1.00x slower                                                    |
| pidigits                   | 282 ms                                                 | 283 ms: 1.00x slower                                                    |
| regex_effbot               | 2.64 ms                                                | 2.65 ms: 1.01x slower                                                   |
| sqlite_synth               | 1.57 us                                                | 1.58 us: 1.01x slower                                                   |
| unpickle_list              | 3.02 us                                                | 3.05 us: 1.01x slower                                                   |
| sympy_integrate            | 11.4 ms                                                | 11.5 ms: 1.01x slower                                                   |
| pickle_dict                | 18.1 us                                                | 18.2 us: 1.01x slower                                                   |
| unpickle                   | 9.12 us                                                | 9.21 us: 1.01x slower                                                   |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.17 ms: 1.01x slower                                                   |
| pickle                     | 7.23 us                                                | 7.32 us: 1.01x slower                                                   |
| bench_thread_pool          | 504 us                                                 | 511 us: 1.01x slower                                                    |
| create_gc_cycles           | 701 us                                                 | 712 us: 1.02x slower                                                    |
| pickle_list                | 2.89 us                                                | 2.94 us: 1.02x slower                                                   |
| docutils                   | 1.50 sec                                               | 1.53 sec: 1.02x slower                                                  |
| sympy_expand               | 241 ms                                                 | 246 ms: 1.02x slower                                                    |
| async_generators           | 304 ms                                                 | 310 ms: 1.02x slower                                                    |
| nbody                      | 68.8 ms                                                | 70.3 ms: 1.02x slower                                                   |
| scimark_monte_carlo        | 45.0 ms                                                | 46.0 ms: 1.02x slower                                                   |
| scimark_fft                | 195 ms                                                 | 200 ms: 1.03x slower                                                    |
| nqueens                    | 62.4 ms                                                | 64.1 ms: 1.03x slower                                                   |
| mdp                        | 1.58 sec                                               | 1.63 sec: 1.03x slower                                                  |
| dulwich_log                | 29.8 ms                                                | 30.9 ms: 1.04x slower                                                   |
| chameleon                  | 4.70 ms                                                | 4.87 ms: 1.04x slower                                                   |
| spectral_norm              | 76.4 ms                                                | 79.3 ms: 1.04x slower                                                   |
| pprint_safe_repr           | 497 ms                                                 | 517 ms: 1.04x slower                                                    |
| json_dumps                 | 6.22 ms                                                | 6.49 ms: 1.04x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 327 ms: 1.05x slower                                                    |
| meteor_contest             | 71.7 ms                                                | 75.0 ms: 1.05x slower                                                   |
| sqlglot_optimize           | 34.0 ms                                                | 35.6 ms: 1.05x slower                                                   |
| async_tree_io              | 668 ms                                                 | 700 ms: 1.05x slower                                                    |
| pprint_pformat             | 1.01 sec                                               | 1.06 sec: 1.05x slower                                                  |
| pathlib                    | 24.2 ms                                                | 25.5 ms: 1.05x slower                                                   |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.31 sec: 1.06x slower                                                  |
| pycparser                  | 677 ms                                                 | 726 ms: 1.07x slower                                                    |
| regex_v8                   | 16.0 ms                                                | 17.3 ms: 1.08x slower                                                   |
| pyflate                    | 316 ms                                                 | 350 ms: 1.11x slower                                                    |
| regex_compile              | 77.9 ms                                                | 86.8 ms: 1.12x slower                                                   |
| scimark_lu                 | 76.0 ms                                                | 85.7 ms: 1.13x slower                                                   |
| go                         | 102 ms                                                 | 116 ms: 1.15x slower                                                    |
| hexiom                     | 4.54 ms                                                | 5.31 ms: 1.17x slower                                                   |
| bench_mp_pool              | 44.9 ms                                                | 52.6 ms: 1.17x slower                                                   |
| 2to3                       | 169 ms                                                 | 205 ms: 1.21x slower                                                    |
| fannkuch                   | 248 ms                                                 | 305 ms: 1.23x slower                                                    |
| coverage                   | 38.9 ms                                                | 47.6 ms: 1.23x slower                                                   |
| richards_super             | 36.0 ms                                                | 44.2 ms: 1.23x slower                                                   |
| telco                      | 3.68 ms                                                | 4.60 ms: 1.25x slower                                                   |
| richards                   | 32.1 ms                                                | 40.5 ms: 1.26x slower                                                   |
| scimark_sor                | 87.4 ms                                                | 113 ms: 1.29x slower                                                    |
| dask                       | 222 ms                                                 | 332 ms: 1.49x slower                                                    |
| python_startup             | 11.4 ms                                                | 17.9 ms: 1.57x slower                                                   |
| mypy2                      | 380 ms                                                 | 596 ms: 1.57x slower                                                    |
| python_startup_no_site     | 9.37 ms                                                | 16.3 ms: 1.74x slower                                                   |
| unpack_sequence            | 31.5 ns                                                | 113 ns: 3.60x slower                                                    |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                            |

Benchmark hidden because not significant (8): xml_etree_process, tomli_loads, xml_etree_parse, async_tree_memoization_tg, asyncio_websockets, async_tree_none_tg, xml_etree_iterparse, tornado_http
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.80% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.82x