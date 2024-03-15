# Results vs. base

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: darwin-arm64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 173 ms                                                                                                            | 178 ms: 1.03x slower                                                                                                          |
| chameleon      | 4.81 ms                                                                                                           | 4.93 ms: 1.02x slower                                                                                                         |
| docutils       | 1.49 sec                                                                                                          | 1.53 sec: 1.03x slower                                                                                                        |
| tornado_http   | 69.4 ms                                                                                                           | 71.7 ms: 1.03x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.03x slower                                                                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| async_tree_io              | 709 ms                                                                                                            | 715 ms: 1.01x slower                                                                                                          |
| async_tree_cpu_io_mixed_tg | 533 ms                                                                                                            | 541 ms: 1.02x slower                                                                                                          |
| async_tree_cpu_io_mixed    | 522 ms                                                                                                            | 531 ms: 1.02x slower                                                                                                          |
| async_tree_io_tg           | 672 ms                                                                                                            | 684 ms: 1.02x slower                                                                                                          |
| async_tree_memoization     | 328 ms                                                                                                            | 337 ms: 1.03x slower                                                                                                          |
| async_tree_none_tg         | 259 ms                                                                                                            | 266 ms: 1.03x slower                                                                                                          |
| async_tree_memoization_tg  | 322 ms                                                                                                            | 333 ms: 1.04x slower                                                                                                          |
| async_tree_none            | 250 ms                                                                                                            | 259 ms: 1.04x slower                                                                                                          |
| Geometric mean             | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 283 ms                                                                                                            | 284 ms: 1.00x slower                                                                                                          |
| nbody          | 79.0 ms                                                                                                           | 89.3 ms: 1.13x slower                                                                                                         |
| float          | 57.9 ms                                                                                                           | 70.1 ms: 1.21x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.11x slower                                                                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 2.49 ms                                                                                                           | 2.49 ms: 1.00x slower                                                                                                         |
| regex_v8       | 16.9 ms                                                                                                           | 17.0 ms: 1.00x slower                                                                                                         |
| regex_compile  | 73.9 ms                                                                                                           | 84.4 ms: 1.14x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.03x slower                                                                                                                  |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| unpickle             | 9.33 us                                                                                                           | 9.20 us: 1.01x faster                                                                                                         |
| pickle               | 7.49 us                                                                                                           | 7.42 us: 1.01x faster                                                                                                         |
| unpickle_list        | 3.15 us                                                                                                           | 3.18 us: 1.01x slower                                                                                                         |
| pickle_pure_python   | 198 us                                                                                                            | 200 us: 1.01x slower                                                                                                          |
| json_dumps           | 6.60 ms                                                                                                           | 6.68 ms: 1.01x slower                                                                                                         |
| pickle_dict          | 17.9 us                                                                                                           | 18.5 us: 1.03x slower                                                                                                         |
| xml_etree_process    | 40.0 ms                                                                                                           | 41.8 ms: 1.04x slower                                                                                                         |
| xml_etree_generate   | 56.7 ms                                                                                                           | 60.1 ms: 1.06x slower                                                                                                         |
| unpickle_pure_python | 157 us                                                                                                            | 167 us: 1.06x slower                                                                                                          |
| xml_etree_iterparse  | 76.1 ms                                                                                                           | 81.2 ms: 1.07x slower                                                                                                         |
| tomli_loads          | 1.58 sec                                                                                                          | 1.69 sec: 1.07x slower                                                                                                        |
| Geometric mean       | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmark hidden because not significant (3): pickle_list, json_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| python_startup_no_site | 12.0 ms                                                                                                           | 11.8 ms: 1.01x faster                                                                                                         |
| python_startup         | 13.4 ms                                                                                                           | 13.2 ms: 1.01x faster                                                                                                         |
| Geometric mean         | (ref)                                                                                                             | 1.01x faster                                                                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|-----------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| mako      | 7.61 ms                                                                                                           | 9.90 ms: 1.30x slower                                                                                                         |

All benchmarks:
===============

