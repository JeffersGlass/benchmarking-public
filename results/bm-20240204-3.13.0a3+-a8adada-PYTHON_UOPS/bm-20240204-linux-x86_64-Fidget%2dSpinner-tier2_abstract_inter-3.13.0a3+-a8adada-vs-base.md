# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: a8adada
- commit date: 2024-02-04
- overall geometric mean: 1.00x slower
- HPT reliability: 99.79%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3+-b3f0b69 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 281 ms                                                                 | 282 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (3): chameleon, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3+-b3f0b69 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg         | 457 ms                                                                 | 459 ms: 1.00x slower                                                             |
| async_tree_io_tg           | 1.21 sec                                                               | 1.22 sec: 1.01x slower                                                           |
| async_tree_io              | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                           |
| async_tree_cpu_io_mixed_tg | 728 ms                                                                 | 737 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed    | 718 ms                                                                 | 727 ms: 1.01x slower                                                             |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3+-b3f0b69 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x slower                                                             |
| float          | 89.2 ms                                                                | 92.0 ms: 1.03x slower                                                            |
| nbody          | 113 ms                                                                 | 119 ms: 1.05x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3+-b3f0b69 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_v8       | 24.7 ms                                                                | 24.2 ms: 1.02x faster                                                            |
| regex_effbot   | 3.70 ms                                                                | 3.66 ms: 1.01x faster                                                            |
| regex_dna      | 224 ms                                                                 | 221 ms: 1.01x faster                                                             |
| regex_compile  | 147 ms                                                                 | 149 ms: 1.01x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3+-b3f0b69 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 2.53 sec                                                               | 2.35 sec: 1.07x faster                                                           |
| unpickle_list        | 5.11 us                                                                | 4.96 us: 1.03x faster                                                            |
| pickle_pure_python   | 302 us                                                                 | 299 us: 1.01x faster                                                             |
| pickle_list          | 5.17 us                                                                | 5.12 us: 1.01x faster                                                            |
| xml_etree_process    | 60.0 ms                                                                | 60.4 ms: 1.01x slower                                                            |
| unpickle_pure_python | 232 us                                                                 | 234 us: 1.01x slower                                                             |
| xml_etree_iterparse  | 108 ms                                                                 | 109 ms: 1.01x slower                                                             |
| json_loads           | 28.3 us                                                                | 28.7 us: 1.01x slower                                                            |
| xml_etree_parse      | 156 ms                                                                 | 158 ms: 1.01x slower                                                             |
| pickle_dict          | 34.2 us                                                                | 35.1 us: 1.02x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (4): unpickle, xml_etree_generate, json_dumps, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3+-b3f0b69 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| python_startup_no_site | 8.76 ms                                                                | 8.84 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3+-b3f0b69 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 13.3 ms                                                                | 13.6 ms: 1.02x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20240202-linux-x86_64-python-b3f0b698daf2438a6e59-3.13.0a3+-b3f0b69 | bm-20240204-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-a8adada |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpack_sequence            | 42.9 ns                                                                | 39.2 ns: 1.09x faster                                                            |
| tomli_loads                | 2.53 sec                                                               | 2.35 sec: 1.07x faster                                                           |
| pycparser                  | 1.26 sec                                                               | 1.21 sec: 1.04x faster                                                           |
| logging_silent             | 103 ns                                                                 | 99.1 ns: 1.04x faster                                                            |
| unpickle_list              | 5.11 us                                                                | 4.96 us: 1.03x faster                                                            |
| scimark_fft                | 427 ms                                                                 | 416 ms: 1.03x faster                                                             |
| sympy_integrate            | 21.1 ms                                                                | 20.7 ms: 1.02x faster                                                            |
| deepcopy_memo              | 41.1 us                                                                | 40.2 us: 1.02x faster                                                            |
| regex_v8                   | 24.7 ms                                                                | 24.2 ms: 1.02x faster                                                            |
| spectral_norm              | 137 ms                                                                 | 135 ms: 1.02x faster                                                             |
| comprehensions             | 20.9 us                                                                | 20.5 us: 1.02x faster                                                            |
| pyflate                    | 515 ms                                                                 | 509 ms: 1.01x faster                                                             |
| regex_effbot               | 3.70 ms                                                                | 3.66 ms: 1.01x faster                                                            |
| sympy_str                  | 292 ms                                                                 | 289 ms: 1.01x faster                                                             |
| regex_dna                  | 224 ms                                                                 | 221 ms: 1.01x faster                                                             |
| scimark_sor                | 124 ms                                                                 | 123 ms: 1.01x faster                                                             |
| pickle_pure_python         | 302 us                                                                 | 299 us: 1.01x faster                                                             |
| pickle_list                | 5.17 us                                                                | 5.12 us: 1.01x faster                                                            |
| richards_super             | 54.2 ms                                                                | 53.7 ms: 1.01x faster                                                            |
| raytrace                   | 298 ms                                                                 | 296 ms: 1.01x faster                                                             |
| coroutines                 | 22.0 ms                                                                | 21.9 ms: 1.01x faster                                                            |
| sympy_sum                  | 161 ms                                                                 | 160 ms: 1.01x faster                                                             |
| deepcopy_reduce            | 3.18 us                                                                | 3.16 us: 1.01x faster                                                            |
| deepcopy                   | 360 us                                                                 | 359 us: 1.00x faster                                                             |
| dulwich_log                | 68.9 ms                                                                | 68.6 ms: 1.00x faster                                                            |
| pidigits                   | 188 ms                                                                 | 188 ms: 1.00x slower                                                             |
| sqlglot_optimize           | 57.1 ms                                                                | 57.4 ms: 1.00x slower                                                            |
| 2to3                       | 281 ms                                                                 | 282 ms: 1.00x slower                                                             |
| async_tree_none_tg         | 457 ms                                                                 | 459 ms: 1.00x slower                                                             |
| sqlglot_parse              | 1.32 ms                                                                | 1.33 ms: 1.01x slower                                                            |
| async_tree_io_tg           | 1.21 sec                                                               | 1.22 sec: 1.01x slower                                                           |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                            |
| create_gc_cycles           | 1.48 ms                                                                | 1.49 ms: 1.01x slower                                                            |
| coverage                   | 94.5 ms                                                                | 95.1 ms: 1.01x slower                                                            |
| xml_etree_process          | 60.0 ms                                                                | 60.4 ms: 1.01x slower                                                            |
| unpickle_pure_python       | 232 us                                                                 | 234 us: 1.01x slower                                                             |
| meteor_contest             | 113 ms                                                                 | 114 ms: 1.01x slower                                                             |
| python_startup_no_site     | 8.76 ms                                                                | 8.84 ms: 1.01x slower                                                            |
| async_tree_io              | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                           |
| regex_compile              | 147 ms                                                                 | 149 ms: 1.01x slower                                                             |
| pprint_safe_repr           | 789 ms                                                                 | 799 ms: 1.01x slower                                                             |
| xml_etree_iterparse        | 108 ms                                                                 | 109 ms: 1.01x slower                                                             |
| pathlib                    | 18.4 ms                                                                | 18.7 ms: 1.01x slower                                                            |
| async_tree_cpu_io_mixed_tg | 728 ms                                                                 | 737 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed    | 718 ms                                                                 | 727 ms: 1.01x slower                                                             |
| json_loads                 | 28.3 us                                                                | 28.7 us: 1.01x slower                                                            |
| nqueens                    | 91.5 ms                                                                | 92.8 ms: 1.01x slower                                                            |
| xml_etree_parse            | 156 ms                                                                 | 158 ms: 1.01x slower                                                             |
| sqlglot_normalize          | 112 ms                                                                 | 114 ms: 1.02x slower                                                             |
| telco                      | 8.60 ms                                                                | 8.75 ms: 1.02x slower                                                            |
| asyncio_tcp                | 487 ms                                                                 | 496 ms: 1.02x slower                                                             |
| scimark_sparse_mat_mult    | 5.52 ms                                                                | 5.63 ms: 1.02x slower                                                            |
| scimark_lu                 | 115 ms                                                                 | 117 ms: 1.02x slower                                                             |
| scimark_monte_carlo        | 78.0 ms                                                                | 79.8 ms: 1.02x slower                                                            |
| pprint_pformat             | 1.63 sec                                                               | 1.67 sec: 1.02x slower                                                           |
| mako                       | 13.3 ms                                                                | 13.6 ms: 1.02x slower                                                            |
| pickle_dict                | 34.2 us                                                                | 35.1 us: 1.02x slower                                                            |
| crypto_pyaes               | 81.8 ms                                                                | 84.0 ms: 1.03x slower                                                            |
| go                         | 172 ms                                                                 | 177 ms: 1.03x slower                                                             |
| fannkuch                   | 434 ms                                                                 | 448 ms: 1.03x slower                                                             |
| float                      | 89.2 ms                                                                | 92.0 ms: 1.03x slower                                                            |
| gc_traversal               | 3.80 ms                                                                | 3.93 ms: 1.04x slower                                                            |
| hexiom                     | 8.02 ms                                                                | 8.34 ms: 1.04x slower                                                            |
| nbody                      | 113 ms                                                                 | 119 ms: 1.05x slower                                                             |
| mdp                        | 2.65 sec                                                               | 2.80 sec: 1.06x slower                                                           |
| Geometric mean             | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (28): unpickle, logging_simple, richards, sympy_expand, docutils, tornado_http, bench_thread_pool, sqlite_synth, asyncio_websockets, xml_etree_generate, chameleon, bench_mp_pool, async_tree_memoization_tg, async_generators, chaos, typing_runtime_protocols, asyncio_tcp_ssl, logging_format, generators, json_dumps, pickle, dask, sqlglot_transpile, deltablue, json, async_tree_memoization, mypy2, async_tree_none


# HPT report

- Reliability score: 99.79% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x