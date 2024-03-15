
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.20x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 175 ms: 1.14x slower                                                             |
| chameleon      | 4.30 ms                                                | 4.89 ms: 1.14x slower                                                            |
| docutils       | 1.43 sec                                               | 1.48 sec: 1.03x slower                                                           |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                             |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                                             |
| async_tree_io_tg           | 724 ms                                                 | 668 ms: 1.08x faster                                                             |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                                             |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                                     |

Benchmark hidden because not significant (3): async_tree_memoization, async_tree_io, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                                             |
| float          | 50.8 ms                                                | 55.7 ms: 1.10x slower                                                            |
| nbody          | 61.7 ms                                                | 74.8 ms: 1.21x slower                                                            |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.02x slower                                                             |
| regex_compile  | 72.8 ms                                                | 76.2 ms: 1.05x slower                                                            |
| regex_effbot   | 2.43 ms                                                | 2.57 ms: 1.06x slower                                                            |
| regex_v8       | 15.1 ms                                                | 17.2 ms: 1.13x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.58 ms: 1.14x faster                                                            |
| pickle_pure_python   | 191 us                                                 | 197 us: 1.03x slower                                                             |
| pickle               | 6.98 us                                                | 7.36 us: 1.05x slower                                                            |
| pickle_dict          | 17.1 us                                                | 18.2 us: 1.06x slower                                                            |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                                             |
| unpickle_pure_python | 149 us                                                 | 160 us: 1.08x slower                                                             |
| unpickle             | 8.29 us                                                | 9.07 us: 1.09x slower                                                            |
| pickle_list          | 2.70 us                                                | 2.99 us: 1.11x slower                                                            |
| tomli_loads          | 1.27 sec                                               | 1.41 sec: 1.11x slower                                                           |
| json_loads           | 15.3 us                                                | 17.1 us: 1.11x slower                                                            |
| xml_etree_iterparse  | 68.3 ms                                                | 76.4 ms: 1.12x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.09 us: 1.15x slower                                                            |
| xml_etree_process    | 33.6 ms                                                | 39.4 ms: 1.17x slower                                                            |
| xml_etree_generate   | 45.8 ms                                                | 55.7 ms: 1.22x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.1 ms: 1.22x slower                                                            |
| python_startup_no_site | 8.57 ms                                                | 11.8 ms: 1.37x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.29x slower                                                                     |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240130-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 72.0 us: 4.18x faster                                                            |
| asyncio_tcp                | 643 ms                                                 | 404 ms: 1.59x faster                                                             |
| unpack_sequence            | 33.6 ns                                                | 28.3 ns: 1.19x faster                                                            |
| raytrace                   | 206 ms                                                 | 177 ms: 1.16x faster                                                             |
| json_dumps                 | 7.53 ms                                                | 6.58 ms: 1.14x faster                                                            |
| comprehensions             | 14.4 us                                                | 12.7 us: 1.13x faster                                                            |
| chaos                      | 47.4 ms                                                | 41.9 ms: 1.13x faster                                                            |
| sqlglot_parse              | 890 us                                                 | 796 us: 1.12x faster                                                             |
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                             |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.27 sec: 1.10x faster                                                           |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                                             |
| deltablue                  | 2.75 ms                                                | 2.52 ms: 1.09x faster                                                            |
| async_tree_io_tg           | 724 ms                                                 | 668 ms: 1.08x faster                                                             |
| generators                 | 30.3 ms                                                | 28.1 ms: 1.08x faster                                                            |
| sqlglot_transpile          | 1.05 ms                                                | 980 us: 1.07x faster                                                             |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                                             |
| sympy_sum                  | 80.2 ms                                                | 76.7 ms: 1.05x faster                                                            |
| richards_super             | 37.3 ms                                                | 35.7 ms: 1.04x faster                                                            |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                                             |
| sympy_str                  | 144 ms                                                 | 143 ms: 1.01x faster                                                             |
| create_gc_cycles           | 711 us                                                 | 706 us: 1.01x faster                                                             |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                                             |
| sympy_integrate            | 11.3 ms                                                | 11.3 ms: 1.01x slower                                                            |
| deepcopy_memo              | 25.7 us                                                | 25.9 us: 1.01x slower                                                            |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                                             |
| gc_traversal               | 2.38 ms                                                | 2.41 ms: 1.01x slower                                                            |
| logging_simple             | 3.41 us                                                | 3.49 us: 1.02x slower                                                            |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.02x slower                                                             |
| richards                   | 31.1 ms                                                | 31.9 ms: 1.03x slower                                                            |
| pickle_pure_python         | 191 us                                                 | 197 us: 1.03x slower                                                             |
| dask                       | 219 ms                                                 | 226 ms: 1.03x slower                                                             |
| docutils                   | 1.43 sec                                               | 1.48 sec: 1.03x slower                                                           |
| logging_format             | 3.67 us                                                | 3.80 us: 1.04x slower                                                            |
| crypto_pyaes               | 47.5 ms                                                | 49.3 ms: 1.04x slower                                                            |
| go                         | 105 ms                                                 | 110 ms: 1.04x slower                                                             |
| regex_compile              | 72.8 ms                                                | 76.2 ms: 1.05x slower                                                            |
| meteor_contest             | 71.1 ms                                                | 74.3 ms: 1.05x slower                                                            |
| pathlib                    | 23.2 ms                                                | 24.3 ms: 1.05x slower                                                            |
| deepcopy                   | 215 us                                                 | 226 us: 1.05x slower                                                             |
| logging_silent             | 66.5 ns                                                | 70.0 ns: 1.05x slower                                                            |
| dulwich_log                | 28.6 ms                                                | 30.1 ms: 1.05x slower                                                            |
| sympy_expand               | 229 ms                                                 | 241 ms: 1.05x slower                                                             |
| pickle                     | 6.98 us                                                | 7.36 us: 1.05x slower                                                            |
| pycparser                  | 659 ms                                                 | 697 ms: 1.06x slower                                                             |
| regex_effbot               | 2.43 ms                                                | 2.57 ms: 1.06x slower                                                            |
| pickle_dict                | 17.1 us                                                | 18.2 us: 1.06x slower                                                            |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                                             |
| unpickle_pure_python       | 149 us                                                 | 160 us: 1.08x slower                                                             |
| json                       | 2.75 ms                                                | 2.97 ms: 1.08x slower                                                            |
| bench_thread_pool          | 465 us                                                 | 506 us: 1.09x slower                                                             |
| unpickle                   | 8.29 us                                                | 9.07 us: 1.09x slower                                                            |
| coverage                   | 43.9 ms                                                | 48.0 ms: 1.09x slower                                                            |
| float                      | 50.8 ms                                                | 55.7 ms: 1.10x slower                                                            |
| pprint_pformat             | 979 ms                                                 | 1.07 sec: 1.10x slower                                                           |
| mdp                        | 1.48 sec                                               | 1.63 sec: 1.10x slower                                                           |
| pprint_safe_repr           | 478 ms                                                 | 526 ms: 1.10x slower                                                             |
| deepcopy_reduce            | 1.79 us                                                | 1.98 us: 1.10x slower                                                            |
| scimark_lu                 | 67.7 ms                                                | 75.1 ms: 1.11x slower                                                            |
| pickle_list                | 2.70 us                                                | 2.99 us: 1.11x slower                                                            |
| tomli_loads                | 1.27 sec                                               | 1.41 sec: 1.11x slower                                                           |
| json_loads                 | 15.3 us                                                | 17.1 us: 1.11x slower                                                            |
| xml_etree_iterparse        | 68.3 ms                                                | 76.4 ms: 1.12x slower                                                            |
| coroutines                 | 17.2 ms                                                | 19.3 ms: 1.12x slower                                                            |
| nqueens                    | 55.9 ms                                                | 62.8 ms: 1.12x slower                                                            |
| hexiom                     | 4.58 ms                                                | 5.14 ms: 1.12x slower                                                            |
| regex_v8                   | 15.1 ms                                                | 17.2 ms: 1.13x slower                                                            |
| 2to3                       | 154 ms                                                 | 175 ms: 1.14x slower                                                             |
| scimark_monte_carlo        | 43.5 ms                                                | 49.4 ms: 1.14x slower                                                            |
| chameleon                  | 4.30 ms                                                | 4.89 ms: 1.14x slower                                                            |
| sqlglot_normalize          | 162 ms                                                 | 185 ms: 1.14x slower                                                             |
| unpickle_list              | 2.69 us                                                | 3.09 us: 1.15x slower                                                            |
| pyflate                    | 284 ms                                                 | 328 ms: 1.16x slower                                                             |
| bench_mp_pool              | 41.0 ms                                                | 47.4 ms: 1.16x slower                                                            |
| xml_etree_process          | 33.6 ms                                                | 39.4 ms: 1.17x slower                                                            |
| sqlglot_optimize           | 29.6 ms                                                | 34.9 ms: 1.18x slower                                                            |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.32 ms: 1.18x slower                                                            |
| nbody                      | 61.7 ms                                                | 74.8 ms: 1.21x slower                                                            |
| xml_etree_generate         | 45.8 ms                                                | 55.7 ms: 1.22x slower                                                            |
| python_startup             | 10.8 ms                                                | 13.1 ms: 1.22x slower                                                            |
| spectral_norm              | 65.7 ms                                                | 80.7 ms: 1.23x slower                                                            |
| fannkuch                   | 240 ms                                                 | 295 ms: 1.23x slower                                                             |
| scimark_fft                | 173 ms                                                 | 215 ms: 1.24x slower                                                             |
| sqlite_synth               | 1.26 us                                                | 1.59 us: 1.27x slower                                                            |
| scimark_sor                | 79.2 ms                                                | 107 ms: 1.35x slower                                                             |
| python_startup_no_site     | 8.57 ms                                                | 11.8 ms: 1.37x slower                                                            |
| mypy2                      | 372 ms                                                 | 529 ms: 1.42x slower                                                             |
| telco                      | 3.17 ms                                                | 4.59 ms: 1.45x slower                                                            |
| async_generators           | 192 ms                                                 | 306 ms: 1.59x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (5): async_tree_memoization, async_tree_io, async_tree_cpu_io_mixed, mako, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.20x