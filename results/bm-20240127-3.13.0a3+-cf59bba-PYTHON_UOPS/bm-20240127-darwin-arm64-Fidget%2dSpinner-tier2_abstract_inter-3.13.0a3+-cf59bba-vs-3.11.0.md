
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 175 ms: 1.13x slower                                                             |
| chameleon      | 4.30 ms                                                | 4.98 ms: 1.16x slower                                                            |
| docutils       | 1.43 sec                                               | 1.51 sec: 1.05x slower                                                           |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 258 ms: 1.09x faster                                                             |
| async_tree_io_tg           | 724 ms                                                 | 677 ms: 1.07x faster                                                             |
| async_tree_memoization_tg  | 352 ms                                                 | 331 ms: 1.07x faster                                                             |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 535 ms: 1.03x faster                                                             |
| async_tree_io              | 697 ms                                                 | 708 ms: 1.02x slower                                                             |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 527 ms: 1.02x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                                     |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 284 ms: 1.01x slower                                                             |
| nbody          | 61.7 ms                                                | 81.7 ms: 1.32x slower                                                            |
| float          | 50.8 ms                                                | 67.3 ms: 1.32x slower                                                            |
| Geometric mean | (ref)                                                  | 1.21x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 157 ms: 1.06x slower                                                             |
| regex_compile  | 72.8 ms                                                | 82.1 ms: 1.13x slower                                                            |
| regex_effbot   | 2.43 ms                                                | 2.78 ms: 1.14x slower                                                            |
| regex_v8       | 15.1 ms                                                | 18.1 ms: 1.20x slower                                                            |
| Geometric mean | (ref)                                                  | 1.13x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.54 ms: 1.15x faster                                                            |
| pickle_pure_python   | 191 us                                                 | 197 us: 1.03x slower                                                             |
| pickle               | 6.98 us                                                | 7.23 us: 1.04x slower                                                            |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                                            |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.06x slower                                                             |
| unpickle_pure_python | 149 us                                                 | 163 us: 1.09x slower                                                             |
| pickle_list          | 2.70 us                                                | 2.98 us: 1.11x slower                                                            |
| unpickle             | 8.29 us                                                | 9.20 us: 1.11x slower                                                            |
| json_loads           | 15.3 us                                                | 17.2 us: 1.12x slower                                                            |
| unpickle_list        | 2.69 us                                                | 3.04 us: 1.13x slower                                                            |
| xml_etree_iterparse  | 68.3 ms                                                | 80.7 ms: 1.18x slower                                                            |
| xml_etree_process    | 33.6 ms                                                | 40.7 ms: 1.21x slower                                                            |
| xml_etree_generate   | 45.8 ms                                                | 58.5 ms: 1.28x slower                                                            |
| tomli_loads          | 1.27 sec                                               | 1.64 sec: 1.29x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.11x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 12.7 ms: 1.18x slower                                                            |
| python_startup_no_site | 8.57 ms                                                | 11.4 ms: 1.33x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 9.64 ms: 1.21x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240127-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 73.6 us: 4.09x faster                                                            |
| asyncio_tcp                | 643 ms                                                 | 409 ms: 1.57x faster                                                             |
| unpack_sequence            | 33.6 ns                                                | 28.1 ns: 1.20x faster                                                            |
| json_dumps                 | 7.53 ms                                                | 6.54 ms: 1.15x faster                                                            |
| raytrace                   | 206 ms                                                 | 184 ms: 1.12x faster                                                             |
| sqlglot_parse              | 890 us                                                 | 812 us: 1.10x faster                                                             |
| async_tree_none            | 282 ms                                                 | 258 ms: 1.09x faster                                                             |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.29 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 724 ms                                                 | 677 ms: 1.07x faster                                                             |
| async_tree_memoization_tg  | 352 ms                                                 | 331 ms: 1.07x faster                                                             |
| sqlglot_transpile          | 1.05 ms                                                | 995 us: 1.06x faster                                                             |
| generators                 | 30.3 ms                                                | 28.7 ms: 1.06x faster                                                            |
| chaos                      | 47.4 ms                                                | 45.3 ms: 1.05x faster                                                            |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 535 ms: 1.03x faster                                                             |
| richards_super             | 37.3 ms                                                | 36.5 ms: 1.02x faster                                                            |
| sympy_sum                  | 80.2 ms                                                | 79.5 ms: 1.01x faster                                                            |
| create_gc_cycles           | 711 us                                                 | 707 us: 1.01x faster                                                             |
| pidigits                   | 280 ms                                                 | 284 ms: 1.01x slower                                                             |
| async_tree_io              | 697 ms                                                 | 708 ms: 1.02x slower                                                             |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 527 ms: 1.02x slower                                                             |
| sympy_integrate            | 11.3 ms                                                | 11.6 ms: 1.03x slower                                                            |
| dask                       | 219 ms                                                 | 226 ms: 1.03x slower                                                             |
| deepcopy_memo              | 25.7 us                                                | 26.5 us: 1.03x slower                                                            |
| pickle_pure_python         | 191 us                                                 | 197 us: 1.03x slower                                                             |
| pickle                     | 6.98 us                                                | 7.23 us: 1.04x slower                                                            |
| sympy_str                  | 144 ms                                                 | 150 ms: 1.04x slower                                                             |
| logging_simple             | 3.41 us                                                | 3.56 us: 1.04x slower                                                            |
| dulwich_log                | 28.6 ms                                                | 30.0 ms: 1.05x slower                                                            |
| richards                   | 31.1 ms                                                | 32.6 ms: 1.05x slower                                                            |
| deepcopy                   | 215 us                                                 | 227 us: 1.05x slower                                                             |
| docutils                   | 1.43 sec                                               | 1.51 sec: 1.05x slower                                                           |
| logging_format             | 3.67 us                                                | 3.87 us: 1.05x slower                                                            |
| comprehensions             | 14.4 us                                                | 15.2 us: 1.05x slower                                                            |
| go                         | 105 ms                                                 | 112 ms: 1.06x slower                                                             |
| pickle_dict                | 17.1 us                                                | 18.1 us: 1.06x slower                                                            |
| regex_dna                  | 148 ms                                                 | 157 ms: 1.06x slower                                                             |
| pathlib                    | 23.2 ms                                                | 24.6 ms: 1.06x slower                                                            |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.06x slower                                                             |
| pycparser                  | 659 ms                                                 | 704 ms: 1.07x slower                                                             |
| gc_traversal               | 2.38 ms                                                | 2.55 ms: 1.07x slower                                                            |
| sympy_expand               | 229 ms                                                 | 246 ms: 1.08x slower                                                             |
| json                       | 2.75 ms                                                | 2.97 ms: 1.08x slower                                                            |
| logging_silent             | 66.5 ns                                                | 71.9 ns: 1.08x slower                                                            |
| meteor_contest             | 71.1 ms                                                | 77.1 ms: 1.08x slower                                                            |
| mdp                        | 1.48 sec                                               | 1.62 sec: 1.09x slower                                                           |
| coverage                   | 43.9 ms                                                | 47.9 ms: 1.09x slower                                                            |
| unpickle_pure_python       | 149 us                                                 | 163 us: 1.09x slower                                                             |
| bench_thread_pool          | 465 us                                                 | 512 us: 1.10x slower                                                             |
| pickle_list                | 2.70 us                                                | 2.98 us: 1.11x slower                                                            |
| unpickle                   | 8.29 us                                                | 9.20 us: 1.11x slower                                                            |
| bench_mp_pool              | 41.0 ms                                                | 45.7 ms: 1.12x slower                                                            |
| deepcopy_reduce            | 1.79 us                                                | 2.01 us: 1.12x slower                                                            |
| json_loads                 | 15.3 us                                                | 17.2 us: 1.12x slower                                                            |
| regex_compile              | 72.8 ms                                                | 82.1 ms: 1.13x slower                                                            |
| coroutines                 | 17.2 ms                                                | 19.4 ms: 1.13x slower                                                            |
| unpickle_list              | 2.69 us                                                | 3.04 us: 1.13x slower                                                            |
| 2to3                       | 154 ms                                                 | 175 ms: 1.13x slower                                                             |
| scimark_lu                 | 67.7 ms                                                | 76.8 ms: 1.13x slower                                                            |
| regex_effbot               | 2.43 ms                                                | 2.78 ms: 1.14x slower                                                            |
| crypto_pyaes               | 47.5 ms                                                | 54.8 ms: 1.15x slower                                                            |
| chameleon                  | 4.30 ms                                                | 4.98 ms: 1.16x slower                                                            |
| sqlglot_normalize          | 162 ms                                                 | 191 ms: 1.18x slower                                                             |
| xml_etree_iterparse        | 68.3 ms                                                | 80.7 ms: 1.18x slower                                                            |
| pprint_safe_repr           | 478 ms                                                 | 566 ms: 1.18x slower                                                             |
| python_startup             | 10.8 ms                                                | 12.7 ms: 1.18x slower                                                            |
| pprint_pformat             | 979 ms                                                 | 1.16 sec: 1.19x slower                                                           |
| regex_v8                   | 15.1 ms                                                | 18.1 ms: 1.20x slower                                                            |
| nqueens                    | 55.9 ms                                                | 67.3 ms: 1.20x slower                                                            |
| sqlglot_optimize           | 29.6 ms                                                | 35.9 ms: 1.21x slower                                                            |
| xml_etree_process          | 33.6 ms                                                | 40.7 ms: 1.21x slower                                                            |
| mako                       | 7.93 ms                                                | 9.64 ms: 1.21x slower                                                            |
| xml_etree_generate         | 45.8 ms                                                | 58.5 ms: 1.28x slower                                                            |
| hexiom                     | 4.58 ms                                                | 5.89 ms: 1.29x slower                                                            |
| deltablue                  | 2.75 ms                                                | 3.54 ms: 1.29x slower                                                            |
| tomli_loads                | 1.27 sec                                               | 1.64 sec: 1.29x slower                                                           |
| pyflate                    | 284 ms                                                 | 367 ms: 1.29x slower                                                             |
| scimark_monte_carlo        | 43.5 ms                                                | 56.3 ms: 1.29x slower                                                            |
| sqlite_synth               | 1.26 us                                                | 1.64 us: 1.31x slower                                                            |
| nbody                      | 61.7 ms                                                | 81.7 ms: 1.32x slower                                                            |
| float                      | 50.8 ms                                                | 67.3 ms: 1.32x slower                                                            |
| python_startup_no_site     | 8.57 ms                                                | 11.4 ms: 1.33x slower                                                            |
| fannkuch                   | 240 ms                                                 | 321 ms: 1.34x slower                                                             |
| scimark_sor                | 79.2 ms                                                | 106 ms: 1.34x slower                                                             |
| scimark_fft                | 173 ms                                                 | 235 ms: 1.36x slower                                                             |
| mypy2                      | 372 ms                                                 | 525 ms: 1.41x slower                                                             |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 4.04 ms: 1.44x slower                                                            |
| telco                      | 3.17 ms                                                | 4.64 ms: 1.47x slower                                                            |
| spectral_norm              | 65.7 ms                                                | 98.2 ms: 1.49x slower                                                            |
| async_generators           | 192 ms                                                 | 299 ms: 1.56x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                                     |

Benchmark hidden because not significant (3): async_tree_memoization, asyncio_websockets, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 1.06x