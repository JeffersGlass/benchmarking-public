# Results vs. base

- fork: python
- ref: 52eade22237eef1f3843
- machine: darwin-arm64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 169 ms                                                                                                            | 173 ms: 1.02x slower                                                                                                          |
| chameleon      | 4.89 ms                                                                                                           | 5.02 ms: 1.03x slower                                                                                                         |
| docutils       | 1.46 sec                                                                                                          | 1.51 sec: 1.03x slower                                                                                                        |
| Geometric mean | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| async_tree_io_tg           | 679 ms                                                                                                            | 682 ms: 1.00x slower                                                                                                          |
| async_tree_cpu_io_mixed_tg | 532 ms                                                                                                            | 538 ms: 1.01x slower                                                                                                          |
| async_tree_io              | 704 ms                                                                                                            | 717 ms: 1.02x slower                                                                                                          |
| async_tree_cpu_io_mixed    | 520 ms                                                                                                            | 531 ms: 1.02x slower                                                                                                          |
| async_tree_memoization     | 331 ms                                                                                                            | 338 ms: 1.02x slower                                                                                                          |
| async_tree_none_tg         | 261 ms                                                                                                            | 268 ms: 1.03x slower                                                                                                          |
| async_tree_memoization_tg  | 325 ms                                                                                                            | 333 ms: 1.03x slower                                                                                                          |
| async_tree_none            | 252 ms                                                                                                            | 261 ms: 1.04x slower                                                                                                          |
| Geometric mean             | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 283 ms                                                                                                            | 284 ms: 1.00x slower                                                                                                          |
| nbody          | 75.5 ms                                                                                                           | 85.7 ms: 1.13x slower                                                                                                         |
| float          | 56.9 ms                                                                                                           | 68.6 ms: 1.21x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.11x slower                                                                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| regex_dna      | 155 ms                                                                                                            | 157 ms: 1.01x slower                                                                                                          |
| regex_v8       | 17.8 ms                                                                                                           | 18.1 ms: 1.02x slower                                                                                                         |
| regex_effbot   | 2.74 ms                                                                                                           | 2.85 ms: 1.04x slower                                                                                                         |
| regex_compile  | 73.9 ms                                                                                                           | 82.6 ms: 1.12x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.05x slower                                                                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| unpickle             | 9.17 us                                                                                                           | 9.11 us: 1.01x faster                                                                                                         |
| pickle_pure_python   | 197 us                                                                                                            | 196 us: 1.00x faster                                                                                                          |
| json_dumps           | 6.59 ms                                                                                                           | 6.61 ms: 1.00x slower                                                                                                         |
| pickle               | 7.40 us                                                                                                           | 7.45 us: 1.01x slower                                                                                                         |
| pickle_list          | 2.94 us                                                                                                           | 2.96 us: 1.01x slower                                                                                                         |
| xml_etree_process    | 39.4 ms                                                                                                           | 41.0 ms: 1.04x slower                                                                                                         |
| xml_etree_generate   | 56.2 ms                                                                                                           | 59.5 ms: 1.06x slower                                                                                                         |
| xml_etree_iterparse  | 75.8 ms                                                                                                           | 80.5 ms: 1.06x slower                                                                                                         |
| unpickle_pure_python | 154 us                                                                                                            | 164 us: 1.06x slower                                                                                                          |
| tomli_loads          | 1.55 sec                                                                                                          | 1.67 sec: 1.08x slower                                                                                                        |
| Geometric mean       | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmark hidden because not significant (4): json_loads, unpickle_list, pickle_dict, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 12.5 ms                                                                                                           | 12.6 ms: 1.01x slower                                                                                                         |
| python_startup_no_site | 11.1 ms                                                                                                           | 11.2 ms: 1.01x slower                                                                                                         |
| Geometric mean         | (ref)                                                                                                             | 1.01x slower                                                                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|-----------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| mako      | 7.62 ms                                                                                                           | 9.74 ms: 1.28x slower                                                                                                         |

All benchmarks:
===============

