
# Results vs. 3.12.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: darwin-arm64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.09x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 181 ms: 1.07x slower                                                   |
| chameleon      | 4.70 ms                                                | 5.34 ms: 1.14x slower                                                  |
| docutils       | 1.50 sec                                               | 1.56 sec: 1.04x slower                                                 |
| tornado_http   | 69.3 ms                                                | 74.9 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 536 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 546 ms: 1.03x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 691 ms: 1.03x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 338 ms: 1.05x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 271 ms: 1.05x slower                                                   |
| async_tree_io              | 668 ms                                                 | 722 ms: 1.08x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 341 ms: 1.09x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| float          | 55.8 ms                                                | 70.9 ms: 1.27x slower                                                  |
| nbody          | 68.8 ms                                                | 90.1 ms: 1.31x slower                                                  |
| Geometric mean | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 153 ms: 1.01x faster                                                   |
| regex_effbot   | 2.64 ms                                                | 2.72 ms: 1.03x slower                                                  |
| regex_v8       | 16.0 ms                                                | 17.8 ms: 1.11x slower                                                  |
| regex_compile  | 77.9 ms                                                | 87.5 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle             | 9.12 us                                                | 9.16 us: 1.00x slower                                                  |
| pickle_list          | 2.89 us                                                | 2.94 us: 1.02x slower                                                  |
| pickle_pure_python   | 200 us                                                 | 206 us: 1.03x slower                                                   |
| pickle               | 7.23 us                                                | 7.46 us: 1.03x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.15 us: 1.04x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.69 ms: 1.07x slower                                                  |
| xml_etree_process    | 39.7 ms                                                | 42.7 ms: 1.08x slower                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 81.1 ms: 1.10x slower                                                  |
| xml_etree_generate   | 55.8 ms                                                | 62.3 ms: 1.11x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 174 us: 1.15x slower                                                   |
| tomli_loads          | 1.39 sec                                               | 1.70 sec: 1.22x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.06x slower                                                           |

