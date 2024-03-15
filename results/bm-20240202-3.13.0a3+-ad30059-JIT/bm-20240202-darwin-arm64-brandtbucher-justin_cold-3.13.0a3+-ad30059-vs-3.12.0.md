
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_cold
- machine: darwin-arm64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.01x slower \*
- HPT reliability: 90.91%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.22x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 177 ms: 1.04x slower                                                |
| chameleon      | 4.70 ms                                                | 4.86 ms: 1.03x slower                                               |
| docutils       | 1.50 sec                                               | 1.48 sec: 1.02x faster                                              |
| Geometric mean | (ref)                                                  | 1.02x slower                                                        |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 250 ms: 1.06x faster                                                |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 518 ms: 1.02x faster                                                |
| async_tree_io_tg           | 669 ms                                                 | 661 ms: 1.01x faster                                                |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 528 ms: 1.01x faster                                                |
| async_tree_io              | 668 ms                                                 | 693 ms: 1.04x slower                                                |
| async_tree_memoization     | 312 ms                                                 | 327 ms: 1.05x slower                                                |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 76.6 ms: 1.11x slower                                               |
| Geometric mean | (ref)                                                  | 1.04x slower                                                        |

Benchmark hidden because not significant (2): float, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.56 ms: 1.03x faster                                               |
| regex_compile  | 77.9 ms                                                | 76.6 ms: 1.02x faster                                               |
| regex_dna      | 154 ms                                                 | 153 ms: 1.01x faster                                                |
| regex_v8       | 16.0 ms                                                | 17.2 ms: 1.08x slower                                               |
| Geometric mean | (ref)                                                  | 1.00x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                |
| unpickle             | 9.12 us                                                | 8.99 us: 1.01x faster                                               |
| json_loads           | 17.2 us                                                | 17.0 us: 1.01x faster                                               |
| xml_etree_process    | 39.7 ms                                                | 39.3 ms: 1.01x faster                                               |
| pickle               | 7.23 us                                                | 7.29 us: 1.01x slower                                               |
| tomli_loads          | 1.39 sec                                               | 1.41 sec: 1.01x slower                                              |
| unpickle_list        | 3.02 us                                                | 3.08 us: 1.02x slower                                               |
| xml_etree_generate   | 55.8 ms                                                | 56.9 ms: 1.02x slower                                               |
| xml_etree_iterparse  | 74.0 ms                                                | 76.0 ms: 1.03x slower                                               |
| pickle_list          | 2.89 us                                                | 3.00 us: 1.04x slower                                               |
| json_dumps           | 6.22 ms                                                | 6.49 ms: 1.04x slower                                               |
| unpickle_pure_python | 151 us                                                 | 158 us: 1.05x slower                                                |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (2): pickle_dict, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 11.6 ms: 1.02x slower                                               |
| python_startup_no_site | 9.37 ms                                                | 10.2 ms: 1.08x slower                                               |
| Geometric mean         | (ref)                                                  | 1.05x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.94 ms: 1.03x slower                                               |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-darwin-arm64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 71.2 us: 1.31x faster                                               |
| raytrace                   | 212 ms                                                 | 177 ms: 1.20x faster                                                |
| comprehensions             | 14.5 us                                                | 12.7 us: 1.14x faster                                               |
| unpack_sequence            | 31.5 ns                                                | 28.2 ns: 1.12x faster                                               |
| asyncio_tcp                | 449 ms                                                 | 405 ms: 1.11x faster                                                |
| generators                 | 31.1 ms                                                | 28.4 ms: 1.09x faster                                               |
| logging_silent             | 76.4 ns                                                | 70.3 ns: 1.09x faster                                               |
| deltablue                  | 2.71 ms                                                | 2.51 ms: 1.08x faster                                               |
| sqlglot_parse              | 848 us                                                 | 794 us: 1.07x faster                                                |
| deepcopy_memo              | 27.7 us                                                | 26.0 us: 1.06x faster                                               |
| async_tree_none            | 266 ms                                                 | 250 ms: 1.06x faster                                                |
| crypto_pyaes               | 51.9 ms                                                | 49.0 ms: 1.06x faster                                               |
| logging_simple             | 3.69 us                                                | 3.48 us: 1.06x faster                                               |
| json                       | 3.09 ms                                                | 2.94 ms: 1.05x faster                                               |
| logging_format             | 3.98 us                                                | 3.80 us: 1.05x faster                                               |
| coroutines                 | 19.2 ms                                                | 18.5 ms: 1.04x faster                                               |
| sympy_str                  | 148 ms                                                 | 142 ms: 1.04x faster                                                |
| deepcopy_reduce            | 2.07 us                                                | 1.99 us: 1.04x faster                                               |
| sqlglot_transpile          | 1.02 ms                                                | 985 us: 1.04x faster                                                |
| deepcopy                   | 235 us                                                 | 227 us: 1.04x faster                                                |
| regex_effbot               | 2.64 ms                                                | 2.56 ms: 1.03x faster                                               |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                                |
| chaos                      | 42.5 ms                                                | 41.8 ms: 1.02x faster                                               |
| regex_compile              | 77.9 ms                                                | 76.6 ms: 1.02x faster                                               |
| docutils                   | 1.50 sec                                               | 1.48 sec: 1.02x faster                                              |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 518 ms: 1.02x faster                                                |
| sympy_sum                  | 77.6 ms                                                | 76.5 ms: 1.01x faster                                               |
| unpickle                   | 9.12 us                                                | 8.99 us: 1.01x faster                                               |
| pathlib                    | 24.2 ms                                                | 23.9 ms: 1.01x faster                                               |
| json_loads                 | 17.2 us                                                | 17.0 us: 1.01x faster                                               |
| async_tree_io_tg           | 669 ms                                                 | 661 ms: 1.01x faster                                                |
| regex_dna                  | 154 ms                                                 | 153 ms: 1.01x faster                                                |
| scimark_lu                 | 76.0 ms                                                | 75.2 ms: 1.01x faster                                               |
| sqlglot_normalize          | 186 ms                                                 | 184 ms: 1.01x faster                                                |
| xml_etree_process          | 39.7 ms                                                | 39.3 ms: 1.01x faster                                               |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 528 ms: 1.01x faster                                                |
| sympy_integrate            | 11.4 ms                                                | 11.3 ms: 1.01x faster                                               |
| gc_traversal               | 2.40 ms                                                | 2.39 ms: 1.01x faster                                               |
| richards                   | 32.1 ms                                                | 32.0 ms: 1.00x faster                                               |
| richards_super             | 36.0 ms                                                | 35.9 ms: 1.00x faster                                               |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                |
| sympy_expand               | 241 ms                                                 | 242 ms: 1.00x slower                                                |
| dulwich_log                | 29.8 ms                                                | 30.0 ms: 1.00x slower                                               |
| bench_thread_pool          | 504 us                                                 | 508 us: 1.01x slower                                                |
| pickle                     | 7.23 us                                                | 7.29 us: 1.01x slower                                               |
| tomli_loads                | 1.39 sec                                               | 1.41 sec: 1.01x slower                                              |
| mdp                        | 1.58 sec                                               | 1.60 sec: 1.01x slower                                              |
| dask                       | 222 ms                                                 | 225 ms: 1.01x slower                                                |
| sqlite_synth               | 1.57 us                                                | 1.60 us: 1.02x slower                                               |
| unpickle_list              | 3.02 us                                                | 3.08 us: 1.02x slower                                               |
| bench_mp_pool              | 44.9 ms                                                | 45.7 ms: 1.02x slower                                               |
| xml_etree_generate         | 55.8 ms                                                | 56.9 ms: 1.02x slower                                               |
| sqlglot_optimize           | 34.0 ms                                                | 34.7 ms: 1.02x slower                                               |
| python_startup             | 11.4 ms                                                | 11.6 ms: 1.02x slower                                               |
| xml_etree_iterparse        | 74.0 ms                                                | 76.0 ms: 1.03x slower                                               |
| pycparser                  | 677 ms                                                 | 696 ms: 1.03x slower                                                |
| mako                       | 7.71 ms                                                | 7.94 ms: 1.03x slower                                               |
| meteor_contest             | 71.7 ms                                                | 74.1 ms: 1.03x slower                                               |
| chameleon                  | 4.70 ms                                                | 4.86 ms: 1.03x slower                                               |
| pprint_safe_repr           | 497 ms                                                 | 515 ms: 1.04x slower                                                |
| async_tree_io              | 668 ms                                                 | 693 ms: 1.04x slower                                                |
| pickle_list                | 2.89 us                                                | 3.00 us: 1.04x slower                                               |
| pyflate                    | 316 ms                                                 | 328 ms: 1.04x slower                                                |
| 2to3                       | 169 ms                                                 | 177 ms: 1.04x slower                                                |
| pprint_pformat             | 1.01 sec                                               | 1.05 sec: 1.04x slower                                              |
| json_dumps                 | 6.22 ms                                                | 6.49 ms: 1.04x slower                                               |
| async_tree_memoization     | 312 ms                                                 | 327 ms: 1.05x slower                                                |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.30 sec: 1.05x slower                                              |
| unpickle_pure_python       | 151 us                                                 | 158 us: 1.05x slower                                                |
| spectral_norm              | 76.4 ms                                                | 81.1 ms: 1.06x slower                                               |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.35 ms: 1.07x slower                                               |
| go                         | 102 ms                                                 | 109 ms: 1.07x slower                                                |
| regex_v8                   | 16.0 ms                                                | 17.2 ms: 1.08x slower                                               |
| python_startup_no_site     | 9.37 ms                                                | 10.2 ms: 1.08x slower                                               |
| scimark_monte_carlo        | 45.0 ms                                                | 49.3 ms: 1.09x slower                                               |
| hexiom                     | 4.54 ms                                                | 4.98 ms: 1.10x slower                                               |
| nbody                      | 68.8 ms                                                | 76.6 ms: 1.11x slower                                               |
| scimark_fft                | 195 ms                                                 | 218 ms: 1.11x slower                                                |
| fannkuch                   | 248 ms                                                 | 278 ms: 1.12x slower                                                |
| coverage                   | 38.9 ms                                                | 46.8 ms: 1.20x slower                                               |
| scimark_sor                | 87.4 ms                                                | 105 ms: 1.21x slower                                                |
| telco                      | 3.68 ms                                                | 4.61 ms: 1.25x slower                                               |
| mypy2                      | 380 ms                                                 | 526 ms: 1.38x slower                                                |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (10): async_tree_memoization_tg, float, pickle_dict, async_tree_none_tg, create_gc_cycles, pidigits, nqueens, xml_etree_parse, async_generators, tornado_http
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 90.91% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.22x