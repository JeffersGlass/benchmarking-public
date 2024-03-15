
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_continue
- machine: darwin-arm64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.00x slower \*
- HPT reliability: 61.38%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.14x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 173 ms: 1.02x slower                                                    |
| chameleon      | 4.70 ms                                                | 4.77 ms: 1.02x slower                                                   |
| docutils       | 1.50 sec                                               | 1.47 sec: 1.02x faster                                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                                            |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 250 ms: 1.06x faster                                                    |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 517 ms: 1.02x faster                                                    |
| async_tree_io_tg           | 669 ms                                                 | 660 ms: 1.01x faster                                                    |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 527 ms: 1.01x faster                                                    |
| async_tree_io              | 668 ms                                                 | 696 ms: 1.04x slower                                                    |
| async_tree_memoization     | 312 ms                                                 | 327 ms: 1.05x slower                                                    |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 54.8 ms: 1.02x faster                                                   |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                    |
| nbody          | 68.8 ms                                                | 75.5 ms: 1.10x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x slower                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 74.6 ms: 1.04x faster                                                   |
| regex_effbot   | 2.64 ms                                                | 2.55 ms: 1.04x faster                                                   |
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                    |
| regex_v8       | 16.0 ms                                                | 17.0 ms: 1.07x slower                                                   |
| Geometric mean | (ref)                                                  | 1.01x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| xml_etree_process    | 39.7 ms                                                | 38.5 ms: 1.03x faster                                                   |
| pickle_pure_python   | 200 us                                                 | 195 us: 1.02x faster                                                    |
| tomli_loads          | 1.39 sec                                               | 1.37 sec: 1.02x faster                                                  |
| json_loads           | 17.2 us                                                | 17.1 us: 1.01x faster                                                   |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                                   |
| pickle               | 7.23 us                                                | 7.27 us: 1.01x slower                                                   |
| unpickle             | 9.12 us                                                | 9.17 us: 1.01x slower                                                   |
| xml_etree_iterparse  | 74.0 ms                                                | 74.9 ms: 1.01x slower                                                   |
| pickle_list          | 2.89 us                                                | 2.95 us: 1.02x slower                                                   |
| unpickle_list        | 3.02 us                                                | 3.09 us: 1.02x slower                                                   |
| json_dumps           | 6.22 ms                                                | 6.48 ms: 1.04x slower                                                   |
| unpickle_pure_python | 151 us                                                 | 158 us: 1.05x slower                                                    |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                            |

