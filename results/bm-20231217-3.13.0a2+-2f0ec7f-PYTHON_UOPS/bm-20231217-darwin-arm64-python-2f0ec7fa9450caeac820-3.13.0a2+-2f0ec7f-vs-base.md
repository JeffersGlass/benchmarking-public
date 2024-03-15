# Results vs. base

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: darwin-arm64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 177 ms                                                                                                            | 181 ms: 1.02x slower                                                                                                          |
| chameleon      | 5.20 ms                                                                                                           | 5.34 ms: 1.03x slower                                                                                                         |
| docutils       | 1.51 sec                                                                                                          | 1.56 sec: 1.03x slower                                                                                                        |
| tornado_http   | 71.6 ms                                                                                                           | 74.9 ms: 1.05x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.03x slower                                                                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 527 ms                                                                                                            | 536 ms: 1.02x slower                                                                                                          |
| async_tree_cpu_io_mixed_tg | 536 ms                                                                                                            | 546 ms: 1.02x slower                                                                                                          |
| async_tree_io              | 709 ms                                                                                                            | 722 ms: 1.02x slower                                                                                                          |
| async_tree_io_tg           | 678 ms                                                                                                            | 691 ms: 1.02x slower                                                                                                          |
| async_tree_none_tg         | 265 ms                                                                                                            | 271 ms: 1.02x slower                                                                                                          |
| async_tree_memoization_tg  | 329 ms                                                                                                            | 338 ms: 1.03x slower                                                                                                          |
| async_tree_memoization     | 332 ms                                                                                                            | 341 ms: 1.03x slower                                                                                                          |
| async_tree_none            | 257 ms                                                                                                            | 264 ms: 1.03x slower                                                                                                          |
| Geometric mean             | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 282 ms                                                                                                            | 283 ms: 1.00x slower                                                                                                          |
| nbody          | 82.5 ms                                                                                                           | 90.1 ms: 1.09x slower                                                                                                         |
| float          | 61.0 ms                                                                                                           | 70.9 ms: 1.16x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.08x slower                                                                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 2.71 ms                                                                                                           | 2.72 ms: 1.00x slower                                                                                                         |
| regex_v8       | 17.7 ms                                                                                                           | 17.8 ms: 1.00x slower                                                                                                         |
| regex_dna      | 152 ms                                                                                                            | 153 ms: 1.01x slower                                                                                                          |
| regex_compile  | 77.4 ms                                                                                                           | 87.5 ms: 1.13x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.03x slower                                                                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| unpickle             | 9.34 us                                                                                                           | 9.16 us: 1.02x faster                                                                                                         |
| unpickle_list        | 3.18 us                                                                                                           | 3.15 us: 1.01x faster                                                                                                         |
| pickle_pure_python   | 207 us                                                                                                            | 206 us: 1.01x faster                                                                                                          |
| json_loads           | 17.3 us                                                                                                           | 17.3 us: 1.01x faster                                                                                                         |
| pickle_list          | 2.90 us                                                                                                           | 2.94 us: 1.01x slower                                                                                                         |
| xml_etree_process    | 41.4 ms                                                                                                           | 42.7 ms: 1.03x slower                                                                                                         |
| unpickle_pure_python | 166 us                                                                                                            | 174 us: 1.05x slower                                                                                                          |
| tomli_loads          | 1.60 sec                                                                                                          | 1.70 sec: 1.06x slower                                                                                                        |
| xml_etree_iterparse  | 76.5 ms                                                                                                           | 81.1 ms: 1.06x slower                                                                                                         |
| xml_etree_generate   | 58.1 ms                                                                                                           | 62.3 ms: 1.07x slower                                                                                                         |
| Geometric mean       | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmark hidden because not significant (4): xml_etree_parse, json_dumps, pickle_dict, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| python_startup_no_site | 11.7 ms                                                                                                           | 11.7 ms: 1.00x slower                                                                                                         |
| Geometric mean         | (ref)                                                                                                             | 1.00x faster                                                                                                                  |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|-----------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| mako      | 8.04 ms                                                                                                           | 9.93 ms: 1.24x slower                                                                                                         |

All benchmarks:
===============

