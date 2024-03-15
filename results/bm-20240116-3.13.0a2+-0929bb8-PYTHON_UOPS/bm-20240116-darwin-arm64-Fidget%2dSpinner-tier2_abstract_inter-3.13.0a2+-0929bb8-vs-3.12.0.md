
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 0929bb8
- commit date: 2024-01-16
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.27x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 176 ms: 1.04x slower                                                             |
| chameleon      | 4.70 ms                                                | 5.16 ms: 1.10x slower                                                            |
| docutils       | 1.50 sec                                               | 1.51 sec: 1.00x slower                                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 259 ms: 1.02x faster                                                             |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 537 ms: 1.01x slower                                                             |
| async_tree_io_tg           | 669 ms                                                 | 687 ms: 1.03x slower                                                             |
| async_tree_none_tg         | 258 ms                                                 | 266 ms: 1.03x slower                                                             |
| async_tree_memoization_tg  | 323 ms                                                 | 334 ms: 1.03x slower                                                             |
| async_tree_io              | 668 ms                                                 | 716 ms: 1.07x slower                                                             |
| async_tree_memoization     | 312 ms                                                 | 337 ms: 1.08x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                                             |
| float          | 55.8 ms                                                | 68.1 ms: 1.22x slower                                                            |
| nbody          | 68.8 ms                                                | 118 ms: 1.71x slower                                                             |
| Geometric mean | (ref)                                                  | 1.28x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 156 ms: 1.01x slower                                                             |
| regex_effbot   | 2.64 ms                                                | 2.75 ms: 1.04x slower                                                            |
| regex_compile  | 77.9 ms                                                | 82.0 ms: 1.05x slower                                                            |
| regex_v8       | 16.0 ms                                                | 17.9 ms: 1.12x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 197 us: 1.01x faster                                                             |
| json_loads           | 17.2 us                                                | 17.1 us: 1.01x faster                                                            |
| unpickle_list        | 3.02 us                                                | 3.00 us: 1.01x faster                                                            |
| unpickle             | 9.12 us                                                | 9.17 us: 1.01x slower                                                            |
| pickle_dict          | 18.1 us                                                | 18.2 us: 1.01x slower                                                            |
| pickle_list          | 2.89 us                                                | 2.95 us: 1.02x slower                                                            |
| xml_etree_process    | 39.7 ms                                                | 40.6 ms: 1.02x slower                                                            |
| pickle               | 7.23 us                                                | 7.48 us: 1.04x slower                                                            |
| json_dumps           | 6.22 ms                                                | 6.58 ms: 1.06x slower                                                            |
| xml_etree_generate   | 55.8 ms                                                | 59.4 ms: 1.06x slower                                                            |
| xml_etree_iterparse  | 74.0 ms                                                | 80.4 ms: 1.09x slower                                                            |
| unpickle_pure_python | 151 us                                                 | 164 us: 1.09x slower                                                             |
| tomli_loads          | 1.39 sec                                               | 1.64 sec: 1.18x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.3 ms: 1.08x slower                                                            |
| python_startup_no_site | 9.37 ms                                                | 11.0 ms: 1.17x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.13x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 9.66 ms: 1.25x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 74.3 us: 1.25x faster                                                            |
| asyncio_tcp                | 449 ms                                                 | 374 ms: 1.20x faster                                                             |
| raytrace                   | 212 ms                                                 | 186 ms: 1.14x faster                                                             |
| generators                 | 31.1 ms                                                | 28.9 ms: 1.08x faster                                                            |
| logging_silent             | 76.4 ns                                                | 72.1 ns: 1.06x faster                                                            |
| unpack_sequence            | 31.5 ns                                                | 29.9 ns: 1.05x faster                                                            |
| json                       | 3.09 ms                                                | 2.94 ms: 1.05x faster                                                            |
| sqlglot_parse              | 848 us                                                 | 813 us: 1.04x faster                                                             |
| deepcopy_reduce            | 2.07 us                                                | 1.99 us: 1.04x faster                                                            |
| deepcopy                   | 235 us                                                 | 226 us: 1.04x faster                                                             |
| logging_format             | 3.98 us                                                | 3.85 us: 1.04x faster                                                            |
| deepcopy_memo              | 27.7 us                                                | 26.7 us: 1.03x faster                                                            |
| logging_simple             | 3.69 us                                                | 3.57 us: 1.03x faster                                                            |
| sqlglot_transpile          | 1.02 ms                                                | 994 us: 1.03x faster                                                             |
| async_tree_none            | 266 ms                                                 | 259 ms: 1.02x faster                                                             |
| async_generators           | 304 ms                                                 | 299 ms: 1.02x faster                                                             |
| pickle_pure_python         | 200 us                                                 | 197 us: 1.01x faster                                                             |
| json_loads                 | 17.2 us                                                | 17.1 us: 1.01x faster                                                            |
| unpickle_list              | 3.02 us                                                | 3.00 us: 1.01x faster                                                            |
| gc_traversal               | 2.40 ms                                                | 2.40 ms: 1.00x slower                                                            |
| create_gc_cycles           | 701 us                                                 | 704 us: 1.00x slower                                                             |
| docutils                   | 1.50 sec                                               | 1.51 sec: 1.00x slower                                                           |
| unpickle                   | 9.12 us                                                | 9.17 us: 1.01x slower                                                            |
| pidigits                   | 282 ms                                                 | 284 ms: 1.01x slower                                                             |
| pickle_dict                | 18.1 us                                                | 18.2 us: 1.01x slower                                                            |
| scimark_lu                 | 76.0 ms                                                | 76.5 ms: 1.01x slower                                                            |
| regex_dna                  | 154 ms                                                 | 156 ms: 1.01x slower                                                             |
| dulwich_log                | 29.8 ms                                                | 30.1 ms: 1.01x slower                                                            |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 537 ms: 1.01x slower                                                             |
| sympy_str                  | 148 ms                                                 | 149 ms: 1.01x slower                                                             |
| bench_mp_pool              | 44.9 ms                                                | 45.4 ms: 1.01x slower                                                            |
| richards                   | 32.1 ms                                                | 32.6 ms: 1.01x slower                                                            |
| sympy_expand               | 241 ms                                                 | 246 ms: 1.02x slower                                                             |
| pickle_list                | 2.89 us                                                | 2.95 us: 1.02x slower                                                            |
| xml_etree_process          | 39.7 ms                                                | 40.6 ms: 1.02x slower                                                            |
| richards_super             | 36.0 ms                                                | 36.9 ms: 1.02x slower                                                            |
| sqlglot_normalize          | 186 ms                                                 | 190 ms: 1.03x slower                                                             |
| async_tree_io_tg           | 669 ms                                                 | 687 ms: 1.03x slower                                                             |
| bench_thread_pool          | 504 us                                                 | 517 us: 1.03x slower                                                             |
| mdp                        | 1.58 sec                                               | 1.62 sec: 1.03x slower                                                           |
| dask                       | 222 ms                                                 | 228 ms: 1.03x slower                                                             |
| coroutines                 | 19.2 ms                                                | 19.8 ms: 1.03x slower                                                            |
| async_tree_none_tg         | 258 ms                                                 | 266 ms: 1.03x slower                                                             |
| async_tree_memoization_tg  | 323 ms                                                 | 334 ms: 1.03x slower                                                             |
| pickle                     | 7.23 us                                                | 7.48 us: 1.04x slower                                                            |
| sympy_integrate            | 11.4 ms                                                | 11.8 ms: 1.04x slower                                                            |
| 2to3                       | 169 ms                                                 | 176 ms: 1.04x slower                                                             |
| sympy_sum                  | 77.6 ms                                                | 80.6 ms: 1.04x slower                                                            |
| regex_effbot               | 2.64 ms                                                | 2.75 ms: 1.04x slower                                                            |
| pycparser                  | 677 ms                                                 | 706 ms: 1.04x slower                                                             |
| sqlite_synth               | 1.57 us                                                | 1.64 us: 1.04x slower                                                            |
| regex_compile              | 77.9 ms                                                | 82.0 ms: 1.05x slower                                                            |
| crypto_pyaes               | 51.9 ms                                                | 54.7 ms: 1.06x slower                                                            |
| pathlib                    | 24.2 ms                                                | 25.6 ms: 1.06x slower                                                            |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.31 sec: 1.06x slower                                                           |
| json_dumps                 | 6.22 ms                                                | 6.58 ms: 1.06x slower                                                            |
| sqlglot_optimize           | 34.0 ms                                                | 36.0 ms: 1.06x slower                                                            |
| xml_etree_generate         | 55.8 ms                                                | 59.4 ms: 1.06x slower                                                            |
| meteor_contest             | 71.7 ms                                                | 76.7 ms: 1.07x slower                                                            |
| async_tree_io              | 668 ms                                                 | 716 ms: 1.07x slower                                                             |
| async_tree_memoization     | 312 ms                                                 | 337 ms: 1.08x slower                                                             |
| python_startup             | 11.4 ms                                                | 12.3 ms: 1.08x slower                                                            |
| comprehensions             | 14.5 us                                                | 15.7 us: 1.08x slower                                                            |
| nqueens                    | 62.4 ms                                                | 67.7 ms: 1.08x slower                                                            |
| xml_etree_iterparse        | 74.0 ms                                                | 80.4 ms: 1.09x slower                                                            |
| unpickle_pure_python       | 151 us                                                 | 164 us: 1.09x slower                                                             |
| go                         | 102 ms                                                 | 111 ms: 1.09x slower                                                             |
| chameleon                  | 4.70 ms                                                | 5.16 ms: 1.10x slower                                                            |
| regex_v8                   | 16.0 ms                                                | 17.9 ms: 1.12x slower                                                            |
| chaos                      | 42.5 ms                                                | 48.4 ms: 1.14x slower                                                            |
| pyflate                    | 316 ms                                                 | 366 ms: 1.16x slower                                                             |
| python_startup_no_site     | 9.37 ms                                                | 11.0 ms: 1.17x slower                                                            |
| tomli_loads                | 1.39 sec                                               | 1.64 sec: 1.18x slower                                                           |
| pprint_safe_repr           | 497 ms                                                 | 590 ms: 1.19x slower                                                             |
| pprint_pformat             | 1.01 sec                                               | 1.21 sec: 1.19x slower                                                           |
| float                      | 55.8 ms                                                | 68.1 ms: 1.22x slower                                                            |
| coverage                   | 38.9 ms                                                | 47.4 ms: 1.22x slower                                                            |
| scimark_sor                | 87.4 ms                                                | 107 ms: 1.23x slower                                                             |
| mako                       | 7.71 ms                                                | 9.66 ms: 1.25x slower                                                            |
| scimark_monte_carlo        | 45.0 ms                                                | 57.1 ms: 1.27x slower                                                            |
| telco                      | 3.68 ms                                                | 4.68 ms: 1.27x slower                                                            |
| fannkuch                   | 248 ms                                                 | 316 ms: 1.27x slower                                                             |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 4.06 ms: 1.30x slower                                                            |
| scimark_fft                | 195 ms                                                 | 255 ms: 1.31x slower                                                             |
| hexiom                     | 4.54 ms                                                | 5.97 ms: 1.31x slower                                                            |
| deltablue                  | 2.71 ms                                                | 3.58 ms: 1.32x slower                                                            |
| spectral_norm              | 76.4 ms                                                | 101 ms: 1.33x slower                                                             |
| mypy2                      | 380 ms                                                 | 529 ms: 1.39x slower                                                             |
| nbody                      | 68.8 ms                                                | 118 ms: 1.71x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.06x slower                                                                     |

Benchmark hidden because not significant (4): asyncio_websockets, tornado_http, async_tree_cpu_io_mixed, xml_etree_parse
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.27x