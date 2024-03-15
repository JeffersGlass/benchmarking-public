
# Results vs. 3.12.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: darwin-arm64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.03x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 178 ms: 1.05x slower                                                   |
| chameleon      | 4.70 ms                                                | 5.19 ms: 1.11x slower                                                  |
| docutils       | 1.50 sec                                               | 1.51 sec: 1.00x slower                                                 |
| tornado_http   | 69.3 ms                                                | 71.8 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 256 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 537 ms: 1.01x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 678 ms: 1.01x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 329 ms: 1.02x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 263 ms: 1.02x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 332 ms: 1.06x slower                                                   |
| async_tree_io              | 668 ms                                                 | 711 ms: 1.06x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 282 ms: 1.00x slower                                                   |
| float          | 55.8 ms                                                | 61.0 ms: 1.09x slower                                                  |
| nbody          | 68.8 ms                                                | 82.4 ms: 1.20x slower                                                  |
| Geometric mean | (ref)                                                  | 1.09x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                   |
| regex_compile  | 77.9 ms                                                | 76.9 ms: 1.01x faster                                                  |
| regex_effbot   | 2.64 ms                                                | 2.72 ms: 1.03x slower                                                  |
| regex_v8       | 16.0 ms                                                | 17.7 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_dict          | 18.1 us                                                | 17.9 us: 1.01x faster                                                  |
| unpickle             | 9.12 us                                                | 9.17 us: 1.01x slower                                                  |
| pickle_list          | 2.89 us                                                | 2.91 us: 1.01x slower                                                  |
| xml_etree_parse      | 106 ms                                                 | 107 ms: 1.01x slower                                                   |
| pickle               | 7.23 us                                                | 7.44 us: 1.03x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.11 us: 1.03x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 76.6 ms: 1.03x slower                                                  |
| xml_etree_process    | 39.7 ms                                                | 41.2 ms: 1.04x slower                                                  |
| pickle_pure_python   | 200 us                                                 | 208 us: 1.04x slower                                                   |
| xml_etree_generate   | 55.8 ms                                                | 58.2 ms: 1.04x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.66 ms: 1.07x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 167 us: 1.11x slower                                                   |
| tomli_loads          | 1.39 sec                                               | 1.61 sec: 1.15x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.1 ms: 1.15x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.6 ms: 1.24x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.99 ms: 1.04x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 75.0 us: 1.24x faster                                                  |
| generators                 | 31.1 ms                                                | 26.2 ms: 1.19x faster                                                  |
| raytrace                   | 212 ms                                                 | 183 ms: 1.16x faster                                                   |
| comprehensions             | 14.5 us                                                | 12.7 us: 1.15x faster                                                  |
| asyncio_tcp                | 449 ms                                                 | 416 ms: 1.08x faster                                                   |
| deltablue                  | 2.71 ms                                                | 2.54 ms: 1.07x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 26.3 us: 1.05x faster                                                  |
| logging_silent             | 76.4 ns                                                | 72.8 ns: 1.05x faster                                                  |
| unpack_sequence            | 31.5 ns                                                | 30.3 ns: 1.04x faster                                                  |
| async_tree_none            | 266 ms                                                 | 256 ms: 1.04x faster                                                   |
| crypto_pyaes               | 51.9 ms                                                | 50.2 ms: 1.03x faster                                                  |
| regex_dna                  | 154 ms                                                 | 152 ms: 1.02x faster                                                   |
| json                       | 3.09 ms                                                | 3.04 ms: 1.01x faster                                                  |
| chaos                      | 42.5 ms                                                | 42.0 ms: 1.01x faster                                                  |
| regex_compile              | 77.9 ms                                                | 76.9 ms: 1.01x faster                                                  |
| sympy_sum                  | 77.6 ms                                                | 76.7 ms: 1.01x faster                                                  |
| sympy_integrate            | 11.4 ms                                                | 11.2 ms: 1.01x faster                                                  |
| logging_simple             | 3.69 us                                                | 3.65 us: 1.01x faster                                                  |
| pickle_dict                | 18.1 us                                                | 17.9 us: 1.01x faster                                                  |
| spectral_norm              | 76.4 ms                                                | 76.1 ms: 1.00x faster                                                  |
| pidigits                   | 282 ms                                                 | 282 ms: 1.00x slower                                                   |
| docutils                   | 1.50 sec                                               | 1.51 sec: 1.00x slower                                                 |
| create_gc_cycles           | 701 us                                                 | 705 us: 1.01x slower                                                   |
| unpickle                   | 9.12 us                                                | 9.17 us: 1.01x slower                                                  |
| async_generators           | 304 ms                                                 | 306 ms: 1.01x slower                                                   |
| nqueens                    | 62.4 ms                                                | 62.8 ms: 1.01x slower                                                  |
| sympy_str                  | 148 ms                                                 | 149 ms: 1.01x slower                                                   |
| pickle_list                | 2.89 us                                                | 2.91 us: 1.01x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 537 ms: 1.01x slower                                                   |
| xml_etree_parse            | 106 ms                                                 | 107 ms: 1.01x slower                                                   |
| dulwich_log                | 29.8 ms                                                | 30.2 ms: 1.01x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 678 ms: 1.01x slower                                                   |
| deepcopy_reduce            | 2.07 us                                                | 2.11 us: 1.02x slower                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.20 ms: 1.02x slower                                                  |
| bench_mp_pool              | 44.9 ms                                                | 45.7 ms: 1.02x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 329 ms: 1.02x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 263 ms: 1.02x slower                                                   |
| sqlglot_parse              | 848 us                                                 | 869 us: 1.03x slower                                                   |
| pathlib                    | 24.2 ms                                                | 24.9 ms: 1.03x slower                                                  |
| regex_effbot               | 2.64 ms                                                | 2.72 ms: 1.03x slower                                                  |
| pickle                     | 7.23 us                                                | 7.44 us: 1.03x slower                                                  |
| unpickle_list              | 3.02 us                                                | 3.11 us: 1.03x slower                                                  |
| bench_thread_pool          | 504 us                                                 | 519 us: 1.03x slower                                                   |
| sqlglot_transpile          | 1.02 ms                                                | 1.05 ms: 1.03x slower                                                  |
| scimark_lu                 | 76.0 ms                                                | 78.3 ms: 1.03x slower                                                  |
| dask                       | 222 ms                                                 | 229 ms: 1.03x slower                                                   |
| xml_etree_iterparse        | 74.0 ms                                                | 76.6 ms: 1.03x slower                                                  |
| mako                       | 7.71 ms                                                | 7.99 ms: 1.04x slower                                                  |
| tornado_http               | 69.3 ms                                                | 71.8 ms: 1.04x slower                                                  |
| sqlglot_normalize          | 186 ms                                                 | 193 ms: 1.04x slower                                                   |
| hexiom                     | 4.54 ms                                                | 4.71 ms: 1.04x slower                                                  |
| xml_etree_process          | 39.7 ms                                                | 41.2 ms: 1.04x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 74.5 ms: 1.04x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.64 sec: 1.04x slower                                                 |
| pickle_pure_python         | 200 us                                                 | 208 us: 1.04x slower                                                   |
| xml_etree_generate         | 55.8 ms                                                | 58.2 ms: 1.04x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.30 sec: 1.05x slower                                                 |
| 2to3                       | 169 ms                                                 | 178 ms: 1.05x slower                                                   |
| sqlglot_optimize           | 34.0 ms                                                | 35.8 ms: 1.05x slower                                                  |
| sqlite_synth               | 1.57 us                                                | 1.65 us: 1.05x slower                                                  |
| pycparser                  | 677 ms                                                 | 720 ms: 1.06x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 332 ms: 1.06x slower                                                   |
| async_tree_io              | 668 ms                                                 | 711 ms: 1.06x slower                                                   |
| sympy_expand               | 241 ms                                                 | 257 ms: 1.07x slower                                                   |
| json_dumps                 | 6.22 ms                                                | 6.66 ms: 1.07x slower                                                  |
| go                         | 102 ms                                                 | 109 ms: 1.07x slower                                                   |
| pprint_pformat             | 1.01 sec                                               | 1.09 sec: 1.08x slower                                                 |
| scimark_fft                | 195 ms                                                 | 211 ms: 1.08x slower                                                   |
| pprint_safe_repr           | 497 ms                                                 | 539 ms: 1.08x slower                                                   |
| float                      | 55.8 ms                                                | 61.0 ms: 1.09x slower                                                  |
| richards_super             | 36.0 ms                                                | 39.8 ms: 1.10x slower                                                  |
| chameleon                  | 4.70 ms                                                | 5.19 ms: 1.11x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 167 us: 1.11x slower                                                   |
| scimark_monte_carlo        | 45.0 ms                                                | 49.8 ms: 1.11x slower                                                  |
| regex_v8                   | 16.0 ms                                                | 17.7 ms: 1.11x slower                                                  |
| pyflate                    | 316 ms                                                 | 350 ms: 1.11x slower                                                   |
| richards                   | 32.1 ms                                                | 35.7 ms: 1.11x slower                                                  |
| python_startup             | 11.4 ms                                                | 13.1 ms: 1.15x slower                                                  |
| tomli_loads                | 1.39 sec                                               | 1.61 sec: 1.15x slower                                                 |
| fannkuch                   | 248 ms                                                 | 293 ms: 1.18x slower                                                   |
| nbody                      | 68.8 ms                                                | 82.4 ms: 1.20x slower                                                  |
| coverage                   | 38.9 ms                                                | 47.8 ms: 1.23x slower                                                  |
| scimark_sor                | 87.4 ms                                                | 108 ms: 1.24x slower                                                   |
| python_startup_no_site     | 9.37 ms                                                | 11.6 ms: 1.24x slower                                                  |
| telco                      | 3.68 ms                                                | 4.62 ms: 1.26x slower                                                  |
| mypy2                      | 380 ms                                                 | 531 ms: 1.40x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (7): asyncio_websockets, deepcopy, json_loads, gc_traversal, logging_format, coroutines, async_tree_cpu_io_mixed
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.99x