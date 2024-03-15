
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.09x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 1.31x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 175 ms: 1.14x slower                                                             |
| chameleon      | 4.30 ms                                                | 5.00 ms: 1.16x slower                                                            |
| docutils       | 1.43 sec                                               | 1.50 sec: 1.05x slower                                                           |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 260 ms: 1.08x faster                                                             |
| async_tree_memoization_tg  | 352 ms                                                 | 334 ms: 1.05x faster                                                             |
| async_tree_io_tg           | 724 ms                                                 | 688 ms: 1.05x faster                                                             |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 538 ms: 1.02x faster                                                             |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 529 ms: 1.02x slower                                                             |
| async_tree_io              | 697 ms                                                 | 715 ms: 1.03x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 284 ms: 1.01x slower                                                             |
| float          | 50.8 ms                                                | 68.0 ms: 1.34x slower                                                            |
| nbody          | 61.7 ms                                                | 85.6 ms: 1.39x slower                                                            |
| Geometric mean | (ref)                                                  | 1.23x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 155 ms: 1.05x slower                                                             |
| regex_compile  | 72.8 ms                                                | 81.8 ms: 1.12x slower                                                            |
| regex_effbot   | 2.43 ms                                                | 2.75 ms: 1.13x slower                                                            |
| regex_v8       | 15.1 ms                                                | 17.9 ms: 1.18x slower                                                            |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.57 ms: 1.15x faster                                                            |
| pickle_pure_python   | 191 us                                                 | 197 us: 1.03x slower                                                             |
| pickle_dict          | 17.1 us                                                | 18.2 us: 1.07x slower                                                            |
| pickle               | 6.98 us                                                | 7.45 us: 1.07x slower                                                            |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                                             |
| pickle_list          | 2.70 us                                                | 2.93 us: 1.09x slower                                                            |
| unpickle_pure_python | 149 us                                                 | 164 us: 1.10x slower                                                             |
| unpickle             | 8.29 us                                                | 9.17 us: 1.11x slower                                                            |
| json_loads           | 15.3 us                                                | 17.2 us: 1.12x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.04 us: 1.13x slower                                                            |
| xml_etree_iterparse  | 68.3 ms                                                | 81.1 ms: 1.19x slower                                                            |
| xml_etree_process    | 33.6 ms                                                | 40.7 ms: 1.21x slower                                                            |
| xml_etree_generate   | 45.8 ms                                                | 58.7 ms: 1.28x slower                                                            |
| tomli_loads          | 1.27 sec                                               | 1.66 sec: 1.30x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.11x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.8 ms: 1.10x slower                                                            |
| python_startup_no_site | 8.57 ms                                                | 10.5 ms: 1.23x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 9.56 ms: 1.21x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 74.7 us: 4.03x faster                                                            |
| asyncio_tcp                | 643 ms                                                 | 393 ms: 1.64x faster                                                             |
| unpack_sequence            | 33.6 ns                                                | 28.4 ns: 1.18x faster                                                            |
| json_dumps                 | 7.53 ms                                                | 6.57 ms: 1.15x faster                                                            |
| raytrace                   | 206 ms                                                 | 186 ms: 1.11x faster                                                             |
| sqlglot_parse              | 890 us                                                 | 810 us: 1.10x faster                                                             |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.27 sec: 1.10x faster                                                           |
| async_tree_none            | 282 ms                                                 | 260 ms: 1.08x faster                                                             |
| sqlglot_transpile          | 1.05 ms                                                | 992 us: 1.06x faster                                                             |
| async_tree_memoization_tg  | 352 ms                                                 | 334 ms: 1.05x faster                                                             |
| generators                 | 30.3 ms                                                | 28.7 ms: 1.05x faster                                                            |
| async_tree_io_tg           | 724 ms                                                 | 688 ms: 1.05x faster                                                             |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                             |
| chaos                      | 47.4 ms                                                | 46.1 ms: 1.03x faster                                                            |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 538 ms: 1.02x faster                                                             |
| richards_super             | 37.3 ms                                                | 36.7 ms: 1.02x faster                                                            |
| create_gc_cycles           | 711 us                                                 | 702 us: 1.01x faster                                                             |
| sympy_sum                  | 80.2 ms                                                | 79.5 ms: 1.01x faster                                                            |
| asyncio_websockets         | 408 ms                                                 | 408 ms: 1.00x faster                                                             |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                            |
| pidigits                   | 280 ms                                                 | 284 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 529 ms: 1.02x slower                                                             |
| sympy_integrate            | 11.3 ms                                                | 11.5 ms: 1.02x slower                                                            |
| async_tree_io              | 697 ms                                                 | 715 ms: 1.03x slower                                                             |
| sympy_str                  | 144 ms                                                 | 148 ms: 1.03x slower                                                             |
| pickle_pure_python         | 191 us                                                 | 197 us: 1.03x slower                                                             |
| dask                       | 219 ms                                                 | 227 ms: 1.04x slower                                                             |
| deepcopy_memo              | 25.7 us                                                | 26.8 us: 1.04x slower                                                            |
| logging_simple             | 3.41 us                                                | 3.56 us: 1.04x slower                                                            |
| docutils                   | 1.43 sec                                               | 1.50 sec: 1.05x slower                                                           |
| regex_dna                  | 148 ms                                                 | 155 ms: 1.05x slower                                                             |
| dulwich_log                | 28.6 ms                                                | 30.0 ms: 1.05x slower                                                            |
| logging_format             | 3.67 us                                                | 3.86 us: 1.05x slower                                                            |
| richards                   | 31.1 ms                                                | 32.6 ms: 1.05x slower                                                            |
| go                         | 105 ms                                                 | 111 ms: 1.05x slower                                                             |
| deepcopy                   | 215 us                                                 | 227 us: 1.05x slower                                                             |
| pickle_dict                | 17.1 us                                                | 18.2 us: 1.07x slower                                                            |
| pycparser                  | 659 ms                                                 | 704 ms: 1.07x slower                                                             |
| pickle                     | 6.98 us                                                | 7.45 us: 1.07x slower                                                            |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                                             |
| sympy_expand               | 229 ms                                                 | 245 ms: 1.07x slower                                                             |
| pathlib                    | 23.2 ms                                                | 24.9 ms: 1.07x slower                                                            |
| json                       | 2.75 ms                                                | 2.96 ms: 1.08x slower                                                            |
| comprehensions             | 14.4 us                                                | 15.6 us: 1.08x slower                                                            |
| mdp                        | 1.48 sec                                               | 1.61 sec: 1.08x slower                                                           |
| logging_silent             | 66.5 ns                                                | 72.2 ns: 1.08x slower                                                            |
| pickle_list                | 2.70 us                                                | 2.93 us: 1.09x slower                                                            |
| meteor_contest             | 71.1 ms                                                | 77.4 ms: 1.09x slower                                                            |
| coroutines                 | 17.2 ms                                                | 18.9 ms: 1.10x slower                                                            |
| python_startup             | 10.8 ms                                                | 11.8 ms: 1.10x slower                                                            |
| unpickle_pure_python       | 149 us                                                 | 164 us: 1.10x slower                                                             |
| unpickle                   | 8.29 us                                                | 9.17 us: 1.11x slower                                                            |
| deepcopy_reduce            | 1.79 us                                                | 1.99 us: 1.11x slower                                                            |
| bench_mp_pool              | 41.0 ms                                                | 45.4 ms: 1.11x slower                                                            |
| bench_thread_pool          | 465 us                                                 | 519 us: 1.12x slower                                                             |
| json_loads                 | 15.3 us                                                | 17.2 us: 1.12x slower                                                            |
| regex_compile              | 72.8 ms                                                | 81.8 ms: 1.12x slower                                                            |
| unpickle_list              | 2.69 us                                                | 3.04 us: 1.13x slower                                                            |
| regex_effbot               | 2.43 ms                                                | 2.75 ms: 1.13x slower                                                            |
| scimark_lu                 | 67.7 ms                                                | 76.7 ms: 1.13x slower                                                            |
| 2to3                       | 154 ms                                                 | 175 ms: 1.14x slower                                                             |
| coverage                   | 43.9 ms                                                | 50.0 ms: 1.14x slower                                                            |
| crypto_pyaes               | 47.5 ms                                                | 54.5 ms: 1.15x slower                                                            |
| chameleon                  | 4.30 ms                                                | 5.00 ms: 1.16x slower                                                            |
| sqlglot_normalize          | 162 ms                                                 | 190 ms: 1.18x slower                                                             |
| regex_v8                   | 15.1 ms                                                | 17.9 ms: 1.18x slower                                                            |
| xml_etree_iterparse        | 68.3 ms                                                | 81.1 ms: 1.19x slower                                                            |
| pprint_safe_repr           | 478 ms                                                 | 572 ms: 1.20x slower                                                             |
| pprint_pformat             | 979 ms                                                 | 1.18 sec: 1.20x slower                                                           |
| mako                       | 7.93 ms                                                | 9.56 ms: 1.21x slower                                                            |
| nqueens                    | 55.9 ms                                                | 67.6 ms: 1.21x slower                                                            |
| sqlglot_optimize           | 29.6 ms                                                | 35.9 ms: 1.21x slower                                                            |
| xml_etree_process          | 33.6 ms                                                | 40.7 ms: 1.21x slower                                                            |
| python_startup_no_site     | 8.57 ms                                                | 10.5 ms: 1.23x slower                                                            |
| xml_etree_generate         | 45.8 ms                                                | 58.7 ms: 1.28x slower                                                            |
| hexiom                     | 4.58 ms                                                | 5.95 ms: 1.30x slower                                                            |
| deltablue                  | 2.75 ms                                                | 3.58 ms: 1.30x slower                                                            |
| scimark_monte_carlo        | 43.5 ms                                                | 56.7 ms: 1.30x slower                                                            |
| tomli_loads                | 1.27 sec                                               | 1.66 sec: 1.30x slower                                                           |
| pyflate                    | 284 ms                                                 | 370 ms: 1.30x slower                                                             |
| sqlite_synth               | 1.26 us                                                | 1.65 us: 1.31x slower                                                            |
| fannkuch                   | 240 ms                                                 | 317 ms: 1.32x slower                                                             |
| float                      | 50.8 ms                                                | 68.0 ms: 1.34x slower                                                            |
| scimark_sor                | 79.2 ms                                                | 106 ms: 1.34x slower                                                             |
| scimark_fft                | 173 ms                                                 | 237 ms: 1.37x slower                                                             |
| nbody                      | 61.7 ms                                                | 85.6 ms: 1.39x slower                                                            |
| mypy2                      | 372 ms                                                 | 529 ms: 1.42x slower                                                             |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 4.11 ms: 1.46x slower                                                            |
| telco                      | 3.17 ms                                                | 4.64 ms: 1.47x slower                                                            |
| spectral_norm              | 65.7 ms                                                | 100 ms: 1.53x slower                                                             |
| async_generators           | 192 ms                                                 | 300 ms: 1.56x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.09x slower                                                                     |

Benchmark hidden because not significant (2): async_tree_memoization, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 1.31x