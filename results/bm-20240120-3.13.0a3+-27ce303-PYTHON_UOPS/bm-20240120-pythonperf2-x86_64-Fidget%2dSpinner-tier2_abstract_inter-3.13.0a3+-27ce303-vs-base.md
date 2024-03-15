# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.02x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.28x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240118-pythonperf2-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 307 ms                                                                       | 316 ms: 1.03x slower                                                                   |
| chameleon      | 7.94 ms                                                                      | 8.17 ms: 1.03x slower                                                                  |
| docutils       | 2.94 sec                                                                     | 2.92 sec: 1.01x faster                                                                 |
| Geometric mean | (ref)                                                                        | 1.02x slower                                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240118-pythonperf2-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 562 ms                                                                       | 549 ms: 1.02x faster                                                                   |
| async_tree_io              | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                                 |
| async_tree_io_tg           | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                                 |
| async_tree_cpu_io_mixed_tg | 709 ms                                                                       | 716 ms: 1.01x slower                                                                   |
| async_tree_cpu_io_mixed    | 705 ms                                                                       | 713 ms: 1.01x slower                                                                   |
| async_tree_none            | 437 ms                                                                       | 444 ms: 1.02x slower                                                                   |
| async_tree_memoization     | 549 ms                                                                       | 560 ms: 1.02x slower                                                                   |
| async_tree_none_tg         | 436 ms                                                                       | 444 ms: 1.02x slower                                                                   |
| Geometric mean             | (ref)                                                                        | 1.01x slower                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240118-pythonperf2-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 264 ms                                                                       | 266 ms: 1.01x slower                                                                   |
| float          | 96.0 ms                                                                      | 105 ms: 1.10x slower                                                                   |
| nbody          | 120 ms                                                                       | 134 ms: 1.12x slower                                                                   |
| Geometric mean | (ref)                                                                        | 1.07x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240118-pythonperf2-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_dna      | 247 ms                                                                       | 240 ms: 1.03x faster                                                                   |
| regex_effbot   | 3.48 ms                                                                      | 3.50 ms: 1.00x slower                                                                  |
| regex_compile  | 167 ms                                                                       | 171 ms: 1.02x slower                                                                   |
| Geometric mean | (ref)                                                                        | 1.00x faster                                                                           |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240118-pythonperf2-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|---------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| unpickle            | 15.5 us                                                                      | 14.8 us: 1.04x faster                                                                  |
| xml_etree_parse     | 153 ms                                                                       | 147 ms: 1.04x faster                                                                   |
| unpickle_list       | 4.79 us                                                                      | 4.69 us: 1.02x faster                                                                  |
| json_dumps          | 10.9 ms                                                                      | 10.8 ms: 1.01x faster                                                                  |
| pickle_pure_python  | 311 us                                                                       | 310 us: 1.01x faster                                                                   |
| xml_etree_process   | 61.6 ms                                                                      | 62.0 ms: 1.01x slower                                                                  |
| xml_etree_generate  | 91.0 ms                                                                      | 91.7 ms: 1.01x slower                                                                  |
| json_loads          | 24.6 us                                                                      | 24.8 us: 1.01x slower                                                                  |
| xml_etree_iterparse | 115 ms                                                                       | 118 ms: 1.02x slower                                                                   |
| pickle_dict         | 30.7 us                                                                      | 32.4 us: 1.06x slower                                                                  |
| tomli_loads         | 2.62 sec                                                                     | 2.83 sec: 1.08x slower                                                                 |
| Geometric mean      | (ref)                                                                        | 1.00x slower                                                                           |