| Benchmark                  | results/bm-20240104-3.13.0a2+-1ae7ceb/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json | results/bm-20240104-3.13.0a2+-1ae7ceb-PYTHON_UOPS/bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| richards                   | 34.0 ms                                                                                                           | 32.7 ms: 1.04x faster                                                                                                         |
| coverage                   | 49.3 ms                                                                                                           | 48.2 ms: 1.02x faster                                                                                                         |
| richards_super             | 37.5 ms                                                                                                           | 36.7 ms: 1.02x faster                                                                                                         |
| python_startup_no_site     | 12.0 ms                                                                                                           | 11.8 ms: 1.01x faster                                                                                                         |
| unpickle                   | 9.33 us                                                                                                           | 9.20 us: 1.01x faster                                                                                                         |
| json                       | 3.03 ms                                                                                                           | 3.00 ms: 1.01x faster                                                                                                         |
| unpack_sequence            | 26.6 ns                                                                                                           | 26.4 ns: 1.01x faster                                                                                                         |
| pickle                     | 7.49 us                                                                                                           | 7.42 us: 1.01x faster                                                                                                         |
| python_startup             | 13.4 ms                                                                                                           | 13.2 ms: 1.01x faster                                                                                                         |
| regex_effbot               | 2.49 ms                                                                                                           | 2.49 ms: 1.00x slower                                                                                                         |
| gc_traversal               | 2.40 ms                                                                                                           | 2.41 ms: 1.00x slower                                                                                                         |
| pidigits                   | 283 ms                                                                                                            | 284 ms: 1.00x slower                                                                                                          |
| regex_v8                   | 16.9 ms                                                                                                           | 17.0 ms: 1.00x slower                                                                                                         |
| coroutines                 | 17.8 ms                                                                                                           | 17.9 ms: 1.01x slower                                                                                                         |
| create_gc_cycles           | 702 us                                                                                                            | 707 us: 1.01x slower                                                                                                          |
| unpickle_list              | 3.15 us                                                                                                           | 3.18 us: 1.01x slower                                                                                                         |
| async_tree_io              | 709 ms                                                                                                            | 715 ms: 1.01x slower                                                                                                          |
| async_generators           | 302 ms                                                                                                            | 305 ms: 1.01x slower                                                                                                          |
| deepcopy_reduce            | 2.06 us                                                                                                           | 2.08 us: 1.01x slower                                                                                                         |
| pycparser                  | 702 ms                                                                                                            | 708 ms: 1.01x slower                                                                                                          |
| pickle_pure_python         | 198 us                                                                                                            | 200 us: 1.01x slower                                                                                                          |
| json_dumps                 | 6.60 ms                                                                                                           | 6.68 ms: 1.01x slower                                                                                                         |
| bench_mp_pool              | 45.6 ms                                                                                                           | 46.2 ms: 1.01x slower                                                                                                         |
| bench_thread_pool          | 514 us                                                                                                            | 521 us: 1.01x slower                                                                                                          |
| async_tree_cpu_io_mixed_tg | 533 ms                                                                                                            | 541 ms: 1.02x slower                                                                                                          |
| dask                       | 227 ms                                                                                                            | 230 ms: 1.02x slower                                                                                                          |
| logging_silent             | 71.1 ns                                                                                                           | 72.4 ns: 1.02x slower                                                                                                         |
| async_tree_cpu_io_mixed    | 522 ms                                                                                                            | 531 ms: 1.02x slower                                                                                                          |
| async_tree_io_tg           | 672 ms                                                                                                            | 684 ms: 1.02x slower                                                                                                          |
| deepcopy                   | 229 us                                                                                                            | 233 us: 1.02x slower                                                                                                          |
| scimark_sor                | 107 ms                                                                                                            | 109 ms: 1.02x slower                                                                                                          |
| chameleon                  | 4.81 ms                                                                                                           | 4.93 ms: 1.02x slower                                                                                                         |
| dulwich_log                | 29.6 ms                                                                                                           | 30.3 ms: 1.02x slower                                                                                                         |
| docutils                   | 1.49 sec                                                                                                          | 1.53 sec: 1.03x slower                                                                                                        |
| sqlglot_parse              | 818 us                                                                                                            | 839 us: 1.03x slower                                                                                                          |
| sqlglot_transpile          | 1000 us                                                                                                           | 1.03 ms: 1.03x slower                                                                                                         |
| 2to3                       | 173 ms                                                                                                            | 178 ms: 1.03x slower                                                                                                          |
| sqlite_synth               | 1.66 us                                                                                                           | 1.71 us: 1.03x slower                                                                                                         |
| async_tree_memoization     | 328 ms                                                                                                            | 337 ms: 1.03x slower                                                                                                          |
| async_tree_none_tg         | 259 ms                                                                                                            | 266 ms: 1.03x slower                                                                                                          |
| logging_format             | 3.84 us                                                                                                           | 3.96 us: 1.03x slower                                                                                                         |
| logging_simple             | 3.53 us                                                                                                           | 3.65 us: 1.03x slower                                                                                                         |
| sympy_expand               | 251 ms                                                                                                            | 259 ms: 1.03x slower                                                                                                          |
| tornado_http               | 69.4 ms                                                                                                           | 71.7 ms: 1.03x slower                                                                                                         |
| pickle_dict                | 17.9 us                                                                                                           | 18.5 us: 1.03x slower                                                                                                         |
| async_tree_memoization_tg  | 322 ms                                                                                                            | 333 ms: 1.04x slower                                                                                                          |
| scimark_lu                 | 75.9 ms                                                                                                           | 78.6 ms: 1.04x slower                                                                                                         |
| async_tree_none            | 250 ms                                                                                                            | 259 ms: 1.04x slower                                                                                                          |
| typing_runtime_protocols   | 73.6 us                                                                                                           | 76.3 us: 1.04x slower                                                                                                         |
| xml_etree_process          | 40.0 ms                                                                                                           | 41.8 ms: 1.04x slower                                                                                                         |
| telco                      | 4.74 ms                                                                                                           | 4.96 ms: 1.05x slower                                                                                                         |
| deepcopy_memo              | 24.9 us                                                                                                           | 26.2 us: 1.05x slower                                                                                                         |
| sqlglot_normalize          | 187 ms                                                                                                            | 196 ms: 1.05x slower                                                                                                          |
| xml_etree_generate         | 56.7 ms                                                                                                           | 60.1 ms: 1.06x slower                                                                                                         |
| go                         | 104 ms                                                                                                            | 111 ms: 1.06x slower                                                                                                          |
| unpickle_pure_python       | 157 us                                                                                                            | 167 us: 1.06x slower                                                                                                          |
| sqlglot_optimize           | 34.9 ms                                                                                                           | 37.2 ms: 1.06x slower                                                                                                         |
| mdp                        | 1.63 sec                                                                                                          | 1.74 sec: 1.07x slower                                                                                                        |
| xml_etree_iterparse        | 76.1 ms                                                                                                           | 81.2 ms: 1.07x slower                                                                                                         |
| tomli_loads                | 1.58 sec                                                                                                          | 1.69 sec: 1.07x slower                                                                                                        |
| meteor_contest             | 74.0 ms                                                                                                           | 79.2 ms: 1.07x slower                                                                                                         |
| sympy_str                  | 145 ms                                                                                                            | 156 ms: 1.08x slower                                                                                                          |
| sympy_integrate            | 11.0 ms                                                                                                           | 11.9 ms: 1.08x slower                                                                                                         |
| raytrace                   | 174 ms                                                                                                            | 188 ms: 1.08x slower                                                                                                          |
| pyflate                    | 343 ms                                                                                                            | 374 ms: 1.09x slower                                                                                                          |
| sympy_sum                  | 75.1 ms                                                                                                           | 82.5 ms: 1.10x slower                                                                                                         |
| pprint_safe_repr           | 529 ms                                                                                                            | 583 ms: 1.10x slower                                                                                                          |
| pprint_pformat             | 1.07 sec                                                                                                          | 1.20 sec: 1.12x slower                                                                                                        |
| nqueens                    | 61.0 ms                                                                                                           | 68.8 ms: 1.13x slower                                                                                                         |
| nbody                      | 79.0 ms                                                                                                           | 89.3 ms: 1.13x slower                                                                                                         |
| regex_compile              | 73.9 ms                                                                                                           | 84.4 ms: 1.14x slower                                                                                                         |
| crypto_pyaes               | 48.2 ms                                                                                                           | 55.7 ms: 1.16x slower                                                                                                         |
| fannkuch                   | 295 ms                                                                                                            | 341 ms: 1.16x slower                                                                                                          |
| chaos                      | 40.0 ms                                                                                                           | 47.1 ms: 1.18x slower                                                                                                         |
| float                      | 57.9 ms                                                                                                           | 70.1 ms: 1.21x slower                                                                                                         |
| scimark_monte_carlo        | 47.7 ms                                                                                                           | 58.0 ms: 1.21x slower                                                                                                         |
| scimark_fft                | 205 ms                                                                                                            | 257 ms: 1.25x slower                                                                                                          |
| mako                       | 7.61 ms                                                                                                           | 9.90 ms: 1.30x slower                                                                                                         |
| comprehensions             | 12.2 us                                                                                                           | 16.1 us: 1.32x slower                                                                                                         |
| hexiom                     | 4.49 ms                                                                                                           | 5.96 ms: 1.33x slower                                                                                                         |
| scimark_sparse_mat_mult    | 3.14 ms                                                                                                           | 4.30 ms: 1.37x slower                                                                                                         |
| deltablue                  | 2.47 ms                                                                                                           | 3.64 ms: 1.47x slower                                                                                                         |
| spectral_norm              | 74.0 ms                                                                                                           | 110 ms: 1.49x slower                                                                                                          |
| Geometric mean             | (ref)                                                                                                             | 1.06x slower                                                                                                                  |

Benchmark hidden because not significant (10): regex_dna, generators, asyncio_tcp_ssl, asyncio_websockets, pickle_list, json_loads, xml_etree_parse, asyncio_tcp, pathlib, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.01x