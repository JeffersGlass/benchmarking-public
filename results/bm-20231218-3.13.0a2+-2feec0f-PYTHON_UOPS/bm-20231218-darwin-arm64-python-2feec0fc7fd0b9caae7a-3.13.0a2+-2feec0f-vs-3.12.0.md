
# Results vs. 3.12.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: darwin-arm64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.15x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 196 ms: 1.15x slower                                                   |
| chameleon      | 4.70 ms                                                | 5.51 ms: 1.17x slower                                                  |
| docutils       | 1.50 sec                                               | 1.67 sec: 1.11x slower                                                 |
| tornado_http   | 69.3 ms                                                | 83.4 ms: 1.20x slower                                                  |
| Geometric mean | (ref)                                                  | 1.16x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 279 ms: 1.05x slower                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 564 ms: 1.07x slower                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 574 ms: 1.08x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 735 ms: 1.10x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 360 ms: 1.12x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 289 ms: 1.12x slower                                                   |
| async_tree_io              | 668 ms                                                 | 767 ms: 1.15x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 360 ms: 1.15x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 294 ms: 1.04x slower                                                   |
| float          | 55.8 ms                                                | 74.2 ms: 1.33x slower                                                  |
| nbody          | 68.8 ms                                                | 92.7 ms: 1.35x slower                                                  |
| Geometric mean | (ref)                                                  | 1.23x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 161 ms: 1.04x slower                                                   |
| regex_effbot   | 2.64 ms                                                | 2.84 ms: 1.08x slower                                                  |
| regex_compile  | 77.9 ms                                                | 89.4 ms: 1.15x slower                                                  |
| regex_v8       | 16.0 ms                                                | 18.4 ms: 1.16x slower                                                  |
| Geometric mean | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_dict          | 18.1 us                                                | 18.6 us: 1.03x slower                                                  |
| json_loads           | 17.2 us                                                | 17.9 us: 1.04x slower                                                  |
| unpickle             | 9.12 us                                                | 9.49 us: 1.04x slower                                                  |
| pickle_list          | 2.89 us                                                | 3.04 us: 1.05x slower                                                  |
| pickle_pure_python   | 200 us                                                 | 212 us: 1.06x slower                                                   |
| xml_etree_parse      | 106 ms                                                 | 113 ms: 1.06x slower                                                   |
| pickle               | 7.23 us                                                | 7.67 us: 1.06x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.27 us: 1.08x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.97 ms: 1.12x slower                                                  |
| xml_etree_process    | 39.7 ms                                                | 44.4 ms: 1.12x slower                                                  |
| xml_etree_generate   | 55.8 ms                                                | 64.3 ms: 1.15x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 86.0 ms: 1.16x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 180 us: 1.20x slower                                                   |
| tomli_loads          | 1.39 sec                                               | 1.76 sec: 1.26x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 15.6 ms: 1.36x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 14.0 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.43x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 10.5 ms: 1.36x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| generators                 | 31.1 ms                                                | 26.6 ms: 1.17x faster                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 80.6 us: 1.15x faster                                                  |
| unpack_sequence            | 31.5 ns                                                | 29.8 ns: 1.06x faster                                                  |
| raytrace                   | 212 ms                                                 | 203 ms: 1.05x faster                                                   |
| coroutines                 | 19.2 ms                                                | 19.4 ms: 1.01x slower                                                  |
| logging_silent             | 76.4 ns                                                | 77.5 ns: 1.01x slower                                                  |
| json                       | 3.09 ms                                                | 3.16 ms: 1.02x slower                                                  |
| deepcopy_memo              | 27.7 us                                                | 28.4 us: 1.03x slower                                                  |
| pickle_dict                | 18.1 us                                                | 18.6 us: 1.03x slower                                                  |
| json_loads                 | 17.2 us                                                | 17.9 us: 1.04x slower                                                  |
| regex_dna                  | 154 ms                                                 | 161 ms: 1.04x slower                                                   |
| unpickle                   | 9.12 us                                                | 9.49 us: 1.04x slower                                                  |
| pidigits                   | 282 ms                                                 | 294 ms: 1.04x slower                                                   |
| async_tree_none            | 266 ms                                                 | 279 ms: 1.05x slower                                                   |
| deepcopy                   | 235 us                                                 | 247 us: 1.05x slower                                                   |
| pickle_list                | 2.89 us                                                | 3.04 us: 1.05x slower                                                  |
| create_gc_cycles           | 701 us                                                 | 740 us: 1.05x slower                                                   |
| logging_simple             | 3.69 us                                                | 3.89 us: 1.06x slower                                                  |
| logging_format             | 3.98 us                                                | 4.22 us: 1.06x slower                                                  |
| deepcopy_reduce            | 2.07 us                                                | 2.19 us: 1.06x slower                                                  |
| pickle_pure_python         | 200 us                                                 | 212 us: 1.06x slower                                                   |
| async_generators           | 304 ms                                                 | 322 ms: 1.06x slower                                                   |
| xml_etree_parse            | 106 ms                                                 | 113 ms: 1.06x slower                                                   |
| pickle                     | 7.23 us                                                | 7.67 us: 1.06x slower                                                  |
| gc_traversal               | 2.40 ms                                                | 2.56 ms: 1.07x slower                                                  |
| asyncio_websockets         | 409 ms                                                 | 437 ms: 1.07x slower                                                   |
| scimark_lu                 | 76.0 ms                                                | 81.4 ms: 1.07x slower                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 564 ms: 1.07x slower                                                   |
| dulwich_log                | 29.8 ms                                                | 32.0 ms: 1.07x slower                                                  |
| regex_effbot               | 2.64 ms                                                | 2.84 ms: 1.08x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 574 ms: 1.08x slower                                                   |
| unpickle_list              | 3.02 us                                                | 3.27 us: 1.08x slower                                                  |
| sqlglot_parse              | 848 us                                                 | 924 us: 1.09x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 735 ms: 1.10x slower                                                   |
| crypto_pyaes               | 51.9 ms                                                | 57.3 ms: 1.10x slower                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 1.13 ms: 1.11x slower                                                  |
| richards_super             | 36.0 ms                                                | 39.9 ms: 1.11x slower                                                  |
| docutils                   | 1.50 sec                                               | 1.67 sec: 1.11x slower                                                 |
| richards                   | 32.1 ms                                                | 35.9 ms: 1.12x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 360 ms: 1.12x slower                                                   |
| json_dumps                 | 6.22 ms                                                | 6.97 ms: 1.12x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 289 ms: 1.12x slower                                                   |
| xml_etree_process          | 39.7 ms                                                | 44.4 ms: 1.12x slower                                                  |
| sympy_integrate            | 11.4 ms                                                | 12.8 ms: 1.13x slower                                                  |
| sympy_str                  | 148 ms                                                 | 167 ms: 1.13x slower                                                   |
| sympy_sum                  | 77.6 ms                                                | 87.7 ms: 1.13x slower                                                  |
| pathlib                    | 24.2 ms                                                | 27.5 ms: 1.13x slower                                                  |
| pycparser                  | 677 ms                                                 | 769 ms: 1.14x slower                                                   |
| dask                       | 222 ms                                                 | 252 ms: 1.14x slower                                                   |
| sympy_expand               | 241 ms                                                 | 274 ms: 1.14x slower                                                   |
| sqlite_synth               | 1.57 us                                                | 1.78 us: 1.14x slower                                                  |
| sqlglot_normalize          | 186 ms                                                 | 211 ms: 1.14x slower                                                   |
| async_tree_io              | 668 ms                                                 | 767 ms: 1.15x slower                                                   |
| regex_compile              | 77.9 ms                                                | 89.4 ms: 1.15x slower                                                  |
| bench_mp_pool              | 44.9 ms                                                | 51.6 ms: 1.15x slower                                                  |
| xml_etree_generate         | 55.8 ms                                                | 64.3 ms: 1.15x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 360 ms: 1.15x slower                                                   |
| 2to3                       | 169 ms                                                 | 196 ms: 1.15x slower                                                   |
| regex_v8                   | 16.0 ms                                                | 18.4 ms: 1.16x slower                                                  |
| bench_thread_pool          | 504 us                                                 | 582 us: 1.16x slower                                                   |
| nqueens                    | 62.4 ms                                                | 72.2 ms: 1.16x slower                                                  |
| xml_etree_iterparse        | 74.0 ms                                                | 86.0 ms: 1.16x slower                                                  |
| comprehensions             | 14.5 us                                                | 16.9 us: 1.16x slower                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 39.5 ms: 1.16x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 83.9 ms: 1.17x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.85 sec: 1.17x slower                                                 |
| go                         | 102 ms                                                 | 119 ms: 1.17x slower                                                   |
| chameleon                  | 4.70 ms                                                | 5.51 ms: 1.17x slower                                                  |
| chaos                      | 42.5 ms                                                | 50.1 ms: 1.18x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 180 us: 1.20x slower                                                   |
| tornado_http               | 69.3 ms                                                | 83.4 ms: 1.20x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 615 ms: 1.24x slower                                                   |
| pprint_pformat             | 1.01 sec                                               | 1.26 sec: 1.24x slower                                                 |
| tomli_loads                | 1.39 sec                                               | 1.76 sec: 1.26x slower                                                 |
| coverage                   | 38.9 ms                                                | 49.9 ms: 1.28x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.62 sec: 1.30x slower                                                 |
| scimark_sor                | 87.4 ms                                                | 114 ms: 1.30x slower                                                   |
| pyflate                    | 316 ms                                                 | 411 ms: 1.30x slower                                                   |
| asyncio_tcp                | 449 ms                                                 | 595 ms: 1.33x slower                                                   |
| float                      | 55.8 ms                                                | 74.2 ms: 1.33x slower                                                  |
| scimark_fft                | 195 ms                                                 | 261 ms: 1.34x slower                                                   |
| telco                      | 3.68 ms                                                | 4.95 ms: 1.34x slower                                                  |
| nbody                      | 68.8 ms                                                | 92.7 ms: 1.35x slower                                                  |
| mako                       | 7.71 ms                                                | 10.5 ms: 1.36x slower                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 61.4 ms: 1.36x slower                                                  |
| python_startup             | 11.4 ms                                                | 15.6 ms: 1.36x slower                                                  |
| spectral_norm              | 76.4 ms                                                | 106 ms: 1.39x slower                                                   |
| hexiom                     | 4.54 ms                                                | 6.31 ms: 1.39x slower                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 4.38 ms: 1.40x slower                                                  |
| deltablue                  | 2.71 ms                                                | 3.83 ms: 1.41x slower                                                  |
| fannkuch                   | 248 ms                                                 | 360 ms: 1.45x slower                                                   |
| python_startup_no_site     | 9.37 ms                                                | 14.0 ms: 1.49x slower                                                  |
| mypy2                      | 380 ms                                                 | 595 ms: 1.56x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.15x slower                                                           |
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.13x
- 95% likely to have a slowdown of 1.13x
- 99% likely to have a slowdown of 1.12x


# Memory

- memory change: 0.99x