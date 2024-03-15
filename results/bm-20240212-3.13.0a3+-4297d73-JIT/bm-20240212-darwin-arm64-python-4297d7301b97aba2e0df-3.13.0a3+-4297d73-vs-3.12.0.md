
# Results vs. 3.12.0

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: darwin-arm64
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.01x slower \*
- HPT reliability: 81.25%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.14x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 174 ms: 1.03x slower                                                   |
| chameleon      | 4.70 ms                                                | 4.82 ms: 1.03x slower                                                  |
| docutils       | 1.50 sec                                               | 1.47 sec: 1.02x faster                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 251 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 517 ms: 1.02x faster                                                   |
| async_tree_io_tg           | 669 ms                                                 | 661 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 528 ms: 1.01x faster                                                   |
| async_tree_io              | 668 ms                                                 | 696 ms: 1.04x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 326 ms: 1.04x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 55.6 ms: 1.00x faster                                                  |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| nbody          | 68.8 ms                                                | 76.6 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.56 ms: 1.03x faster                                                  |
| regex_compile  | 77.9 ms                                                | 75.5 ms: 1.03x faster                                                  |
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                   |
| regex_v8       | 16.0 ms                                                | 17.0 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| xml_etree_process    | 39.7 ms                                                | 38.7 ms: 1.03x faster                                                  |
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                   |
| json_loads           | 17.2 us                                                | 17.0 us: 1.02x faster                                                  |
| xml_etree_generate   | 55.8 ms                                                | 55.2 ms: 1.01x faster                                                  |
| unpickle             | 9.12 us                                                | 9.16 us: 1.00x slower                                                  |
| pickle_dict          | 18.1 us                                                | 18.2 us: 1.01x slower                                                  |
| tomli_loads          | 1.39 sec                                               | 1.41 sec: 1.01x slower                                                 |
| pickle               | 7.23 us                                                | 7.32 us: 1.01x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 75.7 ms: 1.02x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.09 us: 1.02x slower                                                  |
| pickle_list          | 2.89 us                                                | 2.98 us: 1.03x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.47 ms: 1.04x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 159 us: 1.06x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.3 ms: 1.17x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.9 ms: 1.27x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.22x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.80 ms: 1.01x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 70.7 us: 1.32x faster                                                  |
| raytrace                   | 212 ms                                                 | 177 ms: 1.20x faster                                                   |
| comprehensions             | 14.5 us                                                | 12.6 us: 1.15x faster                                                  |
| unpack_sequence            | 31.5 ns                                                | 28.5 ns: 1.11x faster                                                  |
| generators                 | 31.1 ms                                                | 28.2 ms: 1.10x faster                                                  |
| deltablue                  | 2.71 ms                                                | 2.46 ms: 1.10x faster                                                  |
| logging_silent             | 76.4 ns                                                | 70.5 ns: 1.08x faster                                                  |
| logging_simple             | 3.69 us                                                | 3.45 us: 1.07x faster                                                  |
| sqlglot_parse              | 848 us                                                 | 795 us: 1.07x faster                                                   |
| async_tree_none            | 266 ms                                                 | 251 ms: 1.06x faster                                                   |
| deepcopy_memo              | 27.7 us                                                | 26.1 us: 1.06x faster                                                  |
| crypto_pyaes               | 51.9 ms                                                | 49.1 ms: 1.06x faster                                                  |
| logging_format             | 3.98 us                                                | 3.78 us: 1.05x faster                                                  |
| deepcopy                   | 235 us                                                 | 224 us: 1.05x faster                                                   |
| json                       | 3.09 ms                                                | 2.95 ms: 1.05x faster                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 979 us: 1.04x faster                                                   |
| coroutines                 | 19.2 ms                                                | 18.5 ms: 1.04x faster                                                  |
| deepcopy_reduce            | 2.07 us                                                | 2.00 us: 1.03x faster                                                  |
| regex_effbot               | 2.64 ms                                                | 2.56 ms: 1.03x faster                                                  |
| regex_compile              | 77.9 ms                                                | 75.5 ms: 1.03x faster                                                  |
| sympy_str                  | 148 ms                                                 | 143 ms: 1.03x faster                                                   |
| sympy_sum                  | 77.6 ms                                                | 75.5 ms: 1.03x faster                                                  |
| chaos                      | 42.5 ms                                                | 41.5 ms: 1.03x faster                                                  |
| xml_etree_process          | 39.7 ms                                                | 38.7 ms: 1.03x faster                                                  |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                                   |
| docutils                   | 1.50 sec                                               | 1.47 sec: 1.02x faster                                                 |
| regex_dna                  | 154 ms                                                 | 152 ms: 1.02x faster                                                   |
| json_loads                 | 17.2 us                                                | 17.0 us: 1.02x faster                                                  |
| scimark_lu                 | 76.0 ms                                                | 74.8 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 517 ms: 1.02x faster                                                   |
| sqlglot_normalize          | 186 ms                                                 | 183 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 669 ms                                                 | 661 ms: 1.01x faster                                                   |
| xml_etree_generate         | 55.8 ms                                                | 55.2 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 528 ms: 1.01x faster                                                   |
| richards_super             | 36.0 ms                                                | 35.8 ms: 1.01x faster                                                  |
| async_generators           | 304 ms                                                 | 302 ms: 1.01x faster                                                   |
| sympy_integrate            | 11.4 ms                                                | 11.3 ms: 1.01x faster                                                  |
| nqueens                    | 62.4 ms                                                | 62.1 ms: 1.01x faster                                                  |
| richards                   | 32.1 ms                                                | 32.0 ms: 1.00x faster                                                  |
| gc_traversal               | 2.40 ms                                                | 2.39 ms: 1.00x faster                                                  |
| dulwich_log                | 29.8 ms                                                | 29.7 ms: 1.00x faster                                                  |
| float                      | 55.8 ms                                                | 55.6 ms: 1.00x faster                                                  |
| pidigits                   | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| unpickle                   | 9.12 us                                                | 9.16 us: 1.00x slower                                                  |
| create_gc_cycles           | 701 us                                                 | 706 us: 1.01x slower                                                   |
| sympy_expand               | 241 ms                                                 | 243 ms: 1.01x slower                                                   |
| pickle_dict                | 18.1 us                                                | 18.2 us: 1.01x slower                                                  |
| mako                       | 7.71 ms                                                | 7.80 ms: 1.01x slower                                                  |
| tomli_loads                | 1.39 sec                                               | 1.41 sec: 1.01x slower                                                 |
| pickle                     | 7.23 us                                                | 7.32 us: 1.01x slower                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 34.5 ms: 1.01x slower                                                  |
| dask                       | 222 ms                                                 | 225 ms: 1.01x slower                                                   |
| xml_etree_iterparse        | 74.0 ms                                                | 75.7 ms: 1.02x slower                                                  |
| unpickle_list              | 3.02 us                                                | 3.09 us: 1.02x slower                                                  |
| chameleon                  | 4.70 ms                                                | 4.82 ms: 1.03x slower                                                  |
| pycparser                  | 677 ms                                                 | 695 ms: 1.03x slower                                                   |
| 2to3                       | 169 ms                                                 | 174 ms: 1.03x slower                                                   |
| mdp                        | 1.58 sec                                               | 1.63 sec: 1.03x slower                                                 |
| sqlite_synth               | 1.57 us                                                | 1.62 us: 1.03x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 513 ms: 1.03x slower                                                   |
| pickle_list                | 2.89 us                                                | 2.98 us: 1.03x slower                                                  |
| pyflate                    | 316 ms                                                 | 327 ms: 1.03x slower                                                   |
| pprint_pformat             | 1.01 sec                                               | 1.05 sec: 1.04x slower                                                 |
| json_dumps                 | 6.22 ms                                                | 6.47 ms: 1.04x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 74.7 ms: 1.04x slower                                                  |
| async_tree_io              | 668 ms                                                 | 696 ms: 1.04x slower                                                   |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.30 sec: 1.04x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 326 ms: 1.04x slower                                                   |
| bench_mp_pool              | 44.9 ms                                                | 47.0 ms: 1.05x slower                                                  |
| spectral_norm              | 76.4 ms                                                | 80.6 ms: 1.06x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 159 us: 1.06x slower                                                   |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.33 ms: 1.06x slower                                                  |
| regex_v8                   | 16.0 ms                                                | 17.0 ms: 1.07x slower                                                  |
| go                         | 102 ms                                                 | 109 ms: 1.08x slower                                                   |
| scimark_monte_carlo        | 45.0 ms                                                | 48.8 ms: 1.08x slower                                                  |
| hexiom                     | 4.54 ms                                                | 5.01 ms: 1.10x slower                                                  |
| fannkuch                   | 248 ms                                                 | 275 ms: 1.11x slower                                                   |
| nbody                      | 68.8 ms                                                | 76.6 ms: 1.11x slower                                                  |
| scimark_fft                | 195 ms                                                 | 218 ms: 1.12x slower                                                   |
| python_startup             | 11.4 ms                                                | 13.3 ms: 1.17x slower                                                  |
| scimark_sor                | 87.4 ms                                                | 106 ms: 1.21x slower                                                   |
| coverage                   | 38.9 ms                                                | 47.2 ms: 1.22x slower                                                  |
| telco                      | 3.68 ms                                                | 4.59 ms: 1.25x slower                                                  |
| python_startup_no_site     | 9.37 ms                                                | 11.9 ms: 1.27x slower                                                  |
| mypy2                      | 380 ms                                                 | 525 ms: 1.38x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (8): asyncio_tcp, async_tree_memoization_tg, xml_etree_parse, bench_thread_pool, asyncio_websockets, async_tree_none_tg, pathlib, tornado_http
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 81.25% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.14x