Benchmark hidden because not significant (3): pickle, unpickle_pure_python, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240118-pythonperf2-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 12.6 ms                                                                      | 12.7 ms: 1.01x slower                                                                  |
| python_startup_no_site | 11.1 ms                                                                      | 11.1 ms: 1.01x slower                                                                  |
| Geometric mean         | (ref)                                                                        | 1.01x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240118-pythonperf2-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 13.5 ms                                                                      | 14.8 ms: 1.09x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20240118-pythonperf2-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| unpickle                   | 15.5 us                                                                      | 14.8 us: 1.04x faster                                                                  |
| asyncio_websockets         | 391 ms                                                                       | 376 ms: 1.04x faster                                                                   |
| xml_etree_parse            | 153 ms                                                                       | 147 ms: 1.04x faster                                                                   |
| unpack_sequence            | 47.1 ns                                                                      | 45.5 ns: 1.04x faster                                                                  |
| regex_dna                  | 247 ms                                                                       | 240 ms: 1.03x faster                                                                   |
| coverage                   | 82.2 ms                                                                      | 80.2 ms: 1.03x faster                                                                  |
| async_tree_memoization_tg  | 562 ms                                                                       | 549 ms: 1.02x faster                                                                   |
| unpickle_list              | 4.79 us                                                                      | 4.69 us: 1.02x faster                                                                  |
| generators                 | 34.5 ms                                                                      | 33.9 ms: 1.02x faster                                                                  |
| create_gc_cycles           | 1.60 ms                                                                      | 1.58 ms: 1.02x faster                                                                  |
| gc_traversal               | 3.57 ms                                                                      | 3.52 ms: 1.01x faster                                                                  |
| json_dumps                 | 10.9 ms                                                                      | 10.8 ms: 1.01x faster                                                                  |
| sqlite_synth               | 2.84 us                                                                      | 2.82 us: 1.01x faster                                                                  |
| async_generators           | 373 ms                                                                       | 370 ms: 1.01x faster                                                                   |
| docutils                   | 2.94 sec                                                                     | 2.92 sec: 1.01x faster                                                                 |
| pickle_pure_python         | 311 us                                                                       | 310 us: 1.01x faster                                                                   |
| asyncio_tcp_ssl            | 1.59 sec                                                                     | 1.59 sec: 1.00x slower                                                                 |
| dulwich_log                | 71.6 ms                                                                      | 71.9 ms: 1.00x slower                                                                  |
| regex_effbot               | 3.48 ms                                                                      | 3.50 ms: 1.00x slower                                                                  |
| pidigits                   | 264 ms                                                                       | 266 ms: 1.01x slower                                                                   |
| async_tree_io              | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                                 |
| xml_etree_process          | 61.6 ms                                                                      | 62.0 ms: 1.01x slower                                                                  |
| python_startup             | 12.6 ms                                                                      | 12.7 ms: 1.01x slower                                                                  |
| richards                   | 54.3 ms                                                                      | 54.7 ms: 1.01x slower                                                                  |
| coroutines                 | 22.1 ms                                                                      | 22.2 ms: 1.01x slower                                                                  |
| sqlglot_normalize          | 123 ms                                                                       | 124 ms: 1.01x slower                                                                   |
| python_startup_no_site     | 11.1 ms                                                                      | 11.1 ms: 1.01x slower                                                                  |
| xml_etree_generate         | 91.0 ms                                                                      | 91.7 ms: 1.01x slower                                                                  |
| json_loads                 | 24.6 us                                                                      | 24.8 us: 1.01x slower                                                                  |
| pathlib                    | 18.9 ms                                                                      | 19.0 ms: 1.01x slower                                                                  |
| async_tree_io_tg           | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                                 |
| async_tree_cpu_io_mixed_tg | 709 ms                                                                       | 716 ms: 1.01x slower                                                                   |
| async_tree_cpu_io_mixed    | 705 ms                                                                       | 713 ms: 1.01x slower                                                                   |
| richards_super             | 60.4 ms                                                                      | 61.1 ms: 1.01x slower                                                                  |
| async_tree_none            | 437 ms                                                                       | 444 ms: 1.02x slower                                                                   |
| meteor_contest             | 136 ms                                                                       | 138 ms: 1.02x slower                                                                   |
| sympy_expand               | 526 ms                                                                       | 535 ms: 1.02x slower                                                                   |
| scimark_lu                 | 104 ms                                                                       | 105 ms: 1.02x slower                                                                   |
| logging_silent             | 98.0 ns                                                                      | 99.8 ns: 1.02x slower                                                                  |
| async_tree_memoization     | 549 ms                                                                       | 560 ms: 1.02x slower                                                                   |
| async_tree_none_tg         | 436 ms                                                                       | 444 ms: 1.02x slower                                                                   |
| spectral_norm              | 149 ms                                                                       | 152 ms: 1.02x slower                                                                   |
| sqlglot_optimize           | 62.8 ms                                                                      | 64.2 ms: 1.02x slower                                                                  |
| sympy_sum                  | 165 ms                                                                       | 169 ms: 1.02x slower                                                                   |
| raytrace                   | 297 ms                                                                       | 304 ms: 1.02x slower                                                                   |
| sympy_integrate            | 24.5 ms                                                                      | 25.1 ms: 1.02x slower                                                                  |
| regex_compile              | 167 ms                                                                       | 171 ms: 1.02x slower                                                                   |
| pprint_safe_repr           | 899 ms                                                                       | 920 ms: 1.02x slower                                                                   |
| xml_etree_iterparse        | 115 ms                                                                       | 118 ms: 1.02x slower                                                                   |
| deepcopy_reduce            | 3.32 us                                                                      | 3.41 us: 1.02x slower                                                                  |
| logging_format             | 7.23 us                                                                      | 7.42 us: 1.03x slower                                                                  |
| sympy_str                  | 315 ms                                                                       | 324 ms: 1.03x slower                                                                   |
| deepcopy                   | 374 us                                                                       | 384 us: 1.03x slower                                                                   |
| pprint_pformat             | 1.85 sec                                                                     | 1.90 sec: 1.03x slower                                                                 |
| chameleon                  | 7.94 ms                                                                      | 8.17 ms: 1.03x slower                                                                  |
| pycparser                  | 1.31 sec                                                                     | 1.36 sec: 1.03x slower                                                                 |
| 2to3                       | 307 ms                                                                       | 316 ms: 1.03x slower                                                                   |
| telco                      | 8.26 ms                                                                      | 8.54 ms: 1.03x slower                                                                  |
| logging_simple             | 6.71 us                                                                      | 6.94 us: 1.03x slower                                                                  |
| mdp                        | 2.59 sec                                                                     | 2.69 sec: 1.04x slower                                                                 |
| deepcopy_memo              | 39.4 us                                                                      | 40.9 us: 1.04x slower                                                                  |
| scimark_fft                | 406 ms                                                                       | 424 ms: 1.05x slower                                                                   |
| typing_runtime_protocols   | 122 us                                                                       | 128 us: 1.05x slower                                                                   |
| fannkuch                   | 454 ms                                                                       | 478 ms: 1.05x slower                                                                   |
| crypto_pyaes               | 82.1 ms                                                                      | 86.6 ms: 1.06x slower                                                                  |
| pickle_dict                | 30.7 us                                                                      | 32.4 us: 1.06x slower                                                                  |
| go                         | 175 ms                                                                       | 185 ms: 1.06x slower                                                                   |
| pyflate                    | 550 ms                                                                       | 588 ms: 1.07x slower                                                                   |
| chaos                      | 72.9 ms                                                                      | 77.9 ms: 1.07x slower                                                                  |
| scimark_sparse_mat_mult    | 6.10 ms                                                                      | 6.58 ms: 1.08x slower                                                                  |
| tomli_loads                | 2.62 sec                                                                     | 2.83 sec: 1.08x slower                                                                 |
| nqueens                    | 102 ms                                                                       | 111 ms: 1.08x slower                                                                   |
| mako                       | 13.5 ms                                                                      | 14.8 ms: 1.09x slower                                                                  |
| float                      | 96.0 ms                                                                      | 105 ms: 1.10x slower                                                                   |
| hexiom                     | 9.01 ms                                                                      | 9.90 ms: 1.10x slower                                                                  |
| deltablue                  | 5.00 ms                                                                      | 5.50 ms: 1.10x slower                                                                  |
| scimark_monte_carlo        | 81.5 ms                                                                      | 90.4 ms: 1.11x slower                                                                  |
| comprehensions             | 23.1 us                                                                      | 25.7 us: 1.11x slower                                                                  |
| nbody                      | 120 ms                                                                       | 134 ms: 1.12x slower                                                                   |
| Geometric mean             | (ref)                                                                        | 1.02x slower                                                                           |

Benchmark hidden because not significant (14): bench_mp_pool, regex_v8, pickle, unpickle_pure_python, pickle_list, sqlglot_parse, asyncio_tcp, json, sqlglot_transpile, bench_thread_pool, scimark_sor, dask, mypy2, tornado_http


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.28x