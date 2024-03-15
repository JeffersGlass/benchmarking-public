
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 174 ms: 1.03x slower                                                             |
| chameleon      | 4.70 ms                                                | 5.07 ms: 1.08x slower                                                            |
| docutils       | 1.50 sec                                               | 1.49 sec: 1.01x faster                                                           |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none           | 266 ms                                                 | 258 ms: 1.03x faster                                                             |
| async_tree_io_tg          | 669 ms                                                 | 677 ms: 1.01x slower                                                             |
| async_tree_memoization_tg | 323 ms                                                 | 329 ms: 1.02x slower                                                             |
| async_tree_none_tg        | 258 ms                                                 | 265 ms: 1.03x slower                                                             |
| async_tree_io             | 668 ms                                                 | 709 ms: 1.06x slower                                                             |
| async_tree_memoization    | 312 ms                                                 | 334 ms: 1.07x slower                                                             |
| Geometric mean            | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 284 ms: 1.01x slower                                                             |
| nbody          | 68.8 ms                                                | 81.9 ms: 1.19x slower                                                            |
| float          | 55.8 ms                                                | 67.0 ms: 1.20x slower                                                            |
| Geometric mean | (ref)                                                  | 1.13x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 157 ms: 1.02x slower                                                             |
| regex_compile  | 77.9 ms                                                | 81.8 ms: 1.05x slower                                                            |
| regex_effbot   | 2.64 ms                                                | 2.78 ms: 1.05x slower                                                            |
| regex_v8       | 16.0 ms                                                | 18.0 ms: 1.13x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                             |
| json_loads           | 17.2 us                                                | 17.2 us: 1.00x faster                                                            |
| unpickle             | 9.12 us                                                | 9.17 us: 1.01x slower                                                            |
| pickle               | 7.23 us                                                | 7.30 us: 1.01x slower                                                            |
| xml_etree_process    | 39.7 ms                                                | 40.6 ms: 1.02x slower                                                            |
| pickle_list          | 2.89 us                                                | 2.97 us: 1.03x slower                                                            |
| xml_etree_generate   | 55.8 ms                                                | 58.5 ms: 1.05x slower                                                            |
| json_dumps           | 6.22 ms                                                | 6.56 ms: 1.05x slower                                                            |
| unpickle_pure_python | 151 us                                                 | 164 us: 1.09x slower                                                             |
| xml_etree_iterparse  | 74.0 ms                                                | 80.8 ms: 1.09x slower                                                            |
| tomli_loads          | 1.39 sec                                               | 1.62 sec: 1.16x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (3): pickle_dict, unpickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.9 ms: 1.13x slower                                                            |
| python_startup_no_site | 9.37 ms                                                | 11.5 ms: 1.23x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.18x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 9.65 ms: 1.25x slower                                                            |

All benchmarks:
===============

