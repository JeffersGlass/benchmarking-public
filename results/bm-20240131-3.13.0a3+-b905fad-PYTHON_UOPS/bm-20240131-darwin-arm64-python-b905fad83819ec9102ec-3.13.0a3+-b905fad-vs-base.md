# Results vs. base

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 170 ms                                                                                                            | 174 ms: 1.03x slower                                                                                                          |
| chameleon      | 4.89 ms                                                                                                           | 4.95 ms: 1.01x slower                                                                                                         |
| docutils       | 1.45 sec                                                                                                          | 1.50 sec: 1.03x slower                                                                                                        |
| tornado_http   | 67.7 ms                                                                                                           | 69.7 ms: 1.03x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 528 ms                                                                                                            | 535 ms: 1.01x slower                                                                                                          |
| async_tree_cpu_io_mixed    | 517 ms                                                                                                            | 525 ms: 1.02x slower                                                                                                          |
| async_tree_io              | 694 ms                                                                                                            | 706 ms: 1.02x slower                                                                                                          |
| async_tree_io_tg           | 664 ms                                                                                                            | 676 ms: 1.02x slower                                                                                                          |
| async_tree_memoization     | 325 ms                                                                                                            | 333 ms: 1.03x slower                                                                                                          |
| async_tree_memoization_tg  | 321 ms                                                                                                            | 330 ms: 1.03x slower                                                                                                          |
| async_tree_none_tg         | 258 ms                                                                                                            | 266 ms: 1.03x slower                                                                                                          |
| async_tree_none            | 249 ms                                                                                                            | 258 ms: 1.04x slower                                                                                                          |
| Geometric mean             | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 283 ms                                                                                                            | 283 ms: 1.00x slower                                                                                                          |
| nbody          | 75.0 ms                                                                                                           | 85.3 ms: 1.14x slower                                                                                                         |
| float          | 56.4 ms                                                                                                           | 68.3 ms: 1.21x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.11x slower                                                                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| regex_dna      | 151 ms                                                                                                            | 152 ms: 1.00x slower                                                                                                          |
| regex_v8       | 17.1 ms                                                                                                           | 17.1 ms: 1.00x slower                                                                                                         |
| regex_compile  | 73.1 ms                                                                                                           | 81.7 ms: 1.12x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.03x slower                                                                                                                  |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| unpickle             | 9.23 us                                                                                                           | 9.11 us: 1.01x faster                                                                                                         |
| pickle_dict          | 18.1 us                                                                                                           | 18.2 us: 1.01x slower                                                                                                         |
| pickle_list          | 2.97 us                                                                                                           | 2.99 us: 1.01x slower                                                                                                         |
| json_loads           | 16.9 us                                                                                                           | 17.0 us: 1.01x slower                                                                                                         |
| pickle_pure_python   | 196 us                                                                                                            | 198 us: 1.01x slower                                                                                                          |
| json_dumps           | 6.49 ms                                                                                                           | 6.57 ms: 1.01x slower                                                                                                         |
| xml_etree_parse      | 105 ms                                                                                                            | 107 ms: 1.01x slower                                                                                                          |
| xml_etree_process    | 39.6 ms                                                                                                           | 41.0 ms: 1.04x slower                                                                                                         |
| xml_etree_generate   | 56.1 ms                                                                                                           | 58.8 ms: 1.05x slower                                                                                                         |
| tomli_loads          | 1.54 sec                                                                                                          | 1.64 sec: 1.06x slower                                                                                                        |
| unpickle_pure_python | 153 us                                                                                                            | 163 us: 1.06x slower                                                                                                          |
| xml_etree_iterparse  | 75.5 ms                                                                                                           | 80.5 ms: 1.07x slower                                                                                                         |
| Geometric mean       | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmark hidden because not significant (2): unpickle_list, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 13.0 ms                                                                                                           | 13.2 ms: 1.01x slower                                                                                                         |
| python_startup_no_site | 11.6 ms                                                                                                           | 11.8 ms: 1.01x slower                                                                                                         |
| Geometric mean         | (ref)                                                                                                             | 1.01x slower                                                                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|-----------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| mako      | 7.59 ms                                                                                                           | 9.66 ms: 1.27x slower                                                                                                         |

All benchmarks:
===============