| Benchmark                  | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| richards                   | 33.2 ms                                                                                                           | 32.6 ms: 1.02x faster                                                                                                         |
| richards_super             | 37.0 ms                                                                                                           | 36.5 ms: 1.02x faster                                                                                                         |
| unpickle                   | 9.17 us                                                                                                           | 9.11 us: 1.01x faster                                                                                                         |
| pickle_pure_python         | 197 us                                                                                                            | 196 us: 1.00x faster                                                                                                          |
| gc_traversal               | 2.40 ms                                                                                                           | 2.40 ms: 1.00x slower                                                                                                         |
| asyncio_websockets         | 409 ms                                                                                                            | 410 ms: 1.00x slower                                                                                                          |
| create_gc_cycles           | 706 us                                                                                                            | 708 us: 1.00x slower                                                                                                          |
| json_dumps                 | 6.59 ms                                                                                                           | 6.61 ms: 1.00x slower                                                                                                         |
| pidigits                   | 283 ms                                                                                                            | 284 ms: 1.00x slower                                                                                                          |
| async_tree_io_tg           | 679 ms                                                                                                            | 682 ms: 1.00x slower                                                                                                          |
| python_startup             | 12.5 ms                                                                                                           | 12.6 ms: 1.01x slower                                                                                                         |
| pickle                     | 7.40 us                                                                                                           | 7.45 us: 1.01x slower                                                                                                         |
| pycparser                  | 697 ms                                                                                                            | 702 ms: 1.01x slower                                                                                                          |
| generators                 | 28.5 ms                                                                                                           | 28.7 ms: 1.01x slower                                                                                                         |
| pickle_list                | 2.94 us                                                                                                           | 2.96 us: 1.01x slower                                                                                                         |
| coroutines                 | 18.7 ms                                                                                                           | 18.8 ms: 1.01x slower                                                                                                         |
| python_startup_no_site     | 11.1 ms                                                                                                           | 11.2 ms: 1.01x slower                                                                                                         |
| logging_silent             | 70.5 ns                                                                                                           | 71.1 ns: 1.01x slower                                                                                                         |
| deepcopy                   | 225 us                                                                                                            | 227 us: 1.01x slower                                                                                                          |
| json                       | 2.96 ms                                                                                                           | 2.99 ms: 1.01x slower                                                                                                         |
| deepcopy_reduce            | 1.98 us                                                                                                           | 2.00 us: 1.01x slower                                                                                                         |
| async_tree_cpu_io_mixed_tg | 532 ms                                                                                                            | 538 ms: 1.01x slower                                                                                                          |
| async_generators           | 296 ms                                                                                                            | 300 ms: 1.01x slower                                                                                                          |
| regex_dna                  | 155 ms                                                                                                            | 157 ms: 1.01x slower                                                                                                          |
| scimark_sor                | 105 ms                                                                                                            | 107 ms: 1.01x slower                                                                                                          |
| coverage                   | 47.5 ms                                                                                                           | 48.2 ms: 1.01x slower                                                                                                         |
| async_tree_io              | 704 ms                                                                                                            | 717 ms: 1.02x slower                                                                                                          |
| regex_v8                   | 17.8 ms                                                                                                           | 18.1 ms: 1.02x slower                                                                                                         |
| async_tree_cpu_io_mixed    | 520 ms                                                                                                            | 531 ms: 1.02x slower                                                                                                          |
| dulwich_log                | 29.6 ms                                                                                                           | 30.1 ms: 1.02x slower                                                                                                         |
| async_tree_memoization     | 331 ms                                                                                                            | 338 ms: 1.02x slower                                                                                                          |
| sympy_expand               | 240 ms                                                                                                            | 245 ms: 1.02x slower                                                                                                          |
| 2to3                       | 169 ms                                                                                                            | 173 ms: 1.02x slower                                                                                                          |
| dask                       | 224 ms                                                                                                            | 229 ms: 1.03x slower                                                                                                          |
| chameleon                  | 4.89 ms                                                                                                           | 5.02 ms: 1.03x slower                                                                                                         |
| async_tree_none_tg         | 261 ms                                                                                                            | 268 ms: 1.03x slower                                                                                                          |
| sqlglot_parse              | 790 us                                                                                                            | 811 us: 1.03x slower                                                                                                          |
| async_tree_memoization_tg  | 325 ms                                                                                                            | 333 ms: 1.03x slower                                                                                                          |
| logging_simple             | 3.47 us                                                                                                           | 3.56 us: 1.03x slower                                                                                                         |
| logging_format             | 3.74 us                                                                                                           | 3.85 us: 1.03x slower                                                                                                         |
| sqlglot_transpile          | 967 us                                                                                                            | 995 us: 1.03x slower                                                                                                          |
| telco                      | 4.55 ms                                                                                                           | 4.69 ms: 1.03x slower                                                                                                         |
| bench_thread_pool          | 502 us                                                                                                            | 518 us: 1.03x slower                                                                                                          |
| typing_runtime_protocols   | 71.3 us                                                                                                           | 73.6 us: 1.03x slower                                                                                                         |
| docutils                   | 1.46 sec                                                                                                          | 1.51 sec: 1.03x slower                                                                                                        |
| scimark_lu                 | 74.2 ms                                                                                                           | 76.7 ms: 1.03x slower                                                                                                         |
| sqlite_synth               | 1.59 us                                                                                                           | 1.65 us: 1.04x slower                                                                                                         |
| async_tree_none            | 252 ms                                                                                                            | 261 ms: 1.04x slower                                                                                                          |
| mdp                        | 1.56 sec                                                                                                          | 1.62 sec: 1.04x slower                                                                                                        |
| xml_etree_process          | 39.4 ms                                                                                                           | 41.0 ms: 1.04x slower                                                                                                         |
| regex_effbot               | 2.74 ms                                                                                                           | 2.85 ms: 1.04x slower                                                                                                         |
| deepcopy_memo              | 25.7 us                                                                                                           | 26.7 us: 1.04x slower                                                                                                         |
| sqlglot_normalize          | 182 ms                                                                                                            | 190 ms: 1.05x slower                                                                                                          |
| go                         | 106 ms                                                                                                            | 111 ms: 1.05x slower                                                                                                          |
| xml_etree_generate         | 56.2 ms                                                                                                           | 59.5 ms: 1.06x slower                                                                                                         |
| meteor_contest             | 72.3 ms                                                                                                           | 76.8 ms: 1.06x slower                                                                                                         |
| sqlglot_optimize           | 33.8 ms                                                                                                           | 35.9 ms: 1.06x slower                                                                                                         |
| xml_etree_iterparse        | 75.8 ms                                                                                                           | 80.5 ms: 1.06x slower                                                                                                         |
| unpickle_pure_python       | 154 us                                                                                                            | 164 us: 1.06x slower                                                                                                          |
| sympy_str                  | 139 ms                                                                                                            | 149 ms: 1.07x slower                                                                                                          |
| tomli_loads                | 1.55 sec                                                                                                          | 1.67 sec: 1.08x slower                                                                                                        |
| sympy_integrate            | 10.7 ms                                                                                                           | 11.6 ms: 1.08x slower                                                                                                         |
| raytrace                   | 171 ms                                                                                                            | 186 ms: 1.09x slower                                                                                                          |
| pyflate                    | 342 ms                                                                                                            | 371 ms: 1.09x slower                                                                                                          |
| sympy_sum                  | 72.6 ms                                                                                                           | 79.6 ms: 1.10x slower                                                                                                         |
| pprint_safe_repr           | 517 ms                                                                                                            | 572 ms: 1.11x slower                                                                                                          |
| pprint_pformat             | 1.05 sec                                                                                                          | 1.17 sec: 1.12x slower                                                                                                        |
| regex_compile              | 73.9 ms                                                                                                           | 82.6 ms: 1.12x slower                                                                                                         |
| nqueens                    | 60.3 ms                                                                                                           | 68.1 ms: 1.13x slower                                                                                                         |
| crypto_pyaes               | 48.6 ms                                                                                                           | 54.9 ms: 1.13x slower                                                                                                         |
| nbody                      | 75.5 ms                                                                                                           | 85.7 ms: 1.13x slower                                                                                                         |
| chaos                      | 39.9 ms                                                                                                           | 46.5 ms: 1.16x slower                                                                                                         |
| fannkuch                   | 273 ms                                                                                                            | 326 ms: 1.19x slower                                                                                                          |
| scimark_monte_carlo        | 47.2 ms                                                                                                           | 56.5 ms: 1.20x slower                                                                                                         |
| scimark_fft                | 205 ms                                                                                                            | 247 ms: 1.21x slower                                                                                                          |
| float                      | 56.9 ms                                                                                                           | 68.6 ms: 1.21x slower                                                                                                         |
| mako                       | 7.62 ms                                                                                                           | 9.74 ms: 1.28x slower                                                                                                         |
| comprehensions             | 12.1 us                                                                                                           | 15.5 us: 1.28x slower                                                                                                         |
| hexiom                     | 4.53 ms                                                                                                           | 5.95 ms: 1.31x slower                                                                                                         |
| scimark_sparse_mat_mult    | 3.12 ms                                                                                                           | 4.12 ms: 1.32x slower                                                                                                         |
| spectral_norm              | 75.9 ms                                                                                                           | 105 ms: 1.39x slower                                                                                                          |
| deltablue                  | 2.45 ms                                                                                                           | 3.59 ms: 1.47x slower                                                                                                         |
| Geometric mean             | (ref)                                                                                                             | 1.06x slower                                                                                                                  |

Benchmark hidden because not significant (11): json_loads, unpickle_list, pickle_dict, xml_etree_parse, unpack_sequence, pathlib, asyncio_tcp_ssl, bench_mp_pool, tornado_http, asyncio_tcp, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.00x