| Benchmark                 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|---------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols  | 93.0 us                                                | 73.1 us: 1.27x faster                                                            |
| raytrace                  | 212 ms                                                 | 184 ms: 1.15x faster                                                             |
| generators                | 31.1 ms                                                | 28.7 ms: 1.08x faster                                                            |
| unpack_sequence           | 31.5 ns                                                | 29.2 ns: 1.08x faster                                                            |
| logging_silent            | 76.4 ns                                                | 72.3 ns: 1.06x faster                                                            |
| json                      | 3.09 ms                                                | 2.95 ms: 1.05x faster                                                            |
| sqlglot_parse             | 848 us                                                 | 810 us: 1.05x faster                                                             |
| deepcopy_memo             | 27.7 us                                                | 26.7 us: 1.04x faster                                                            |
| deepcopy_reduce           | 2.07 us                                                | 2.00 us: 1.04x faster                                                            |
| logging_format            | 3.98 us                                                | 3.85 us: 1.04x faster                                                            |
| logging_simple            | 3.69 us                                                | 3.57 us: 1.03x faster                                                            |
| deepcopy                  | 235 us                                                 | 227 us: 1.03x faster                                                             |
| async_tree_none           | 266 ms                                                 | 258 ms: 1.03x faster                                                             |
| sqlglot_transpile         | 1.02 ms                                                | 992 us: 1.03x faster                                                             |
| async_generators          | 304 ms                                                 | 297 ms: 1.02x faster                                                             |
| pickle_pure_python        | 200 us                                                 | 196 us: 1.02x faster                                                             |
| scimark_lu                | 76.0 ms                                                | 75.4 ms: 1.01x faster                                                            |
| docutils                  | 1.50 sec                                               | 1.49 sec: 1.01x faster                                                           |
| json_loads                | 17.2 us                                                | 17.2 us: 1.00x faster                                                            |
| asyncio_websockets        | 409 ms                                                 | 409 ms: 1.00x faster                                                             |
| gc_traversal              | 2.40 ms                                                | 2.40 ms: 1.00x slower                                                            |
| create_gc_cycles          | 701 us                                                 | 704 us: 1.00x slower                                                             |
| unpickle                  | 9.12 us                                                | 9.17 us: 1.01x slower                                                            |
| pidigits                  | 282 ms                                                 | 284 ms: 1.01x slower                                                             |
| sympy_str                 | 148 ms                                                 | 149 ms: 1.01x slower                                                             |
| dulwich_log               | 29.8 ms                                                | 30.0 ms: 1.01x slower                                                            |
| pickle                    | 7.23 us                                                | 7.30 us: 1.01x slower                                                            |
| bench_thread_pool         | 504 us                                                 | 510 us: 1.01x slower                                                             |
| async_tree_io_tg          | 669 ms                                                 | 677 ms: 1.01x slower                                                             |
| richards_super            | 36.0 ms                                                | 36.5 ms: 1.01x slower                                                            |
| bench_mp_pool             | 44.9 ms                                                | 45.4 ms: 1.01x slower                                                            |
| sympy_integrate           | 11.4 ms                                                | 11.5 ms: 1.01x slower                                                            |
| regex_dna                 | 154 ms                                                 | 157 ms: 1.02x slower                                                             |
| sympy_expand              | 241 ms                                                 | 245 ms: 1.02x slower                                                             |
| asyncio_tcp_ssl           | 1.24 sec                                               | 1.27 sec: 1.02x slower                                                           |
| richards                  | 32.1 ms                                                | 32.8 ms: 1.02x slower                                                            |
| async_tree_memoization_tg | 323 ms                                                 | 329 ms: 1.02x slower                                                             |
| mdp                       | 1.58 sec                                               | 1.61 sec: 1.02x slower                                                           |
| sympy_sum                 | 77.6 ms                                                | 79.3 ms: 1.02x slower                                                            |
| coroutines                | 19.2 ms                                                | 19.7 ms: 1.02x slower                                                            |
| dask                      | 222 ms                                                 | 227 ms: 1.02x slower                                                             |
| xml_etree_process         | 39.7 ms                                                | 40.6 ms: 1.02x slower                                                            |
| 2to3                      | 169 ms                                                 | 174 ms: 1.03x slower                                                             |
| pickle_list               | 2.89 us                                                | 2.97 us: 1.03x slower                                                            |
| sqlglot_normalize         | 186 ms                                                 | 191 ms: 1.03x slower                                                             |
| pathlib                   | 24.2 ms                                                | 24.9 ms: 1.03x slower                                                            |
| async_tree_none_tg        | 258 ms                                                 | 265 ms: 1.03x slower                                                             |
| pycparser                 | 677 ms                                                 | 701 ms: 1.04x slower                                                             |
| comprehensions            | 14.5 us                                                | 15.1 us: 1.04x slower                                                            |
| xml_etree_generate        | 55.8 ms                                                | 58.5 ms: 1.05x slower                                                            |
| sqlite_synth              | 1.57 us                                                | 1.65 us: 1.05x slower                                                            |
| regex_compile             | 77.9 ms                                                | 81.8 ms: 1.05x slower                                                            |
| regex_effbot              | 2.64 ms                                                | 2.78 ms: 1.05x slower                                                            |
| json_dumps                | 6.22 ms                                                | 6.56 ms: 1.05x slower                                                            |
| sqlglot_optimize          | 34.0 ms                                                | 36.0 ms: 1.06x slower                                                            |
| async_tree_io             | 668 ms                                                 | 709 ms: 1.06x slower                                                             |
| crypto_pyaes              | 51.9 ms                                                | 55.2 ms: 1.06x slower                                                            |
| chaos                     | 42.5 ms                                                | 45.5 ms: 1.07x slower                                                            |
| async_tree_memoization    | 312 ms                                                 | 334 ms: 1.07x slower                                                             |
| meteor_contest            | 71.7 ms                                                | 77.1 ms: 1.08x slower                                                            |
| nqueens                   | 62.4 ms                                                | 67.1 ms: 1.08x slower                                                            |
| chameleon                 | 4.70 ms                                                | 5.07 ms: 1.08x slower                                                            |
| unpickle_pure_python      | 151 us                                                 | 164 us: 1.09x slower                                                             |
| xml_etree_iterparse       | 74.0 ms                                                | 80.8 ms: 1.09x slower                                                            |
| go                        | 102 ms                                                 | 111 ms: 1.09x slower                                                             |
| python_startup            | 11.4 ms                                                | 12.9 ms: 1.13x slower                                                            |
| regex_v8                  | 16.0 ms                                                | 18.0 ms: 1.13x slower                                                            |
| pprint_safe_repr          | 497 ms                                                 | 567 ms: 1.14x slower                                                             |
| pprint_pformat            | 1.01 sec                                               | 1.16 sec: 1.15x slower                                                           |
| tomli_loads               | 1.39 sec                                               | 1.62 sec: 1.16x slower                                                           |
| pyflate                   | 316 ms                                                 | 367 ms: 1.16x slower                                                             |
| nbody                     | 68.8 ms                                                | 81.9 ms: 1.19x slower                                                            |
| scimark_fft               | 195 ms                                                 | 233 ms: 1.19x slower                                                             |
| float                     | 55.8 ms                                                | 67.0 ms: 1.20x slower                                                            |
| coverage                  | 38.9 ms                                                | 47.1 ms: 1.21x slower                                                            |
| scimark_sor               | 87.4 ms                                                | 106 ms: 1.21x slower                                                             |
| python_startup_no_site    | 9.37 ms                                                | 11.5 ms: 1.23x slower                                                            |
| scimark_monte_carlo       | 45.0 ms                                                | 56.1 ms: 1.25x slower                                                            |
| mako                      | 7.71 ms                                                | 9.65 ms: 1.25x slower                                                            |
| telco                     | 3.68 ms                                                | 4.63 ms: 1.26x slower                                                            |
| scimark_sparse_mat_mult   | 3.14 ms                                                | 3.96 ms: 1.26x slower                                                            |
| spectral_norm             | 76.4 ms                                                | 96.6 ms: 1.26x slower                                                            |
| fannkuch                  | 248 ms                                                 | 318 ms: 1.28x slower                                                             |
| hexiom                    | 4.54 ms                                                | 5.87 ms: 1.29x slower                                                            |
| deltablue                 | 2.71 ms                                                | 3.52 ms: 1.30x slower                                                            |
| mypy2                     | 380 ms                                                 | 525 ms: 1.38x slower                                                             |
| Geometric mean            | (ref)                                                  | 1.05x slower                                                                     |

Benchmark hidden because not significant (7): asyncio_tcp, pickle_dict, unpickle_list, async_tree_cpu_io_mixed, tornado_http, async_tree_cpu_io_mixed_tg, xml_etree_parse
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.01x