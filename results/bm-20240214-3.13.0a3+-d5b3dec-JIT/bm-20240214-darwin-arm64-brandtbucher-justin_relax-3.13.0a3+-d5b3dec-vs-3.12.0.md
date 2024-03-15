
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: d5b3dec
- commit date: 2024-02-14
- overall geometric mean: 1.01x slower \*
- HPT reliability: 73.20%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.14x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 174 ms: 1.03x slower                                                 |
| chameleon      | 4.70 ms                                                | 4.79 ms: 1.02x slower                                                |
| docutils       | 1.50 sec                                               | 1.47 sec: 1.02x faster                                               |
| Geometric mean | (ref)                                                  | 1.01x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 251 ms: 1.06x faster                                                 |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 518 ms: 1.02x faster                                                 |
| async_tree_io_tg           | 669 ms                                                 | 660 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 527 ms: 1.01x faster                                                 |
| async_tree_io              | 668 ms                                                 | 694 ms: 1.04x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 326 ms: 1.04x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 55.6 ms: 1.00x faster                                                |
| nbody          | 68.8 ms                                                | 76.5 ms: 1.11x slower                                                |
| Geometric mean | (ref)                                                  | 1.03x slower                                                         |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.55 ms: 1.03x faster                                                |
| regex_compile  | 77.9 ms                                                | 75.6 ms: 1.03x faster                                                |
| regex_dna      | 154 ms                                                 | 151 ms: 1.02x faster                                                 |
| regex_v8       | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                |
| Geometric mean | (ref)                                                  | 1.00x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 195 us: 1.02x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 38.8 ms: 1.02x faster                                                |
| json_loads           | 17.2 us                                                | 17.0 us: 1.01x faster                                                |
| xml_etree_generate   | 55.8 ms                                                | 55.7 ms: 1.00x faster                                                |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                                |
| unpickle             | 9.12 us                                                | 9.15 us: 1.00x slower                                                |
| tomli_loads          | 1.39 sec                                               | 1.40 sec: 1.01x slower                                               |
| pickle_list          | 2.89 us                                                | 2.93 us: 1.02x slower                                                |
| xml_etree_iterparse  | 74.0 ms                                                | 75.6 ms: 1.02x slower                                                |
| unpickle_list        | 3.02 us                                                | 3.10 us: 1.03x slower                                                |
| json_dumps           | 6.22 ms                                                | 6.46 ms: 1.04x slower                                                |
| unpickle_pure_python | 151 us                                                 | 158 us: 1.05x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                         |