Benchmark hidden because not significant (3): pickle_dict, json_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.2 ms: 1.15x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.7 ms: 1.25x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.20x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 9.93 ms: 1.29x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| generators                 | 31.1 ms                                                | 25.6 ms: 1.21x faster                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 78.1 us: 1.19x faster                                                  |
| unpack_sequence            | 31.5 ns                                                | 28.9 ns: 1.09x faster                                                  |
| raytrace                   | 212 ms                                                 | 199 ms: 1.07x faster                                                   |
| json                       | 3.09 ms                                                | 3.01 ms: 1.03x faster                                                  |
| coroutines                 | 19.2 ms                                                | 18.8 ms: 1.02x faster                                                  |
| logging_silent             | 76.4 ns                                                | 75.0 ns: 1.02x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 27.3 us: 1.01x faster                                                  |
| regex_dna                  | 154 ms                                                 | 153 ms: 1.01x faster                                                   |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                   |
| create_gc_cycles           | 701 us                                                 | 704 us: 1.00x slower                                                   |
| pidigits                   | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| unpickle                   | 9.12 us                                                | 9.16 us: 1.00x slower                                                  |
| logging_format             | 3.98 us                                                | 4.02 us: 1.01x slower                                                  |
| logging_simple             | 3.69 us                                                | 3.72 us: 1.01x slower                                                  |
| async_generators           | 304 ms                                                 | 309 ms: 1.02x slower                                                   |
| deepcopy                   | 235 us                                                 | 239 us: 1.02x slower                                                   |
| pickle_list                | 2.89 us                                                | 2.94 us: 1.02x slower                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 536 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 546 ms: 1.03x slower                                                   |
| deepcopy_reduce            | 2.07 us                                                | 2.12 us: 1.03x slower                                                  |
| dulwich_log                | 29.8 ms                                                | 30.6 ms: 1.03x slower                                                  |
| regex_effbot               | 2.64 ms                                                | 2.72 ms: 1.03x slower                                                  |
| bench_mp_pool              | 44.9 ms                                                | 46.1 ms: 1.03x slower                                                  |
| pickle_pure_python         | 200 us                                                 | 206 us: 1.03x slower                                                   |
| pickle                     | 7.23 us                                                | 7.46 us: 1.03x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 691 ms: 1.03x slower                                                   |
| scimark_lu                 | 76.0 ms                                                | 78.7 ms: 1.04x slower                                                  |
| docutils                   | 1.50 sec                                               | 1.56 sec: 1.04x slower                                                 |
| pathlib                    | 24.2 ms                                                | 25.2 ms: 1.04x slower                                                  |
| unpickle_list              | 3.02 us                                                | 3.15 us: 1.04x slower                                                  |
| sqlglot_parse              | 848 us                                                 | 886 us: 1.04x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 338 ms: 1.05x slower                                                   |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.31 sec: 1.05x slower                                                 |
| bench_thread_pool          | 504 us                                                 | 530 us: 1.05x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 271 ms: 1.05x slower                                                   |
| dask                       | 222 ms                                                 | 234 ms: 1.05x slower                                                   |
| sqlglot_transpile          | 1.02 ms                                                | 1.08 ms: 1.05x slower                                                  |
| sympy_integrate            | 11.4 ms                                                | 12.1 ms: 1.07x slower                                                  |
| pycparser                  | 677 ms                                                 | 721 ms: 1.07x slower                                                   |
| 2to3                       | 169 ms                                                 | 181 ms: 1.07x slower                                                   |
| sympy_str                  | 148 ms                                                 | 158 ms: 1.07x slower                                                   |
| richards_super             | 36.0 ms                                                | 38.5 ms: 1.07x slower                                                  |
| json_dumps                 | 6.22 ms                                                | 6.69 ms: 1.07x slower                                                  |
| sympy_sum                  | 77.6 ms                                                | 83.4 ms: 1.07x slower                                                  |
| sqlglot_normalize          | 186 ms                                                 | 200 ms: 1.08x slower                                                   |
| xml_etree_process          | 39.7 ms                                                | 42.7 ms: 1.08x slower                                                  |
| crypto_pyaes               | 51.9 ms                                                | 55.9 ms: 1.08x slower                                                  |
| richards                   | 32.1 ms                                                | 34.6 ms: 1.08x slower                                                  |
| async_tree_io              | 668 ms                                                 | 722 ms: 1.08x slower                                                   |
| tornado_http               | 69.3 ms                                                | 74.9 ms: 1.08x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.71 sec: 1.08x slower                                                 |
| sympy_expand               | 241 ms                                                 | 262 ms: 1.09x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 341 ms: 1.09x slower                                                   |
| sqlite_synth               | 1.57 us                                                | 1.72 us: 1.09x slower                                                  |
| xml_etree_iterparse        | 74.0 ms                                                | 81.1 ms: 1.10x slower                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 37.8 ms: 1.11x slower                                                  |
| regex_v8                   | 16.0 ms                                                | 17.8 ms: 1.11x slower                                                  |
| xml_etree_generate         | 55.8 ms                                                | 62.3 ms: 1.11x slower                                                  |
| nqueens                    | 62.4 ms                                                | 69.7 ms: 1.12x slower                                                  |
| comprehensions             | 14.5 us                                                | 16.3 us: 1.12x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 80.3 ms: 1.12x slower                                                  |
| regex_compile              | 77.9 ms                                                | 87.5 ms: 1.12x slower                                                  |
| chaos                      | 42.5 ms                                                | 48.2 ms: 1.13x slower                                                  |
| go                         | 102 ms                                                 | 115 ms: 1.13x slower                                                   |
| chameleon                  | 4.70 ms                                                | 5.34 ms: 1.14x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 174 us: 1.15x slower                                                   |
| python_startup             | 11.4 ms                                                | 13.2 ms: 1.15x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 594 ms: 1.19x slower                                                   |
| pyflate                    | 316 ms                                                 | 377 ms: 1.20x slower                                                   |
| pprint_pformat             | 1.01 sec                                               | 1.22 sec: 1.20x slower                                                 |
| tomli_loads                | 1.39 sec                                               | 1.70 sec: 1.22x slower                                                 |
| coverage                   | 38.9 ms                                                | 48.4 ms: 1.25x slower                                                  |
| python_startup_no_site     | 9.37 ms                                                | 11.7 ms: 1.25x slower                                                  |
| scimark_sor                | 87.4 ms                                                | 110 ms: 1.26x slower                                                   |
| float                      | 55.8 ms                                                | 70.9 ms: 1.27x slower                                                  |
| mako                       | 7.71 ms                                                | 9.93 ms: 1.29x slower                                                  |
| scimark_fft                | 195 ms                                                 | 253 ms: 1.30x slower                                                   |
| nbody                      | 68.8 ms                                                | 90.1 ms: 1.31x slower                                                  |
| telco                      | 3.68 ms                                                | 4.83 ms: 1.31x slower                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 59.3 ms: 1.32x slower                                                  |
| hexiom                     | 4.54 ms                                                | 6.08 ms: 1.34x slower                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 4.21 ms: 1.34x slower                                                  |
| deltablue                  | 2.71 ms                                                | 3.68 ms: 1.36x slower                                                  |
| fannkuch                   | 248 ms                                                 | 341 ms: 1.37x slower                                                   |
| spectral_norm              | 76.4 ms                                                | 106 ms: 1.38x slower                                                   |
| mypy2                      | 380 ms                                                 | 542 ms: 1.43x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.09x slower                                                           |

Benchmark hidden because not significant (6): asyncio_tcp, async_tree_none, pickle_dict, gc_traversal, json_loads, xml_etree_parse
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.06x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 0.99x