| Benchmark                  | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| richards                   | 33.5 ms                                                                                                           | 33.0 ms: 1.02x faster                                                                                                         |
| unpickle                   | 9.23 us                                                                                                           | 9.11 us: 1.01x faster                                                                                                         |
| richards_super             | 37.4 ms                                                                                                           | 37.0 ms: 1.01x faster                                                                                                         |
| coverage                   | 47.6 ms                                                                                                           | 47.1 ms: 1.01x faster                                                                                                         |
| asyncio_websockets         | 409 ms                                                                                                            | 409 ms: 1.00x faster                                                                                                          |
| regex_dna                  | 151 ms                                                                                                            | 152 ms: 1.00x slower                                                                                                          |
| pidigits                   | 283 ms                                                                                                            | 283 ms: 1.00x slower                                                                                                          |
| regex_v8                   | 17.1 ms                                                                                                           | 17.1 ms: 1.00x slower                                                                                                         |
| create_gc_cycles           | 701 us                                                                                                            | 704 us: 1.00x slower                                                                                                          |
| pickle_dict                | 18.1 us                                                                                                           | 18.2 us: 1.01x slower                                                                                                         |
| pickle_list                | 2.97 us                                                                                                           | 2.99 us: 1.01x slower                                                                                                         |
| json_loads                 | 16.9 us                                                                                                           | 17.0 us: 1.01x slower                                                                                                         |
| pickle_pure_python         | 196 us                                                                                                            | 198 us: 1.01x slower                                                                                                          |
| async_generators           | 294 ms                                                                                                            | 297 ms: 1.01x slower                                                                                                          |
| python_startup             | 13.0 ms                                                                                                           | 13.2 ms: 1.01x slower                                                                                                         |
| coroutines                 | 19.5 ms                                                                                                           | 19.7 ms: 1.01x slower                                                                                                         |
| json_dumps                 | 6.49 ms                                                                                                           | 6.57 ms: 1.01x slower                                                                                                         |
| async_tree_cpu_io_mixed_tg | 528 ms                                                                                                            | 535 ms: 1.01x slower                                                                                                          |
| scimark_sor                | 105 ms                                                                                                            | 106 ms: 1.01x slower                                                                                                          |
| chameleon                  | 4.89 ms                                                                                                           | 4.95 ms: 1.01x slower                                                                                                         |
| deepcopy                   | 224 us                                                                                                            | 227 us: 1.01x slower                                                                                                          |
| dask                       | 222 ms                                                                                                            | 224 ms: 1.01x slower                                                                                                          |
| python_startup_no_site     | 11.6 ms                                                                                                           | 11.8 ms: 1.01x slower                                                                                                         |
| xml_etree_parse            | 105 ms                                                                                                            | 107 ms: 1.01x slower                                                                                                          |
| generators                 | 28.3 ms                                                                                                           | 28.7 ms: 1.02x slower                                                                                                         |
| async_tree_cpu_io_mixed    | 517 ms                                                                                                            | 525 ms: 1.02x slower                                                                                                          |
| logging_silent             | 70.1 ns                                                                                                           | 71.3 ns: 1.02x slower                                                                                                         |
| pycparser                  | 691 ms                                                                                                            | 702 ms: 1.02x slower                                                                                                          |
| async_tree_io              | 694 ms                                                                                                            | 706 ms: 1.02x slower                                                                                                          |
| bench_mp_pool              | 44.7 ms                                                                                                           | 45.5 ms: 1.02x slower                                                                                                         |
| async_tree_io_tg           | 664 ms                                                                                                            | 676 ms: 1.02x slower                                                                                                          |
| dulwich_log                | 29.5 ms                                                                                                           | 30.1 ms: 1.02x slower                                                                                                         |
| sqlglot_parse              | 793 us                                                                                                            | 813 us: 1.02x slower                                                                                                          |
| unpack_sequence            | 28.4 ns                                                                                                           | 29.1 ns: 1.02x slower                                                                                                         |
| async_tree_memoization     | 325 ms                                                                                                            | 333 ms: 1.03x slower                                                                                                          |
| 2to3                       | 170 ms                                                                                                            | 174 ms: 1.03x slower                                                                                                          |
| sqlglot_transpile          | 971 us                                                                                                            | 998 us: 1.03x slower                                                                                                          |
| scimark_lu                 | 74.7 ms                                                                                                           | 76.8 ms: 1.03x slower                                                                                                         |
| sympy_expand               | 237 ms                                                                                                            | 244 ms: 1.03x slower                                                                                                          |
| async_tree_memoization_tg  | 321 ms                                                                                                            | 330 ms: 1.03x slower                                                                                                          |
| tornado_http               | 67.7 ms                                                                                                           | 69.7 ms: 1.03x slower                                                                                                         |
| docutils                   | 1.45 sec                                                                                                          | 1.50 sec: 1.03x slower                                                                                                        |
| async_tree_none_tg         | 258 ms                                                                                                            | 266 ms: 1.03x slower                                                                                                          |
| logging_simple             | 3.45 us                                                                                                           | 3.56 us: 1.03x slower                                                                                                         |
| typing_runtime_protocols   | 70.8 us                                                                                                           | 73.2 us: 1.03x slower                                                                                                         |
| logging_format             | 3.75 us                                                                                                           | 3.88 us: 1.03x slower                                                                                                         |
| xml_etree_process          | 39.6 ms                                                                                                           | 41.0 ms: 1.04x slower                                                                                                         |
| async_tree_none            | 249 ms                                                                                                            | 258 ms: 1.04x slower                                                                                                          |
| mdp                        | 1.56 sec                                                                                                          | 1.62 sec: 1.04x slower                                                                                                        |
| sqlite_synth               | 1.58 us                                                                                                           | 1.64 us: 1.04x slower                                                                                                         |
| bench_thread_pool          | 491 us                                                                                                            | 511 us: 1.04x slower                                                                                                          |
| deepcopy_memo              | 25.7 us                                                                                                           | 26.7 us: 1.04x slower                                                                                                         |
| xml_etree_generate         | 56.1 ms                                                                                                           | 58.8 ms: 1.05x slower                                                                                                         |
| sqlglot_normalize          | 182 ms                                                                                                            | 190 ms: 1.05x slower                                                                                                          |
| telco                      | 4.46 ms                                                                                                           | 4.70 ms: 1.05x slower                                                                                                         |
| go                         | 105 ms                                                                                                            | 111 ms: 1.06x slower                                                                                                          |
| sqlglot_optimize           | 33.7 ms                                                                                                           | 35.8 ms: 1.06x slower                                                                                                         |
| tomli_loads                | 1.54 sec                                                                                                          | 1.64 sec: 1.06x slower                                                                                                        |
| sympy_str                  | 139 ms                                                                                                            | 147 ms: 1.06x slower                                                                                                          |
| unpickle_pure_python       | 153 us                                                                                                            | 163 us: 1.06x slower                                                                                                          |
| xml_etree_iterparse        | 75.5 ms                                                                                                           | 80.5 ms: 1.07x slower                                                                                                         |
| meteor_contest             | 72.4 ms                                                                                                           | 77.2 ms: 1.07x slower                                                                                                         |
| sympy_integrate            | 10.7 ms                                                                                                           | 11.5 ms: 1.08x slower                                                                                                         |
| raytrace                   | 170 ms                                                                                                            | 185 ms: 1.09x slower                                                                                                          |
| pyflate                    | 334 ms                                                                                                            | 366 ms: 1.10x slower                                                                                                          |
| sympy_sum                  | 72.1 ms                                                                                                           | 79.1 ms: 1.10x slower                                                                                                         |
| pprint_safe_repr           | 513 ms                                                                                                            | 568 ms: 1.11x slower                                                                                                          |
| pprint_pformat             | 1.04 sec                                                                                                          | 1.16 sec: 1.12x slower                                                                                                        |
| crypto_pyaes               | 48.3 ms                                                                                                           | 54.0 ms: 1.12x slower                                                                                                         |
| regex_compile              | 73.1 ms                                                                                                           | 81.7 ms: 1.12x slower                                                                                                         |
| nqueens                    | 60.1 ms                                                                                                           | 67.9 ms: 1.13x slower                                                                                                         |
| nbody                      | 75.0 ms                                                                                                           | 85.3 ms: 1.14x slower                                                                                                         |
| chaos                      | 39.5 ms                                                                                                           | 45.9 ms: 1.16x slower                                                                                                         |
| fannkuch                   | 271 ms                                                                                                            | 319 ms: 1.18x slower                                                                                                          |
| scimark_monte_carlo        | 47.2 ms                                                                                                           | 56.0 ms: 1.19x slower                                                                                                         |
| scimark_fft                | 203 ms                                                                                                            | 244 ms: 1.20x slower                                                                                                          |
| float                      | 56.4 ms                                                                                                           | 68.3 ms: 1.21x slower                                                                                                         |
| mako                       | 7.59 ms                                                                                                           | 9.66 ms: 1.27x slower                                                                                                         |
| comprehensions             | 11.9 us                                                                                                           | 15.2 us: 1.28x slower                                                                                                         |
| hexiom                     | 4.47 ms                                                                                                           | 5.85 ms: 1.31x slower                                                                                                         |
| scimark_sparse_mat_mult    | 3.11 ms                                                                                                           | 4.09 ms: 1.31x slower                                                                                                         |
| spectral_norm              | 74.7 ms                                                                                                           | 101 ms: 1.35x slower                                                                                                          |
| deltablue                  | 2.43 ms                                                                                                           | 3.53 ms: 1.45x slower                                                                                                         |
| Geometric mean             | (ref)                                                                                                             | 1.06x slower                                                                                                                  |

Benchmark hidden because not significant (10): asyncio_tcp, unpickle_list, json, pathlib, pickle, regex_effbot, gc_traversal, deepcopy_reduce, asyncio_tcp_ssl, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.01x