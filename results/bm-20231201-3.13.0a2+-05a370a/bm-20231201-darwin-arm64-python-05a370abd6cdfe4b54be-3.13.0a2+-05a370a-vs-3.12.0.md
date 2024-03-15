
# Results vs. 3.12.0

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: darwin-arm64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.03x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 175 ms: 1.03x slower                                                   |
| chameleon      | 4.70 ms                                                | 5.13 ms: 1.09x slower                                                  |
| docutils       | 1.50 sec                                               | 1.50 sec: 1.00x faster                                                 |
| tornado_http   | 69.3 ms                                                | 71.9 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 256 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 543 ms: 1.02x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 686 ms: 1.02x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 333 ms: 1.03x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 268 ms: 1.04x slower                                                   |
| async_tree_io              | 668 ms                                                 | 706 ms: 1.06x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 331 ms: 1.06x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 282 ms: 1.00x slower                                                   |
| float          | 55.8 ms                                                | 58.0 ms: 1.04x slower                                                  |
| nbody          | 68.8 ms                                                | 82.1 ms: 1.19x slower                                                  |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 149 ms: 1.04x faster                                                   |
| regex_effbot   | 2.64 ms                                                | 2.57 ms: 1.03x faster                                                  |
| regex_compile  | 77.9 ms                                                | 79.3 ms: 1.02x slower                                                  |
| regex_v8       | 16.0 ms                                                | 16.9 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_dict          | 18.1 us                                                | 17.9 us: 1.01x faster                                                  |
| unpickle             | 9.12 us                                                | 9.07 us: 1.01x faster                                                  |
| xml_etree_parse      | 106 ms                                                 | 108 ms: 1.02x slower                                                   |
| xml_etree_process    | 39.7 ms                                                | 40.7 ms: 1.03x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 76.1 ms: 1.03x slower                                                  |
| pickle               | 7.23 us                                                | 7.47 us: 1.03x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.14 us: 1.04x slower                                                  |
| pickle_pure_python   | 200 us                                                 | 208 us: 1.04x slower                                                   |
| xml_etree_generate   | 55.8 ms                                                | 58.4 ms: 1.05x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.59 ms: 1.06x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 165 us: 1.10x slower                                                   |
| tomli_loads          | 1.39 sec                                               | 1.61 sec: 1.15x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (2): json_loads, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.2 ms: 1.15x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.8 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.20x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.78 ms: 1.01x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 77.5 us: 1.20x faster                                                  |
| generators                 | 31.1 ms                                                | 26.1 ms: 1.19x faster                                                  |
| raytrace                   | 212 ms                                                 | 184 ms: 1.15x faster                                                   |
| comprehensions             | 14.5 us                                                | 12.7 us: 1.15x faster                                                  |
| deltablue                  | 2.71 ms                                                | 2.45 ms: 1.11x faster                                                  |
| asyncio_tcp                | 449 ms                                                 | 412 ms: 1.09x faster                                                   |
| unpack_sequence            | 31.5 ns                                                | 29.0 ns: 1.08x faster                                                  |
| logging_silent             | 76.4 ns                                                | 71.0 ns: 1.08x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 26.0 us: 1.06x faster                                                  |
| crypto_pyaes               | 51.9 ms                                                | 48.9 ms: 1.06x faster                                                  |
| async_tree_none            | 266 ms                                                 | 256 ms: 1.04x faster                                                   |
| regex_dna                  | 154 ms                                                 | 149 ms: 1.04x faster                                                   |
| regex_effbot               | 2.64 ms                                                | 2.57 ms: 1.03x faster                                                  |
| sqlglot_parse              | 848 us                                                 | 829 us: 1.02x faster                                                   |
| sympy_sum                  | 77.6 ms                                                | 75.9 ms: 1.02x faster                                                  |
| spectral_norm              | 76.4 ms                                                | 75.1 ms: 1.02x faster                                                  |
| sympy_integrate            | 11.4 ms                                                | 11.2 ms: 1.02x faster                                                  |
| logging_simple             | 3.69 us                                                | 3.63 us: 1.02x faster                                                  |
| json                       | 3.09 ms                                                | 3.04 ms: 1.01x faster                                                  |
| deepcopy                   | 235 us                                                 | 232 us: 1.01x faster                                                   |
| sqlglot_transpile          | 1.02 ms                                                | 1.01 ms: 1.01x faster                                                  |
| logging_format             | 3.98 us                                                | 3.95 us: 1.01x faster                                                  |
| pickle_dict                | 18.1 us                                                | 17.9 us: 1.01x faster                                                  |
| sympy_str                  | 148 ms                                                 | 147 ms: 1.01x faster                                                   |
| unpickle                   | 9.12 us                                                | 9.07 us: 1.01x faster                                                  |
| docutils                   | 1.50 sec                                               | 1.50 sec: 1.00x faster                                                 |
| pidigits                   | 282 ms                                                 | 282 ms: 1.00x slower                                                   |
| async_generators           | 304 ms                                                 | 305 ms: 1.00x slower                                                   |
| create_gc_cycles           | 701 us                                                 | 703 us: 1.00x slower                                                   |
| mako                       | 7.71 ms                                                | 7.78 ms: 1.01x slower                                                  |
| nqueens                    | 62.4 ms                                                | 63.0 ms: 1.01x slower                                                  |
| bench_mp_pool              | 44.9 ms                                                | 45.3 ms: 1.01x slower                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.17 ms: 1.01x slower                                                  |
| dulwich_log                | 29.8 ms                                                | 30.2 ms: 1.01x slower                                                  |
| chaos                      | 42.5 ms                                                | 43.2 ms: 1.02x slower                                                  |
| xml_etree_parse            | 106 ms                                                 | 108 ms: 1.02x slower                                                   |
| regex_compile              | 77.9 ms                                                | 79.3 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 543 ms: 1.02x slower                                                   |
| pathlib                    | 24.2 ms                                                | 24.8 ms: 1.02x slower                                                  |
| bench_thread_pool          | 504 us                                                 | 516 us: 1.02x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 686 ms: 1.02x slower                                                   |
| xml_etree_process          | 39.7 ms                                                | 40.7 ms: 1.03x slower                                                  |
| xml_etree_iterparse        | 74.0 ms                                                | 76.1 ms: 1.03x slower                                                  |
| 2to3                       | 169 ms                                                 | 175 ms: 1.03x slower                                                   |
| sqlglot_normalize          | 186 ms                                                 | 192 ms: 1.03x slower                                                   |
| dask                       | 222 ms                                                 | 229 ms: 1.03x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 333 ms: 1.03x slower                                                   |
| pickle                     | 7.23 us                                                | 7.47 us: 1.03x slower                                                  |
| tornado_http               | 69.3 ms                                                | 71.9 ms: 1.04x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 268 ms: 1.04x slower                                                   |
| float                      | 55.8 ms                                                | 58.0 ms: 1.04x slower                                                  |
| unpickle_list              | 3.02 us                                                | 3.14 us: 1.04x slower                                                  |
| pickle_pure_python         | 200 us                                                 | 208 us: 1.04x slower                                                   |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.30 sec: 1.04x slower                                                 |
| go                         | 102 ms                                                 | 106 ms: 1.04x slower                                                   |
| xml_etree_generate         | 55.8 ms                                                | 58.4 ms: 1.05x slower                                                  |
| pycparser                  | 677 ms                                                 | 710 ms: 1.05x slower                                                   |
| meteor_contest             | 71.7 ms                                                | 75.3 ms: 1.05x slower                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 35.8 ms: 1.05x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.66 sec: 1.05x slower                                                 |
| sqlite_synth               | 1.57 us                                                | 1.65 us: 1.05x slower                                                  |
| sympy_expand               | 241 ms                                                 | 254 ms: 1.05x slower                                                   |
| async_tree_io              | 668 ms                                                 | 706 ms: 1.06x slower                                                   |
| gc_traversal               | 2.40 ms                                                | 2.54 ms: 1.06x slower                                                  |
| regex_v8                   | 16.0 ms                                                | 16.9 ms: 1.06x slower                                                  |
| json_dumps                 | 6.22 ms                                                | 6.59 ms: 1.06x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 331 ms: 1.06x slower                                                   |
| pprint_pformat             | 1.01 sec                                               | 1.09 sec: 1.08x slower                                                 |
| pprint_safe_repr           | 497 ms                                                 | 536 ms: 1.08x slower                                                   |
| scimark_monte_carlo        | 45.0 ms                                                | 48.5 ms: 1.08x slower                                                  |
| richards_super             | 36.0 ms                                                | 38.9 ms: 1.08x slower                                                  |
| scimark_fft                | 195 ms                                                 | 212 ms: 1.09x slower                                                   |
| pyflate                    | 316 ms                                                 | 344 ms: 1.09x slower                                                   |
| chameleon                  | 4.70 ms                                                | 5.13 ms: 1.09x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 165 us: 1.10x slower                                                   |
| richards                   | 32.1 ms                                                | 35.2 ms: 1.10x slower                                                  |
| hexiom                     | 4.54 ms                                                | 5.02 ms: 1.10x slower                                                  |
| python_startup             | 11.4 ms                                                | 13.2 ms: 1.15x slower                                                  |
| tomli_loads                | 1.39 sec                                               | 1.61 sec: 1.15x slower                                                 |
| fannkuch                   | 248 ms                                                 | 289 ms: 1.16x slower                                                   |
| nbody                      | 68.8 ms                                                | 82.1 ms: 1.19x slower                                                  |
| scimark_sor                | 87.4 ms                                                | 107 ms: 1.23x slower                                                   |
| coverage                   | 38.9 ms                                                | 48.0 ms: 1.23x slower                                                  |
| python_startup_no_site     | 9.37 ms                                                | 11.8 ms: 1.26x slower                                                  |
| telco                      | 3.68 ms                                                | 4.72 ms: 1.28x slower                                                  |
| mypy2                      | 380 ms                                                 | 525 ms: 1.38x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (7): json_loads, pickle_list, scimark_lu, async_tree_cpu_io_mixed, asyncio_websockets, deepcopy_reduce, coroutines
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.99x