Benchmark hidden because not significant (2): xml_etree_parse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.6 ms: 1.20x slower                                                |
| python_startup_no_site | 9.37 ms                                                | 12.1 ms: 1.29x slower                                                |
| Geometric mean         | (ref)                                                  | 1.24x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.80 ms: 1.01x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 70.4 us: 1.32x faster                                                |
| raytrace                   | 212 ms                                                 | 177 ms: 1.20x faster                                                 |
| comprehensions             | 14.5 us                                                | 12.6 us: 1.15x faster                                                |
| unpack_sequence            | 31.5 ns                                                | 28.5 ns: 1.10x faster                                                |
| deltablue                  | 2.71 ms                                                | 2.46 ms: 1.10x faster                                                |
| generators                 | 31.1 ms                                                | 28.3 ms: 1.10x faster                                                |
| asyncio_tcp                | 449 ms                                                 | 411 ms: 1.09x faster                                                 |
| logging_silent             | 76.4 ns                                                | 70.6 ns: 1.08x faster                                                |
| deepcopy_memo              | 27.7 us                                                | 25.8 us: 1.07x faster                                                |
| sqlglot_parse              | 848 us                                                 | 792 us: 1.07x faster                                                 |
| logging_simple             | 3.69 us                                                | 3.47 us: 1.06x faster                                                |
| crypto_pyaes               | 51.9 ms                                                | 48.9 ms: 1.06x faster                                                |
| async_tree_none            | 266 ms                                                 | 251 ms: 1.06x faster                                                 |
| logging_format             | 3.98 us                                                | 3.77 us: 1.06x faster                                                |
| sqlglot_transpile          | 1.02 ms                                                | 978 us: 1.04x faster                                                 |
| deepcopy                   | 235 us                                                 | 225 us: 1.04x faster                                                 |
| sympy_str                  | 148 ms                                                 | 142 ms: 1.04x faster                                                 |
| coroutines                 | 19.2 ms                                                | 18.5 ms: 1.04x faster                                                |
| deepcopy_reduce            | 2.07 us                                                | 1.99 us: 1.04x faster                                                |
| json                       | 3.09 ms                                                | 2.98 ms: 1.04x faster                                                |
| regex_effbot               | 2.64 ms                                                | 2.55 ms: 1.03x faster                                                |
| chaos                      | 42.5 ms                                                | 41.3 ms: 1.03x faster                                                |
| regex_compile              | 77.9 ms                                                | 75.6 ms: 1.03x faster                                                |
| sympy_sum                  | 77.6 ms                                                | 75.6 ms: 1.03x faster                                                |
| pickle_pure_python         | 200 us                                                 | 195 us: 1.02x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 38.8 ms: 1.02x faster                                                |
| docutils                   | 1.50 sec                                               | 1.47 sec: 1.02x faster                                               |
| regex_dna                  | 154 ms                                                 | 151 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 518 ms: 1.02x faster                                                 |
| async_tree_io_tg           | 669 ms                                                 | 660 ms: 1.01x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 183 ms: 1.01x faster                                                 |
| json_loads                 | 17.2 us                                                | 17.0 us: 1.01x faster                                                |
| scimark_lu                 | 76.0 ms                                                | 75.0 ms: 1.01x faster                                                |
| pathlib                    | 24.2 ms                                                | 24.0 ms: 1.01x faster                                                |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 527 ms: 1.01x faster                                                 |
| sympy_integrate            | 11.4 ms                                                | 11.3 ms: 1.01x faster                                                |
| richards_super             | 36.0 ms                                                | 35.7 ms: 1.01x faster                                                |
| richards                   | 32.1 ms                                                | 31.9 ms: 1.01x faster                                                |
| nqueens                    | 62.4 ms                                                | 62.2 ms: 1.00x faster                                                |
| xml_etree_generate         | 55.8 ms                                                | 55.7 ms: 1.00x faster                                                |
| float                      | 55.8 ms                                                | 55.6 ms: 1.00x faster                                                |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                 |
| gc_traversal               | 2.40 ms                                                | 2.39 ms: 1.00x faster                                                |
| sympy_expand               | 241 ms                                                 | 241 ms: 1.00x faster                                                 |
| dulwich_log                | 29.8 ms                                                | 29.8 ms: 1.00x faster                                                |
| pickle_dict                | 18.1 us                                                | 18.1 us: 1.00x slower                                                |
| unpickle                   | 9.12 us                                                | 9.15 us: 1.00x slower                                                |
| create_gc_cycles           | 701 us                                                 | 706 us: 1.01x slower                                                 |
| tomli_loads                | 1.39 sec                                               | 1.40 sec: 1.01x slower                                               |
| mako                       | 7.71 ms                                                | 7.80 ms: 1.01x slower                                                |
| dask                       | 222 ms                                                 | 225 ms: 1.01x slower                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 34.5 ms: 1.01x slower                                                |
| pickle_list                | 2.89 us                                                | 2.93 us: 1.02x slower                                                |
| sqlite_synth               | 1.57 us                                                | 1.60 us: 1.02x slower                                                |
| chameleon                  | 4.70 ms                                                | 4.79 ms: 1.02x slower                                                |
| xml_etree_iterparse        | 74.0 ms                                                | 75.6 ms: 1.02x slower                                                |
| pycparser                  | 677 ms                                                 | 693 ms: 1.02x slower                                                 |
| mdp                        | 1.58 sec                                               | 1.62 sec: 1.03x slower                                               |
| unpickle_list              | 3.02 us                                                | 3.10 us: 1.03x slower                                                |
| 2to3                       | 169 ms                                                 | 174 ms: 1.03x slower                                                 |
| pyflate                    | 316 ms                                                 | 327 ms: 1.04x slower                                                 |
| json_dumps                 | 6.22 ms                                                | 6.46 ms: 1.04x slower                                                |
| async_tree_io              | 668 ms                                                 | 694 ms: 1.04x slower                                                 |
| meteor_contest             | 71.7 ms                                                | 74.7 ms: 1.04x slower                                                |
| pprint_pformat             | 1.01 sec                                               | 1.05 sec: 1.04x slower                                               |
| async_tree_memoization     | 312 ms                                                 | 326 ms: 1.04x slower                                                 |
| pprint_safe_repr           | 497 ms                                                 | 519 ms: 1.04x slower                                                 |
| unpickle_pure_python       | 151 us                                                 | 158 us: 1.05x slower                                                 |
| bench_mp_pool              | 44.9 ms                                                | 47.2 ms: 1.05x slower                                                |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.31 sec: 1.05x slower                                               |
| spectral_norm              | 76.4 ms                                                | 80.5 ms: 1.05x slower                                                |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.33 ms: 1.06x slower                                                |
| regex_v8                   | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                |
| go                         | 102 ms                                                 | 110 ms: 1.08x slower                                                 |
| fannkuch                   | 248 ms                                                 | 270 ms: 1.09x slower                                                 |
| scimark_monte_carlo        | 45.0 ms                                                | 48.9 ms: 1.09x slower                                                |
| hexiom                     | 4.54 ms                                                | 5.04 ms: 1.11x slower                                                |
| nbody                      | 68.8 ms                                                | 76.5 ms: 1.11x slower                                                |
| scimark_fft                | 195 ms                                                 | 218 ms: 1.12x slower                                                 |
| python_startup             | 11.4 ms                                                | 13.6 ms: 1.20x slower                                                |
| scimark_sor                | 87.4 ms                                                | 106 ms: 1.21x slower                                                 |
| telco                      | 3.68 ms                                                | 4.49 ms: 1.22x slower                                                |
| coverage                   | 38.9 ms                                                | 47.5 ms: 1.22x slower                                                |
| python_startup_no_site     | 9.37 ms                                                | 12.1 ms: 1.29x slower                                                |
| mypy2                      | 380 ms                                                 | 524 ms: 1.38x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                         |

Benchmark hidden because not significant (8): async_tree_memoization_tg, xml_etree_parse, async_tree_none_tg, async_generators, pidigits, pickle, bench_thread_pool, tornado_http
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 73.20% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.14x