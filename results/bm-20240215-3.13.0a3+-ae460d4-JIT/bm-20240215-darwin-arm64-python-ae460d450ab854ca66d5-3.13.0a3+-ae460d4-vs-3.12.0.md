
# Results vs. 3.12.0

- fork: python
- ref: ae460d450ab854ca66d5
- machine: darwin-arm64
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.00x slower \*
- HPT reliability: 75.06%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.13x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 173 ms: 1.02x slower                                                   |
| chameleon      | 4.70 ms                                                | 4.82 ms: 1.03x slower                                                  |
| docutils       | 1.50 sec                                               | 1.46 sec: 1.03x faster                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 250 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 518 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 669 ms                                                 | 663 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 528 ms: 1.01x faster                                                   |
| async_tree_io              | 668 ms                                                 | 695 ms: 1.04x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 326 ms: 1.04x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 55.4 ms: 1.01x faster                                                  |
| nbody          | 68.8 ms                                                | 75.8 ms: 1.10x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.46 ms: 1.07x faster                                                  |
| regex_dna      | 154 ms                                                 | 145 ms: 1.07x faster                                                   |
| regex_compile  | 77.9 ms                                                | 75.0 ms: 1.04x faster                                                  |
| regex_v8       | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                   |
| xml_etree_process    | 39.7 ms                                                | 38.9 ms: 1.02x faster                                                  |
| json_loads           | 17.2 us                                                | 16.9 us: 1.02x faster                                                  |
| xml_etree_generate   | 55.8 ms                                                | 55.6 ms: 1.01x faster                                                  |
| pickle               | 7.23 us                                                | 7.26 us: 1.01x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.05 us: 1.01x slower                                                  |
| tomli_loads          | 1.39 sec                                               | 1.42 sec: 1.02x slower                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 75.4 ms: 1.02x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.47 ms: 1.04x slower                                                  |
| pickle_list          | 2.89 us                                                | 3.00 us: 1.04x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 158 us: 1.05x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (3): xml_etree_parse, pickle_dict, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.6 ms: 1.20x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 12.2 ms: 1.30x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.78 ms: 1.01x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 70.8 us: 1.31x faster                                                  |
| raytrace                   | 212 ms                                                 | 176 ms: 1.20x faster                                                   |
| asyncio_tcp                | 449 ms                                                 | 381 ms: 1.18x faster                                                   |
| comprehensions             | 14.5 us                                                | 12.6 us: 1.15x faster                                                  |
| unpack_sequence            | 31.5 ns                                                | 28.4 ns: 1.11x faster                                                  |
| deltablue                  | 2.71 ms                                                | 2.45 ms: 1.11x faster                                                  |
| generators                 | 31.1 ms                                                | 28.2 ms: 1.10x faster                                                  |
| logging_silent             | 76.4 ns                                                | 70.6 ns: 1.08x faster                                                  |
| sqlglot_parse              | 848 us                                                 | 790 us: 1.07x faster                                                   |
| regex_effbot               | 2.64 ms                                                | 2.46 ms: 1.07x faster                                                  |
| logging_simple             | 3.69 us                                                | 3.45 us: 1.07x faster                                                  |
| regex_dna                  | 154 ms                                                 | 145 ms: 1.07x faster                                                   |
| crypto_pyaes               | 51.9 ms                                                | 48.8 ms: 1.06x faster                                                  |
| async_tree_none            | 266 ms                                                 | 250 ms: 1.06x faster                                                   |
| logging_format             | 3.98 us                                                | 3.76 us: 1.06x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 26.2 us: 1.05x faster                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 972 us: 1.05x faster                                                   |
| json                       | 3.09 ms                                                | 2.94 ms: 1.05x faster                                                  |
| sympy_str                  | 148 ms                                                 | 141 ms: 1.05x faster                                                   |
| deepcopy_reduce            | 2.07 us                                                | 1.98 us: 1.04x faster                                                  |
| regex_compile              | 77.9 ms                                                | 75.0 ms: 1.04x faster                                                  |
| chaos                      | 42.5 ms                                                | 41.0 ms: 1.04x faster                                                  |
| deepcopy                   | 235 us                                                 | 226 us: 1.04x faster                                                   |
| coroutines                 | 19.2 ms                                                | 18.7 ms: 1.03x faster                                                  |
| sympy_sum                  | 77.6 ms                                                | 75.3 ms: 1.03x faster                                                  |
| docutils                   | 1.50 sec                                               | 1.46 sec: 1.03x faster                                                 |
| sympy_integrate            | 11.4 ms                                                | 11.1 ms: 1.02x faster                                                  |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                                   |
| scimark_lu                 | 76.0 ms                                                | 74.4 ms: 1.02x faster                                                  |
| xml_etree_process          | 39.7 ms                                                | 38.9 ms: 1.02x faster                                                  |
| json_loads                 | 17.2 us                                                | 16.9 us: 1.02x faster                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 518 ms: 1.01x faster                                                   |
| nqueens                    | 62.4 ms                                                | 61.6 ms: 1.01x faster                                                  |
| pathlib                    | 24.2 ms                                                | 23.9 ms: 1.01x faster                                                  |
| sqlglot_normalize          | 186 ms                                                 | 184 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 669 ms                                                 | 663 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 528 ms: 1.01x faster                                                   |
| richards                   | 32.1 ms                                                | 31.9 ms: 1.01x faster                                                  |
| richards_super             | 36.0 ms                                                | 35.8 ms: 1.01x faster                                                  |
| float                      | 55.8 ms                                                | 55.4 ms: 1.01x faster                                                  |
| xml_etree_generate         | 55.8 ms                                                | 55.6 ms: 1.01x faster                                                  |
| gc_traversal               | 2.40 ms                                                | 2.39 ms: 1.00x faster                                                  |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                   |
| sympy_expand               | 241 ms                                                 | 242 ms: 1.00x slower                                                   |
| create_gc_cycles           | 701 us                                                 | 705 us: 1.00x slower                                                   |
| pickle                     | 7.23 us                                                | 7.26 us: 1.01x slower                                                  |
| mako                       | 7.71 ms                                                | 7.78 ms: 1.01x slower                                                  |
| unpickle_list              | 3.02 us                                                | 3.05 us: 1.01x slower                                                  |
| sqlite_synth               | 1.57 us                                                | 1.59 us: 1.01x slower                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 34.6 ms: 1.02x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.61 sec: 1.02x slower                                                 |
| tomli_loads                | 1.39 sec                                               | 1.42 sec: 1.02x slower                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 75.4 ms: 1.02x slower                                                  |
| 2to3                       | 169 ms                                                 | 173 ms: 1.02x slower                                                   |
| pycparser                  | 677 ms                                                 | 690 ms: 1.02x slower                                                   |
| pprint_safe_repr           | 497 ms                                                 | 509 ms: 1.02x slower                                                   |
| chameleon                  | 4.70 ms                                                | 4.82 ms: 1.03x slower                                                  |
| pprint_pformat             | 1.01 sec                                               | 1.04 sec: 1.03x slower                                                 |
| pyflate                    | 316 ms                                                 | 326 ms: 1.03x slower                                                   |
| spectral_norm              | 76.4 ms                                                | 79.0 ms: 1.03x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 74.5 ms: 1.04x slower                                                  |
| json_dumps                 | 6.22 ms                                                | 6.47 ms: 1.04x slower                                                  |
| pickle_list                | 2.89 us                                                | 3.00 us: 1.04x slower                                                  |
| async_tree_io              | 668 ms                                                 | 695 ms: 1.04x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 326 ms: 1.04x slower                                                   |
| unpickle_pure_python       | 151 us                                                 | 158 us: 1.05x slower                                                   |
| bench_mp_pool              | 44.9 ms                                                | 47.4 ms: 1.06x slower                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.31 ms: 1.06x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.32 sec: 1.06x slower                                                 |
| regex_v8                   | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 48.6 ms: 1.08x slower                                                  |
| hexiom                     | 4.54 ms                                                | 4.92 ms: 1.08x slower                                                  |
| go                         | 102 ms                                                 | 110 ms: 1.09x slower                                                   |
| scimark_fft                | 195 ms                                                 | 213 ms: 1.09x slower                                                   |
| fannkuch                   | 248 ms                                                 | 272 ms: 1.09x slower                                                   |
| nbody                      | 68.8 ms                                                | 75.8 ms: 1.10x slower                                                  |
| python_startup             | 11.4 ms                                                | 13.6 ms: 1.20x slower                                                  |
| scimark_sor                | 87.4 ms                                                | 105 ms: 1.21x slower                                                   |
| coverage                   | 38.9 ms                                                | 47.6 ms: 1.22x slower                                                  |
| telco                      | 3.68 ms                                                | 4.58 ms: 1.25x slower                                                  |
| python_startup_no_site     | 9.37 ms                                                | 12.2 ms: 1.30x slower                                                  |
| mypy2                      | 380 ms                                                 | 524 ms: 1.38x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (11): xml_etree_parse, async_tree_memoization_tg, dulwich_log, bench_thread_pool, async_generators, pidigits, pickle_dict, async_tree_none_tg, unpickle, tornado_http, dask
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 75.06% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.13x