| Benchmark                  | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| unpack_sequence            | 30.3 ns                                                                                                           | 28.9 ns: 1.05x faster                                                                                                         |
| richards                   | 35.7 ms                                                                                                           | 34.6 ms: 1.03x faster                                                                                                         |
| richards_super             | 39.7 ms                                                                                                           | 38.5 ms: 1.03x faster                                                                                                         |
| generators                 | 26.1 ms                                                                                                           | 25.6 ms: 1.02x faster                                                                                                         |
| unpickle                   | 9.34 us                                                                                                           | 9.16 us: 1.02x faster                                                                                                         |
| coroutines                 | 19.2 ms                                                                                                           | 18.8 ms: 1.02x faster                                                                                                         |
| unpickle_list              | 3.18 us                                                                                                           | 3.15 us: 1.01x faster                                                                                                         |
| pickle_pure_python         | 207 us                                                                                                            | 206 us: 1.01x faster                                                                                                          |
| json                       | 3.03 ms                                                                                                           | 3.01 ms: 1.01x faster                                                                                                         |
| create_gc_cycles           | 708 us                                                                                                            | 704 us: 1.01x faster                                                                                                          |
| json_loads                 | 17.3 us                                                                                                           | 17.3 us: 1.01x faster                                                                                                         |
| gc_traversal               | 2.40 ms                                                                                                           | 2.40 ms: 1.00x faster                                                                                                         |
| regex_effbot               | 2.71 ms                                                                                                           | 2.72 ms: 1.00x slower                                                                                                         |
| python_startup_no_site     | 11.7 ms                                                                                                           | 11.7 ms: 1.00x slower                                                                                                         |
| coverage                   | 48.3 ms                                                                                                           | 48.4 ms: 1.00x slower                                                                                                         |
| pidigits                   | 282 ms                                                                                                            | 283 ms: 1.00x slower                                                                                                          |
| regex_v8                   | 17.7 ms                                                                                                           | 17.8 ms: 1.00x slower                                                                                                         |
| logging_format             | 4.00 us                                                                                                           | 4.02 us: 1.01x slower                                                                                                         |
| regex_dna                  | 152 ms                                                                                                            | 153 ms: 1.01x slower                                                                                                          |
| scimark_lu                 | 78.1 ms                                                                                                           | 78.7 ms: 1.01x slower                                                                                                         |
| pycparser                  | 715 ms                                                                                                            | 721 ms: 1.01x slower                                                                                                          |
| pickle_list                | 2.90 us                                                                                                           | 2.94 us: 1.01x slower                                                                                                         |
| bench_mp_pool              | 45.6 ms                                                                                                           | 46.1 ms: 1.01x slower                                                                                                         |
| deepcopy                   | 236 us                                                                                                            | 239 us: 1.01x slower                                                                                                          |
| pathlib                    | 24.9 ms                                                                                                           | 25.2 ms: 1.01x slower                                                                                                         |
| scimark_sor                | 108 ms                                                                                                            | 110 ms: 1.01x slower                                                                                                          |
| async_generators           | 304 ms                                                                                                            | 309 ms: 1.01x slower                                                                                                          |
| logging_simple             | 3.67 us                                                                                                           | 3.72 us: 1.02x slower                                                                                                         |
| sympy_expand               | 258 ms                                                                                                            | 262 ms: 1.02x slower                                                                                                          |
| dask                       | 230 ms                                                                                                            | 234 ms: 1.02x slower                                                                                                          |
| async_tree_cpu_io_mixed    | 527 ms                                                                                                            | 536 ms: 1.02x slower                                                                                                          |
| dulwich_log                | 30.1 ms                                                                                                           | 30.6 ms: 1.02x slower                                                                                                         |
| async_tree_cpu_io_mixed_tg | 536 ms                                                                                                            | 546 ms: 1.02x slower                                                                                                          |
| async_tree_io              | 709 ms                                                                                                            | 722 ms: 1.02x slower                                                                                                          |
| sqlglot_parse              | 869 us                                                                                                            | 886 us: 1.02x slower                                                                                                          |
| async_tree_io_tg           | 678 ms                                                                                                            | 691 ms: 1.02x slower                                                                                                          |
| 2to3                       | 177 ms                                                                                                            | 181 ms: 1.02x slower                                                                                                          |
| async_tree_none_tg         | 265 ms                                                                                                            | 271 ms: 1.02x slower                                                                                                          |
| bench_thread_pool          | 519 us                                                                                                            | 530 us: 1.02x slower                                                                                                          |
| sqlglot_transpile          | 1.05 ms                                                                                                           | 1.08 ms: 1.02x slower                                                                                                         |
| telco                      | 4.72 ms                                                                                                           | 4.83 ms: 1.02x slower                                                                                                         |
| logging_silent             | 73.1 ns                                                                                                           | 75.0 ns: 1.03x slower                                                                                                         |
| chameleon                  | 5.20 ms                                                                                                           | 5.34 ms: 1.03x slower                                                                                                         |
| async_tree_memoization_tg  | 329 ms                                                                                                            | 338 ms: 1.03x slower                                                                                                          |
| async_tree_memoization     | 332 ms                                                                                                            | 341 ms: 1.03x slower                                                                                                          |
| sqlglot_normalize          | 195 ms                                                                                                            | 200 ms: 1.03x slower                                                                                                          |
| async_tree_none            | 257 ms                                                                                                            | 264 ms: 1.03x slower                                                                                                          |
| docutils                   | 1.51 sec                                                                                                          | 1.56 sec: 1.03x slower                                                                                                        |
| xml_etree_process          | 41.4 ms                                                                                                           | 42.7 ms: 1.03x slower                                                                                                         |
| deepcopy_memo              | 26.4 us                                                                                                           | 27.3 us: 1.03x slower                                                                                                         |
| mdp                        | 1.65 sec                                                                                                          | 1.71 sec: 1.03x slower                                                                                                        |
| sqlglot_optimize           | 36.5 ms                                                                                                           | 37.8 ms: 1.04x slower                                                                                                         |
| sqlite_synth               | 1.66 us                                                                                                           | 1.72 us: 1.04x slower                                                                                                         |
| typing_runtime_protocols   | 75.1 us                                                                                                           | 78.1 us: 1.04x slower                                                                                                         |
| unpickle_pure_python       | 166 us                                                                                                            | 174 us: 1.05x slower                                                                                                          |
| tornado_http               | 71.6 ms                                                                                                           | 74.9 ms: 1.05x slower                                                                                                         |
| go                         | 109 ms                                                                                                            | 115 ms: 1.05x slower                                                                                                          |
| tomli_loads                | 1.60 sec                                                                                                          | 1.70 sec: 1.06x slower                                                                                                        |
| sympy_str                  | 149 ms                                                                                                            | 158 ms: 1.06x slower                                                                                                          |
| xml_etree_iterparse        | 76.5 ms                                                                                                           | 81.1 ms: 1.06x slower                                                                                                         |
| xml_etree_generate         | 58.1 ms                                                                                                           | 62.3 ms: 1.07x slower                                                                                                         |
| sympy_integrate            | 11.2 ms                                                                                                           | 12.1 ms: 1.08x slower                                                                                                         |
| sympy_sum                  | 77.3 ms                                                                                                           | 83.4 ms: 1.08x slower                                                                                                         |
| pyflate                    | 350 ms                                                                                                            | 377 ms: 1.08x slower                                                                                                          |
| pprint_safe_repr           | 548 ms                                                                                                            | 594 ms: 1.08x slower                                                                                                          |
| meteor_contest             | 74.1 ms                                                                                                           | 80.3 ms: 1.08x slower                                                                                                         |
| raytrace                   | 183 ms                                                                                                            | 199 ms: 1.09x slower                                                                                                          |
| nbody                      | 82.5 ms                                                                                                           | 90.1 ms: 1.09x slower                                                                                                         |
| pprint_pformat             | 1.11 sec                                                                                                          | 1.22 sec: 1.09x slower                                                                                                        |
| crypto_pyaes               | 50.5 ms                                                                                                           | 55.9 ms: 1.11x slower                                                                                                         |
| nqueens                    | 62.8 ms                                                                                                           | 69.7 ms: 1.11x slower                                                                                                         |
| regex_compile              | 77.4 ms                                                                                                           | 87.5 ms: 1.13x slower                                                                                                         |
| chaos                      | 42.0 ms                                                                                                           | 48.2 ms: 1.15x slower                                                                                                         |
| float                      | 61.0 ms                                                                                                           | 70.9 ms: 1.16x slower                                                                                                         |
| fannkuch                   | 293 ms                                                                                                            | 341 ms: 1.16x slower                                                                                                          |
| scimark_monte_carlo        | 49.7 ms                                                                                                           | 59.3 ms: 1.19x slower                                                                                                         |
| scimark_fft                | 211 ms                                                                                                            | 253 ms: 1.20x slower                                                                                                          |
| mako                       | 8.04 ms                                                                                                           | 9.93 ms: 1.24x slower                                                                                                         |
| comprehensions             | 12.7 us                                                                                                           | 16.3 us: 1.28x slower                                                                                                         |
| hexiom                     | 4.70 ms                                                                                                           | 6.08 ms: 1.29x slower                                                                                                         |
| scimark_sparse_mat_mult    | 3.19 ms                                                                                                           | 4.21 ms: 1.32x slower                                                                                                         |
| spectral_norm              | 76.5 ms                                                                                                           | 106 ms: 1.38x slower                                                                                                          |
| deltablue                  | 2.53 ms                                                                                                           | 3.68 ms: 1.45x slower                                                                                                         |
| Geometric mean             | (ref)                                                                                                             | 1.05x slower                                                                                                                  |

Benchmark hidden because not significant (10): xml_etree_parse, python_startup, json_dumps, asyncio_websockets, asyncio_tcp_ssl, deepcopy_reduce, pickle_dict, asyncio_tcp, pickle, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.00x