Benchmark hidden because not significant (2): xml_etree_generate, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.3 ms: 1.17x slower                                                   |
| python_startup_no_site | 9.37 ms                                                | 12.0 ms: 1.28x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.22x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.47 ms: 1.03x faster                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 70.0 us: 1.33x faster                                                   |
| comprehensions             | 14.5 us                                                | 12.0 us: 1.21x faster                                                   |
| raytrace                   | 212 ms                                                 | 176 ms: 1.21x faster                                                    |
| deltablue                  | 2.71 ms                                                | 2.44 ms: 1.11x faster                                                   |
| unpack_sequence            | 31.5 ns                                                | 28.5 ns: 1.10x faster                                                   |
| generators                 | 31.1 ms                                                | 28.4 ms: 1.09x faster                                                   |
| asyncio_tcp                | 449 ms                                                 | 412 ms: 1.09x faster                                                    |
| logging_silent             | 76.4 ns                                                | 70.5 ns: 1.08x faster                                                   |
| sqlglot_parse              | 848 us                                                 | 785 us: 1.08x faster                                                    |
| deepcopy_memo              | 27.7 us                                                | 25.8 us: 1.07x faster                                                   |
| crypto_pyaes               | 51.9 ms                                                | 48.4 ms: 1.07x faster                                                   |
| logging_simple             | 3.69 us                                                | 3.46 us: 1.06x faster                                                   |
| async_tree_none            | 266 ms                                                 | 250 ms: 1.06x faster                                                    |
| logging_format             | 3.98 us                                                | 3.79 us: 1.05x faster                                                   |
| sqlglot_transpile          | 1.02 ms                                                | 972 us: 1.05x faster                                                    |
| chaos                      | 42.5 ms                                                | 40.7 ms: 1.04x faster                                                   |
| coroutines                 | 19.2 ms                                                | 18.4 ms: 1.04x faster                                                   |
| sympy_str                  | 148 ms                                                 | 141 ms: 1.04x faster                                                    |
| regex_compile              | 77.9 ms                                                | 74.6 ms: 1.04x faster                                                   |
| json                       | 3.09 ms                                                | 2.97 ms: 1.04x faster                                                   |
| deepcopy_reduce            | 2.07 us                                                | 1.99 us: 1.04x faster                                                   |
| deepcopy                   | 235 us                                                 | 226 us: 1.04x faster                                                    |
| sympy_sum                  | 77.6 ms                                                | 74.8 ms: 1.04x faster                                                   |
| regex_effbot               | 2.64 ms                                                | 2.55 ms: 1.04x faster                                                   |
| mako                       | 7.71 ms                                                | 7.47 ms: 1.03x faster                                                   |
| xml_etree_process          | 39.7 ms                                                | 38.5 ms: 1.03x faster                                                   |
| pathlib                    | 24.2 ms                                                | 23.5 ms: 1.03x faster                                                   |
| docutils                   | 1.50 sec                                               | 1.47 sec: 1.02x faster                                                  |
| pickle_pure_python         | 200 us                                                 | 195 us: 1.02x faster                                                    |
| sympy_integrate            | 11.4 ms                                                | 11.1 ms: 1.02x faster                                                   |
| sqlglot_normalize          | 186 ms                                                 | 182 ms: 1.02x faster                                                    |
| float                      | 55.8 ms                                                | 54.8 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 517 ms: 1.02x faster                                                    |
| tomli_loads                | 1.39 sec                                               | 1.37 sec: 1.02x faster                                                  |
| regex_dna                  | 154 ms                                                 | 152 ms: 1.02x faster                                                    |
| scimark_lu                 | 76.0 ms                                                | 74.8 ms: 1.02x faster                                                   |
| nqueens                    | 62.4 ms                                                | 61.5 ms: 1.02x faster                                                   |
| async_tree_io_tg           | 669 ms                                                 | 660 ms: 1.01x faster                                                    |
| richards_super             | 36.0 ms                                                | 35.6 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 527 ms: 1.01x faster                                                    |
| bench_thread_pool          | 504 us                                                 | 499 us: 1.01x faster                                                    |
| async_generators           | 304 ms                                                 | 301 ms: 1.01x faster                                                    |
| richards                   | 32.1 ms                                                | 31.9 ms: 1.01x faster                                                   |
| json_loads                 | 17.2 us                                                | 17.1 us: 1.01x faster                                                   |
| sympy_expand               | 241 ms                                                 | 240 ms: 1.01x faster                                                    |
| dulwich_log                | 29.8 ms                                                | 29.7 ms: 1.00x faster                                                   |
| gc_traversal               | 2.40 ms                                                | 2.39 ms: 1.00x faster                                                   |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                    |
| pidigits                   | 282 ms                                                 | 283 ms: 1.00x slower                                                    |
| create_gc_cycles           | 701 us                                                 | 704 us: 1.00x slower                                                    |
| pprint_pformat             | 1.01 sec                                               | 1.01 sec: 1.00x slower                                                  |
| pickle_dict                | 18.1 us                                                | 18.1 us: 1.00x slower                                                   |
| sqlite_synth               | 1.57 us                                                | 1.58 us: 1.00x slower                                                   |
| pickle                     | 7.23 us                                                | 7.27 us: 1.01x slower                                                   |
| sqlglot_optimize           | 34.0 ms                                                | 34.2 ms: 1.01x slower                                                   |
| unpickle                   | 9.12 us                                                | 9.17 us: 1.01x slower                                                   |
| mdp                        | 1.58 sec                                               | 1.59 sec: 1.01x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 501 ms: 1.01x slower                                                    |
| xml_etree_iterparse        | 74.0 ms                                                | 74.9 ms: 1.01x slower                                                   |
| chameleon                  | 4.70 ms                                                | 4.77 ms: 1.02x slower                                                   |
| pyflate                    | 316 ms                                                 | 321 ms: 1.02x slower                                                    |
| 2to3                       | 169 ms                                                 | 173 ms: 1.02x slower                                                    |
| pycparser                  | 677 ms                                                 | 692 ms: 1.02x slower                                                    |
| spectral_norm              | 76.4 ms                                                | 78.1 ms: 1.02x slower                                                   |
| pickle_list                | 2.89 us                                                | 2.95 us: 1.02x slower                                                   |
| unpickle_list              | 3.02 us                                                | 3.09 us: 1.02x slower                                                   |
| meteor_contest             | 71.7 ms                                                | 74.3 ms: 1.03x slower                                                   |
| json_dumps                 | 6.22 ms                                                | 6.48 ms: 1.04x slower                                                   |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.27 ms: 1.04x slower                                                   |
| async_tree_io              | 668 ms                                                 | 696 ms: 1.04x slower                                                    |
| bench_mp_pool              | 44.9 ms                                                | 46.8 ms: 1.04x slower                                                   |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.30 sec: 1.04x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 327 ms: 1.05x slower                                                    |
| unpickle_pure_python       | 151 us                                                 | 158 us: 1.05x slower                                                    |
| hexiom                     | 4.54 ms                                                | 4.78 ms: 1.05x slower                                                   |
| fannkuch                   | 248 ms                                                 | 263 ms: 1.06x slower                                                    |
| scimark_monte_carlo        | 45.0 ms                                                | 47.8 ms: 1.06x slower                                                   |
| regex_v8                   | 16.0 ms                                                | 17.0 ms: 1.07x slower                                                   |
| go                         | 102 ms                                                 | 109 ms: 1.07x slower                                                    |
| scimark_fft                | 195 ms                                                 | 213 ms: 1.09x slower                                                    |
| nbody                      | 68.8 ms                                                | 75.5 ms: 1.10x slower                                                   |
| python_startup             | 11.4 ms                                                | 13.3 ms: 1.17x slower                                                   |
| scimark_sor                | 87.4 ms                                                | 106 ms: 1.21x slower                                                    |
| telco                      | 3.68 ms                                                | 4.45 ms: 1.21x slower                                                   |
| coverage                   | 38.9 ms                                                | 47.5 ms: 1.22x slower                                                   |
| python_startup_no_site     | 9.37 ms                                                | 12.0 ms: 1.28x slower                                                   |
| mypy2                      | 380 ms                                                 | 522 ms: 1.37x slower                                                    |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                            |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_none_tg, tornado_http, xml_etree_generate, xml_etree_parse, dask
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 61.38% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.14x