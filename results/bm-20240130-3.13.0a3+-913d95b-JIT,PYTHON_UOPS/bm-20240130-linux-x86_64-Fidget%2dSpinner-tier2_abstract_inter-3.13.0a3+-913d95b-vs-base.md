# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.01x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 275 ms                                                                 | 280 ms: 1.02x slower                                                             |
| docutils       | 2.64 sec                                                               | 2.68 sec: 1.02x slower                                                           |
| tornado_http   | 97.3 ms                                                                | 97.9 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 572 ms                                                                 | 580 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 715 ms                                                                 | 724 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed    | 705 ms                                                                 | 717 ms: 1.02x slower                                                             |
| async_tree_none_tg         | 445 ms                                                                 | 453 ms: 1.02x slower                                                             |
| async_tree_memoization     | 559 ms                                                                 | 570 ms: 1.02x slower                                                             |
| async_tree_io              | 1.16 sec                                                               | 1.19 sec: 1.02x slower                                                           |
| async_tree_io_tg           | 1.18 sec                                                               | 1.20 sec: 1.02x slower                                                           |
| Geometric mean             | (ref)                                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 106 ms                                                                 | 99.8 ms: 1.07x faster                                                            |
| pidigits       | 188 ms                                                                 | 188 ms: 1.00x slower                                                             |
| float          | 86.2 ms                                                                | 86.6 ms: 1.00x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 225 ms                                                                 | 222 ms: 1.01x faster                                                             |
| regex_compile  | 141 ms                                                                 | 143 ms: 1.01x slower                                                             |
| regex_effbot   | 3.59 ms                                                                | 3.67 ms: 1.02x slower                                                            |
| regex_v8       | 24.6 ms                                                                | 25.2 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle             | 16.0 us                                                                | 14.7 us: 1.09x faster                                                            |
| tomli_loads          | 2.24 sec                                                               | 2.22 sec: 1.01x faster                                                           |
| unpickle_list        | 5.27 us                                                                | 5.22 us: 1.01x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                                 | 109 ms: 1.01x slower                                                             |
| xml_etree_generate   | 87.0 ms                                                                | 87.7 ms: 1.01x slower                                                            |
| pickle_pure_python   | 297 us                                                                 | 300 us: 1.01x slower                                                             |
| json_dumps           | 10.2 ms                                                                | 10.4 ms: 1.02x slower                                                            |
| unpickle_pure_python | 224 us                                                                 | 229 us: 1.02x slower                                                             |
| pickle_dict          | 34.0 us                                                                | 35.0 us: 1.03x slower                                                            |
| pickle_list          | 4.98 us                                                                | 5.20 us: 1.04x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (4): pickle, xml_etree_process, json_loads, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.2 ms                                                                | 10.3 ms: 1.01x slower                                                            |
| python_startup_no_site | 8.82 ms                                                                | 8.93 ms: 1.01x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20240129-linux-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle                   | 16.0 us                                                                | 14.7 us: 1.09x faster                                                            |
| scimark_sor                | 134 ms                                                                 | 125 ms: 1.07x faster                                                             |
| nbody                      | 106 ms                                                                 | 99.8 ms: 1.07x faster                                                            |
| chaos                      | 73.1 ms                                                                | 69.5 ms: 1.05x faster                                                            |
| scimark_fft                | 386 ms                                                                 | 372 ms: 1.04x faster                                                             |
| spectral_norm              | 139 ms                                                                 | 135 ms: 1.03x faster                                                             |
| scimark_sparse_mat_mult    | 5.73 ms                                                                | 5.57 ms: 1.03x faster                                                            |
| pathlib                    | 18.6 ms                                                                | 18.2 ms: 1.02x faster                                                            |
| deltablue                  | 4.07 ms                                                                | 4.01 ms: 1.01x faster                                                            |
| fannkuch                   | 434 ms                                                                 | 428 ms: 1.01x faster                                                             |
| coverage                   | 95.8 ms                                                                | 94.6 ms: 1.01x faster                                                            |
| regex_dna                  | 225 ms                                                                 | 222 ms: 1.01x faster                                                             |
| telco                      | 8.53 ms                                                                | 8.43 ms: 1.01x faster                                                            |
| scimark_lu                 | 114 ms                                                                 | 113 ms: 1.01x faster                                                             |
| tomli_loads                | 2.24 sec                                                               | 2.22 sec: 1.01x faster                                                           |
| raytrace                   | 284 ms                                                                 | 281 ms: 1.01x faster                                                             |
| unpickle_list              | 5.27 us                                                                | 5.22 us: 1.01x faster                                                            |
| sqlite_synth               | 2.85 us                                                                | 2.82 us: 1.01x faster                                                            |
| pidigits                   | 188 ms                                                                 | 188 ms: 1.00x slower                                                             |
| generators                 | 29.6 ms                                                                | 29.7 ms: 1.00x slower                                                            |
| float                      | 86.2 ms                                                                | 86.6 ms: 1.00x slower                                                            |
| asyncio_websockets         | 552 ms                                                                 | 555 ms: 1.01x slower                                                             |
| pycparser                  | 1.16 sec                                                               | 1.17 sec: 1.01x slower                                                           |
| asyncio_tcp_ssl            | 1.80 sec                                                               | 1.81 sec: 1.01x slower                                                           |
| tornado_http               | 97.3 ms                                                                | 97.9 ms: 1.01x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                                 | 109 ms: 1.01x slower                                                             |
| xml_etree_generate         | 87.0 ms                                                                | 87.7 ms: 1.01x slower                                                            |
| create_gc_cycles           | 1.49 ms                                                                | 1.50 ms: 1.01x slower                                                            |
| python_startup             | 10.2 ms                                                                | 10.3 ms: 1.01x slower                                                            |
| sqlglot_optimize           | 55.9 ms                                                                | 56.5 ms: 1.01x slower                                                            |
| dulwich_log                | 67.8 ms                                                                | 68.5 ms: 1.01x slower                                                            |
| logging_simple             | 5.79 us                                                                | 5.86 us: 1.01x slower                                                            |
| pickle_pure_python         | 297 us                                                                 | 300 us: 1.01x slower                                                             |
| sqlglot_parse              | 1.27 ms                                                                | 1.29 ms: 1.01x slower                                                            |
| sympy_expand               | 480 ms                                                                 | 485 ms: 1.01x slower                                                             |
| richards                   | 46.1 ms                                                                | 46.6 ms: 1.01x slower                                                            |
| deepcopy                   | 345 us                                                                 | 349 us: 1.01x slower                                                             |
| python_startup_no_site     | 8.82 ms                                                                | 8.93 ms: 1.01x slower                                                            |
| async_tree_memoization_tg  | 572 ms                                                                 | 580 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 715 ms                                                                 | 724 ms: 1.01x slower                                                             |
| pprint_safe_repr           | 798 ms                                                                 | 809 ms: 1.01x slower                                                             |
| richards_super             | 52.1 ms                                                                | 52.9 ms: 1.01x slower                                                            |
| regex_compile              | 141 ms                                                                 | 143 ms: 1.01x slower                                                             |
| docutils                   | 2.64 sec                                                               | 2.68 sec: 1.02x slower                                                           |
| sqlglot_transpile          | 1.60 ms                                                                | 1.62 ms: 1.02x slower                                                            |
| logging_silent             | 101 ns                                                                 | 102 ns: 1.02x slower                                                             |
| async_tree_cpu_io_mixed    | 705 ms                                                                 | 717 ms: 1.02x slower                                                             |
| sympy_sum                  | 160 ms                                                                 | 162 ms: 1.02x slower                                                             |
| json_dumps                 | 10.2 ms                                                                | 10.4 ms: 1.02x slower                                                            |
| 2to3                       | 275 ms                                                                 | 280 ms: 1.02x slower                                                             |
| async_tree_none_tg         | 445 ms                                                                 | 453 ms: 1.02x slower                                                             |
| async_tree_memoization     | 559 ms                                                                 | 570 ms: 1.02x slower                                                             |
| json                       | 5.09 ms                                                                | 5.19 ms: 1.02x slower                                                            |
| deepcopy_memo              | 38.0 us                                                                | 38.8 us: 1.02x slower                                                            |
| go                         | 149 ms                                                                 | 152 ms: 1.02x slower                                                             |
| unpickle_pure_python       | 224 us                                                                 | 229 us: 1.02x slower                                                             |
| async_tree_io              | 1.16 sec                                                               | 1.19 sec: 1.02x slower                                                           |
| asyncio_tcp                | 485 ms                                                                 | 495 ms: 1.02x slower                                                             |
| sympy_integrate            | 20.8 ms                                                                | 21.3 ms: 1.02x slower                                                            |
| sqlglot_normalize          | 109 ms                                                                 | 111 ms: 1.02x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                                               | 1.20 sec: 1.02x slower                                                           |
| sympy_str                  | 285 ms                                                                 | 291 ms: 1.02x slower                                                             |
| regex_effbot               | 3.59 ms                                                                | 3.67 ms: 1.02x slower                                                            |
| deepcopy_reduce            | 3.01 us                                                                | 3.08 us: 1.02x slower                                                            |
| regex_v8                   | 24.6 ms                                                                | 25.2 ms: 1.02x slower                                                            |
| crypto_pyaes               | 78.8 ms                                                                | 81.1 ms: 1.03x slower                                                            |
| pickle_dict                | 34.0 us                                                                | 35.0 us: 1.03x slower                                                            |
| mdp                        | 2.65 sec                                                               | 2.74 sec: 1.03x slower                                                           |
| gc_traversal               | 3.73 ms                                                                | 3.87 ms: 1.04x slower                                                            |
| coroutines                 | 22.3 ms                                                                | 23.2 ms: 1.04x slower                                                            |
| pickle_list                | 4.98 us                                                                | 5.20 us: 1.04x slower                                                            |
| unpack_sequence            | 41.2 ns                                                                | 43.2 ns: 1.05x slower                                                            |
| hexiom                     | 8.13 ms                                                                | 8.65 ms: 1.06x slower                                                            |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (20): meteor_contest, async_generators, pickle, nqueens, typing_runtime_protocols, mako, chameleon, comprehensions, bench_mp_pool, pyflate, xml_etree_process, bench_thread_pool, json_loads, logging_format, dask, xml_etree_parse, scimark_monte_carlo, mypy2, async_tree_none, pprint_pformat


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x