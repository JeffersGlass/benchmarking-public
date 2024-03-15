
# Results vs. 3.12.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: darwin-arm64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 173 ms: 1.02x slower                                                   |
| chameleon      | 4.70 ms                                                | 5.02 ms: 1.07x slower                                                  |
| docutils       | 1.50 sec                                               | 1.51 sec: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 261 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 531 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 538 ms: 1.01x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 682 ms: 1.02x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 333 ms: 1.03x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 268 ms: 1.04x slower                                                   |
| async_tree_io              | 668 ms                                                 | 717 ms: 1.07x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 338 ms: 1.08x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                                   |
| float          | 55.8 ms                                                | 68.6 ms: 1.23x slower                                                  |
| nbody          | 68.8 ms                                                | 85.7 ms: 1.24x slower                                                  |
| Geometric mean | (ref)                                                  | 1.16x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 157 ms: 1.02x slower                                                   |
| regex_compile  | 77.9 ms                                                | 82.6 ms: 1.06x slower                                                  |
| regex_effbot   | 2.64 ms                                                | 2.85 ms: 1.08x slower                                                  |
| regex_v8       | 16.0 ms                                                | 18.1 ms: 1.14x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                   |
| json_loads           | 17.2 us                                                | 17.1 us: 1.01x faster                                                  |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.06 us: 1.01x slower                                                  |
| pickle_list          | 2.89 us                                                | 2.96 us: 1.03x slower                                                  |
| pickle               | 7.23 us                                                | 7.45 us: 1.03x slower                                                  |
| xml_etree_process    | 39.7 ms                                                | 41.0 ms: 1.03x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.61 ms: 1.06x slower                                                  |
| xml_etree_generate   | 55.8 ms                                                | 59.5 ms: 1.06x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 80.5 ms: 1.09x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 164 us: 1.09x slower                                                   |
| tomli_loads          | 1.39 sec                                               | 1.67 sec: 1.20x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (2): unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.6 ms: 1.11x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.2 ms: 1.19x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 9.74 ms: 1.26x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 73.6 us: 1.26x faster                                                  |
| raytrace                   | 212 ms                                                 | 186 ms: 1.14x faster                                                   |
| unpack_sequence            | 31.5 ns                                                | 28.5 ns: 1.11x faster                                                  |
| generators                 | 31.1 ms                                                | 28.7 ms: 1.08x faster                                                  |
| logging_silent             | 76.4 ns                                                | 71.1 ns: 1.08x faster                                                  |
| sqlglot_parse              | 848 us                                                 | 811 us: 1.05x faster                                                   |
| deepcopy_memo              | 27.7 us                                                | 26.7 us: 1.04x faster                                                  |
| logging_format             | 3.98 us                                                | 3.85 us: 1.03x faster                                                  |
| deepcopy_reduce            | 2.07 us                                                | 2.00 us: 1.03x faster                                                  |
| logging_simple             | 3.69 us                                                | 3.56 us: 1.03x faster                                                  |
| deepcopy                   | 235 us                                                 | 227 us: 1.03x faster                                                   |
| json                       | 3.09 ms                                                | 2.99 ms: 1.03x faster                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 995 us: 1.03x faster                                                   |
| coroutines                 | 19.2 ms                                                | 18.8 ms: 1.02x faster                                                  |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                                   |
| async_tree_none            | 266 ms                                                 | 261 ms: 1.02x faster                                                   |
| async_generators           | 304 ms                                                 | 300 ms: 1.01x faster                                                   |
| json_loads                 | 17.2 us                                                | 17.1 us: 1.01x faster                                                  |
| gc_traversal               | 2.40 ms                                                | 2.40 ms: 1.00x slower                                                  |
| pickle_dict                | 18.1 us                                                | 18.1 us: 1.00x slower                                                  |
| docutils                   | 1.50 sec                                               | 1.51 sec: 1.01x slower                                                 |
| pidigits                   | 282 ms                                                 | 284 ms: 1.01x slower                                                   |
| sympy_str                  | 148 ms                                                 | 149 ms: 1.01x slower                                                   |
| scimark_lu                 | 76.0 ms                                                | 76.7 ms: 1.01x slower                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 531 ms: 1.01x slower                                                   |
| create_gc_cycles           | 701 us                                                 | 708 us: 1.01x slower                                                   |
| dulwich_log                | 29.8 ms                                                | 30.1 ms: 1.01x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 538 ms: 1.01x slower                                                   |
| unpickle_list              | 3.02 us                                                | 3.06 us: 1.01x slower                                                  |
| richards_super             | 36.0 ms                                                | 36.5 ms: 1.01x slower                                                  |
| richards                   | 32.1 ms                                                | 32.6 ms: 1.01x slower                                                  |
| sympy_integrate            | 11.4 ms                                                | 11.6 ms: 1.02x slower                                                  |
| sympy_expand               | 241 ms                                                 | 245 ms: 1.02x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 682 ms: 1.02x slower                                                   |
| regex_dna                  | 154 ms                                                 | 157 ms: 1.02x slower                                                   |
| 2to3                       | 169 ms                                                 | 173 ms: 1.02x slower                                                   |
| mdp                        | 1.58 sec                                               | 1.62 sec: 1.02x slower                                                 |
| sympy_sum                  | 77.6 ms                                                | 79.6 ms: 1.02x slower                                                  |
| sqlglot_normalize          | 186 ms                                                 | 190 ms: 1.03x slower                                                   |
| bench_thread_pool          | 504 us                                                 | 518 us: 1.03x slower                                                   |
| pickle_list                | 2.89 us                                                | 2.96 us: 1.03x slower                                                  |
| pickle                     | 7.23 us                                                | 7.45 us: 1.03x slower                                                  |
| dask                       | 222 ms                                                 | 229 ms: 1.03x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 333 ms: 1.03x slower                                                   |
| xml_etree_process          | 39.7 ms                                                | 41.0 ms: 1.03x slower                                                  |
| pycparser                  | 677 ms                                                 | 702 ms: 1.04x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 268 ms: 1.04x slower                                                   |
| sqlite_synth               | 1.57 us                                                | 1.65 us: 1.05x slower                                                  |
| pathlib                    | 24.2 ms                                                | 25.5 ms: 1.05x slower                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 35.9 ms: 1.06x slower                                                  |
| crypto_pyaes               | 51.9 ms                                                | 54.9 ms: 1.06x slower                                                  |
| regex_compile              | 77.9 ms                                                | 82.6 ms: 1.06x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.32 sec: 1.06x slower                                                 |
| json_dumps                 | 6.22 ms                                                | 6.61 ms: 1.06x slower                                                  |
| xml_etree_generate         | 55.8 ms                                                | 59.5 ms: 1.06x slower                                                  |
| comprehensions             | 14.5 us                                                | 15.5 us: 1.07x slower                                                  |
| chameleon                  | 4.70 ms                                                | 5.02 ms: 1.07x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 76.8 ms: 1.07x slower                                                  |
| async_tree_io              | 668 ms                                                 | 717 ms: 1.07x slower                                                   |
| regex_effbot               | 2.64 ms                                                | 2.85 ms: 1.08x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 338 ms: 1.08x slower                                                   |
| xml_etree_iterparse        | 74.0 ms                                                | 80.5 ms: 1.09x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 164 us: 1.09x slower                                                   |
| nqueens                    | 62.4 ms                                                | 68.1 ms: 1.09x slower                                                  |
| chaos                      | 42.5 ms                                                | 46.5 ms: 1.09x slower                                                  |
| go                         | 102 ms                                                 | 111 ms: 1.10x slower                                                   |
| python_startup             | 11.4 ms                                                | 12.6 ms: 1.11x slower                                                  |
| regex_v8                   | 16.0 ms                                                | 18.1 ms: 1.14x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 572 ms: 1.15x slower                                                   |
| pprint_pformat             | 1.01 sec                                               | 1.17 sec: 1.16x slower                                                 |
| pyflate                    | 316 ms                                                 | 371 ms: 1.18x slower                                                   |
| python_startup_no_site     | 9.37 ms                                                | 11.2 ms: 1.19x slower                                                  |
| tomli_loads                | 1.39 sec                                               | 1.67 sec: 1.20x slower                                                 |
| scimark_sor                | 87.4 ms                                                | 107 ms: 1.22x slower                                                   |
| float                      | 55.8 ms                                                | 68.6 ms: 1.23x slower                                                  |
| coverage                   | 38.9 ms                                                | 48.2 ms: 1.24x slower                                                  |
| nbody                      | 68.8 ms                                                | 85.7 ms: 1.24x slower                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 56.5 ms: 1.26x slower                                                  |
| mako                       | 7.71 ms                                                | 9.74 ms: 1.26x slower                                                  |
| scimark_fft                | 195 ms                                                 | 247 ms: 1.27x slower                                                   |
| telco                      | 3.68 ms                                                | 4.69 ms: 1.27x slower                                                  |
| hexiom                     | 4.54 ms                                                | 5.95 ms: 1.31x slower                                                  |
| fannkuch                   | 248 ms                                                 | 326 ms: 1.31x slower                                                   |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 4.12 ms: 1.31x slower                                                  |
| deltablue                  | 2.71 ms                                                | 3.59 ms: 1.33x slower                                                  |
| spectral_norm              | 76.4 ms                                                | 105 ms: 1.38x slower                                                   |
| mypy2                      | 380 ms                                                 | 531 ms: 1.40x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.06x slower                                                           |

Benchmark hidden because not significant (6): asyncio_tcp, bench_mp_pool, unpickle, asyncio_websockets, tornado_http, xml_etree_parse
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.00x