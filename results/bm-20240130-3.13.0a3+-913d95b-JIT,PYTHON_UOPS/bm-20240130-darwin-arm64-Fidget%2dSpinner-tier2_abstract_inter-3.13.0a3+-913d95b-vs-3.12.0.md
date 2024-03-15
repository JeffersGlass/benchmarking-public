
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.01x slower
- HPT reliability: 98.92%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 175 ms: 1.03x slower                                                             |
| chameleon      | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                            |
| docutils       | 1.50 sec                                               | 1.48 sec: 1.02x faster                                                           |
| Geometric mean | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 266 ms                                                 | 252 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed | 526 ms                                                 | 519 ms: 1.01x faster                                                             |
| async_tree_none_tg      | 258 ms                                                 | 259 ms: 1.01x slower                                                             |
| async_tree_io           | 668 ms                                                 | 698 ms: 1.04x slower                                                             |
| async_tree_memoization  | 312 ms                                                 | 328 ms: 1.05x slower                                                             |
| Geometric mean          | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                             |
| nbody          | 68.8 ms                                                | 74.8 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.57 ms: 1.03x faster                                                            |
| regex_compile  | 77.9 ms                                                | 76.2 ms: 1.02x faster                                                            |
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                             |
| regex_v8       | 16.0 ms                                                | 17.2 ms: 1.07x slower                                                            |
| Geometric mean | (ref)                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 197 us: 1.02x faster                                                             |
| json_loads           | 17.2 us                                                | 17.1 us: 1.01x faster                                                            |
| xml_etree_process    | 39.7 ms                                                | 39.4 ms: 1.01x faster                                                            |
| unpickle             | 9.12 us                                                | 9.07 us: 1.01x faster                                                            |
| xml_etree_generate   | 55.8 ms                                                | 55.7 ms: 1.00x faster                                                            |
| pickle_dict          | 18.1 us                                                | 18.2 us: 1.01x slower                                                            |
| tomli_loads          | 1.39 sec                                               | 1.41 sec: 1.01x slower                                                           |
| pickle               | 7.23 us                                                | 7.36 us: 1.02x slower                                                            |
| unpickle_list        | 3.02 us                                                | 3.09 us: 1.02x slower                                                            |
| xml_etree_iterparse  | 74.0 ms                                                | 76.4 ms: 1.03x slower                                                            |
| pickle_list          | 2.89 us                                                | 2.99 us: 1.04x slower                                                            |
| json_dumps           | 6.22 ms                                                | 6.58 ms: 1.06x slower                                                            |
| unpickle_pure_python | 151 us                                                 | 160 us: 1.06x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.1 ms: 1.15x slower                                                            |
| python_startup_no_site | 9.37 ms                                                | 11.8 ms: 1.25x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.20x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.94 ms: 1.03x slower                                                            |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 72.0 us: 1.29x faster                                                            |
| raytrace                 | 212 ms                                                 | 177 ms: 1.19x faster                                                             |
| comprehensions           | 14.5 us                                                | 12.7 us: 1.14x faster                                                            |
| unpack_sequence          | 31.5 ns                                                | 28.3 ns: 1.11x faster                                                            |
| asyncio_tcp              | 449 ms                                                 | 404 ms: 1.11x faster                                                             |
| generators               | 31.1 ms                                                | 28.1 ms: 1.11x faster                                                            |
| logging_silent           | 76.4 ns                                                | 70.0 ns: 1.09x faster                                                            |
| deltablue                | 2.71 ms                                                | 2.52 ms: 1.07x faster                                                            |
| deepcopy_memo            | 27.7 us                                                | 25.9 us: 1.07x faster                                                            |
| sqlglot_parse            | 848 us                                                 | 796 us: 1.07x faster                                                             |
| logging_simple           | 3.69 us                                                | 3.49 us: 1.06x faster                                                            |
| async_tree_none          | 266 ms                                                 | 252 ms: 1.05x faster                                                             |
| crypto_pyaes             | 51.9 ms                                                | 49.3 ms: 1.05x faster                                                            |
| logging_format           | 3.98 us                                                | 3.80 us: 1.05x faster                                                            |
| deepcopy_reduce          | 2.07 us                                                | 1.98 us: 1.04x faster                                                            |
| sqlglot_transpile        | 1.02 ms                                                | 980 us: 1.04x faster                                                             |
| deepcopy                 | 235 us                                                 | 226 us: 1.04x faster                                                             |
| json                     | 3.09 ms                                                | 2.97 ms: 1.04x faster                                                            |
| sympy_str                | 148 ms                                                 | 143 ms: 1.04x faster                                                             |
| regex_effbot             | 2.64 ms                                                | 2.57 ms: 1.03x faster                                                            |
| regex_compile            | 77.9 ms                                                | 76.2 ms: 1.02x faster                                                            |
| regex_dna                | 154 ms                                                 | 152 ms: 1.02x faster                                                             |
| docutils                 | 1.50 sec                                               | 1.48 sec: 1.02x faster                                                           |
| pickle_pure_python       | 200 us                                                 | 197 us: 1.02x faster                                                             |
| chaos                    | 42.5 ms                                                | 41.9 ms: 1.01x faster                                                            |
| async_tree_cpu_io_mixed  | 526 ms                                                 | 519 ms: 1.01x faster                                                             |
| sympy_sum                | 77.6 ms                                                | 76.7 ms: 1.01x faster                                                            |
| scimark_lu               | 76.0 ms                                                | 75.1 ms: 1.01x faster                                                            |
| richards_super           | 36.0 ms                                                | 35.7 ms: 1.01x faster                                                            |
| json_loads               | 17.2 us                                                | 17.1 us: 1.01x faster                                                            |
| richards                 | 32.1 ms                                                | 31.9 ms: 1.01x faster                                                            |
| xml_etree_process        | 39.7 ms                                                | 39.4 ms: 1.01x faster                                                            |
| unpickle                 | 9.12 us                                                | 9.07 us: 1.01x faster                                                            |
| sqlglot_normalize        | 186 ms                                                 | 185 ms: 1.01x faster                                                             |
| sympy_integrate          | 11.4 ms                                                | 11.3 ms: 1.00x faster                                                            |
| xml_etree_generate       | 55.8 ms                                                | 55.7 ms: 1.00x faster                                                            |
| gc_traversal             | 2.40 ms                                                | 2.41 ms: 1.00x slower                                                            |
| bench_thread_pool        | 504 us                                                 | 506 us: 1.00x slower                                                             |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                             |
| create_gc_cycles         | 701 us                                                 | 706 us: 1.01x slower                                                             |
| nqueens                  | 62.4 ms                                                | 62.8 ms: 1.01x slower                                                            |
| async_generators         | 304 ms                                                 | 306 ms: 1.01x slower                                                             |
| async_tree_none_tg       | 258 ms                                                 | 259 ms: 1.01x slower                                                             |
| pickle_dict              | 18.1 us                                                | 18.2 us: 1.01x slower                                                            |
| dulwich_log              | 29.8 ms                                                | 30.1 ms: 1.01x slower                                                            |
| sqlite_synth             | 1.57 us                                                | 1.59 us: 1.01x slower                                                            |
| tomli_loads              | 1.39 sec                                               | 1.41 sec: 1.01x slower                                                           |
| dask                     | 222 ms                                                 | 226 ms: 1.02x slower                                                             |
| pickle                   | 7.23 us                                                | 7.36 us: 1.02x slower                                                            |
| unpickle_list            | 3.02 us                                                | 3.09 us: 1.02x slower                                                            |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.27 sec: 1.02x slower                                                           |
| sqlglot_optimize         | 34.0 ms                                                | 34.9 ms: 1.03x slower                                                            |
| pycparser                | 677 ms                                                 | 697 ms: 1.03x slower                                                             |
| mako                     | 7.71 ms                                                | 7.94 ms: 1.03x slower                                                            |
| mdp                      | 1.58 sec                                               | 1.63 sec: 1.03x slower                                                           |
| xml_etree_iterparse      | 74.0 ms                                                | 76.4 ms: 1.03x slower                                                            |
| 2to3                     | 169 ms                                                 | 175 ms: 1.03x slower                                                             |
| pickle_list              | 2.89 us                                                | 2.99 us: 1.04x slower                                                            |
| meteor_contest           | 71.7 ms                                                | 74.3 ms: 1.04x slower                                                            |
| pyflate                  | 316 ms                                                 | 328 ms: 1.04x slower                                                             |
| chameleon                | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                            |
| async_tree_io            | 668 ms                                                 | 698 ms: 1.04x slower                                                             |
| async_tree_memoization   | 312 ms                                                 | 328 ms: 1.05x slower                                                             |
| spectral_norm            | 76.4 ms                                                | 80.7 ms: 1.06x slower                                                            |
| bench_mp_pool            | 44.9 ms                                                | 47.4 ms: 1.06x slower                                                            |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.32 ms: 1.06x slower                                                            |
| json_dumps               | 6.22 ms                                                | 6.58 ms: 1.06x slower                                                            |
| pprint_safe_repr         | 497 ms                                                 | 526 ms: 1.06x slower                                                             |
| pprint_pformat           | 1.01 sec                                               | 1.07 sec: 1.06x slower                                                           |
| unpickle_pure_python     | 151 us                                                 | 160 us: 1.06x slower                                                             |
| regex_v8                 | 16.0 ms                                                | 17.2 ms: 1.07x slower                                                            |
| go                       | 102 ms                                                 | 110 ms: 1.08x slower                                                             |
| nbody                    | 68.8 ms                                                | 74.8 ms: 1.09x slower                                                            |
| scimark_monte_carlo      | 45.0 ms                                                | 49.4 ms: 1.10x slower                                                            |
| scimark_fft              | 195 ms                                                 | 215 ms: 1.10x slower                                                             |
| hexiom                   | 4.54 ms                                                | 5.14 ms: 1.13x slower                                                            |
| python_startup           | 11.4 ms                                                | 13.1 ms: 1.15x slower                                                            |
| fannkuch                 | 248 ms                                                 | 295 ms: 1.19x slower                                                             |
| scimark_sor              | 87.4 ms                                                | 107 ms: 1.23x slower                                                             |
| coverage                 | 38.9 ms                                                | 48.0 ms: 1.24x slower                                                            |
| telco                    | 3.68 ms                                                | 4.59 ms: 1.25x slower                                                            |
| python_startup_no_site   | 9.37 ms                                                | 11.8 ms: 1.25x slower                                                            |
| mypy2                    | 380 ms                                                 | 529 ms: 1.39x slower                                                             |
| Geometric mean           | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (10): async_tree_cpu_io_mixed_tg, float, async_tree_io_tg, async_tree_memoization_tg, asyncio_websockets, sympy_expand, coroutines, pathlib, xml_etree_parse, tornado_http
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 98.92% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.15x