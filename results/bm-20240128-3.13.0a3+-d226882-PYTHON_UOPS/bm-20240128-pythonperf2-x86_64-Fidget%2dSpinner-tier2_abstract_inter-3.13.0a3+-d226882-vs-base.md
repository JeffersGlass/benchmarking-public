# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.01x faster
- HPT reliability: 99.76%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 309 ms                                                                       | 309 ms: 1.00x faster                                                                   |
| chameleon      | 7.86 ms                                                                      | 8.09 ms: 1.03x slower                                                                  |
| docutils       | 2.96 sec                                                                     | 2.95 sec: 1.00x faster                                                                 |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 449 ms                                                                       | 438 ms: 1.03x faster                                                                   |
| async_tree_memoization_tg  | 569 ms                                                                       | 555 ms: 1.03x faster                                                                   |
| async_tree_memoization     | 561 ms                                                                       | 549 ms: 1.02x faster                                                                   |
| async_tree_io              | 1.09 sec                                                                     | 1.07 sec: 1.02x faster                                                                 |
| async_tree_none_tg         | 447 ms                                                                       | 441 ms: 1.01x faster                                                                   |
| async_tree_cpu_io_mixed    | 711 ms                                                                       | 702 ms: 1.01x faster                                                                   |
| async_tree_io_tg           | 1.09 sec                                                                     | 1.07 sec: 1.01x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 716 ms                                                                       | 707 ms: 1.01x faster                                                                   |
| Geometric mean             | (ref)                                                                        | 1.02x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| nbody          | 125 ms                                                                       | 114 ms: 1.10x faster                                                                   |
| float          | 98.8 ms                                                                      | 95.3 ms: 1.04x faster                                                                  |
| pidigits       | 265 ms                                                                       | 264 ms: 1.00x faster                                                                   |
| Geometric mean | (ref)                                                                        | 1.04x faster                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_v8       | 26.2 ms                                                                      | 26.3 ms: 1.00x slower                                                                  |
| regex_compile  | 168 ms                                                                       | 169 ms: 1.01x slower                                                                   |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                                           |

Benchmark hidden because not significant (2): regex_effbot, regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| tomli_loads          | 2.74 sec                                                                     | 2.61 sec: 1.05x faster                                                                 |
| xml_etree_parse      | 151 ms                                                                       | 144 ms: 1.05x faster                                                                   |
| xml_etree_iterparse  | 117 ms                                                                       | 112 ms: 1.04x faster                                                                   |
| unpickle_list        | 4.90 us                                                                      | 4.75 us: 1.03x faster                                                                  |
| xml_etree_generate   | 90.2 ms                                                                      | 89.9 ms: 1.00x faster                                                                  |
| json_dumps           | 10.8 ms                                                                      | 10.8 ms: 1.00x slower                                                                  |
| json_loads           | 24.6 us                                                                      | 24.9 us: 1.01x slower                                                                  |
| unpickle_pure_python | 224 us                                                                       | 229 us: 1.02x slower                                                                   |
| pickle_pure_python   | 304 us                                                                       | 314 us: 1.03x slower                                                                   |
| pickle               | 10.3 us                                                                      | 10.7 us: 1.04x slower                                                                  |
| pickle_dict          | 32.6 us                                                                      | 34.6 us: 1.06x slower                                                                  |
| Geometric mean       | (ref)                                                                        | 1.00x slower                                                                           |

Benchmark hidden because not significant (3): unpickle, xml_etree_process, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 12.7 ms                                                                      | 12.7 ms: 1.00x faster                                                                  |
| python_startup_no_site | 11.1 ms                                                                      | 11.2 ms: 1.00x slower                                                                  |
| Geometric mean         | (ref)                                                                        | 1.00x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.4 ms                                                                      | 13.6 ms: 1.06x faster                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| spectral_norm              | 163 ms                                                                       | 144 ms: 1.13x faster                                                                   |
| gc_traversal               | 3.98 ms                                                                      | 3.56 ms: 1.12x faster                                                                  |
| nbody                      | 125 ms                                                                       | 114 ms: 1.10x faster                                                                   |
| deltablue                  | 5.35 ms                                                                      | 4.88 ms: 1.09x faster                                                                  |
| comprehensions             | 24.9 us                                                                      | 23.1 us: 1.07x faster                                                                  |
| mako                       | 14.4 ms                                                                      | 13.6 ms: 1.06x faster                                                                  |
| hexiom                     | 9.43 ms                                                                      | 8.91 ms: 1.06x faster                                                                  |
| logging_format             | 7.61 us                                                                      | 7.20 us: 1.06x faster                                                                  |
| fannkuch                   | 471 ms                                                                       | 446 ms: 1.05x faster                                                                   |
| scimark_fft                | 417 ms                                                                       | 396 ms: 1.05x faster                                                                   |
| tomli_loads                | 2.74 sec                                                                     | 2.61 sec: 1.05x faster                                                                 |
| xml_etree_parse            | 151 ms                                                                       | 144 ms: 1.05x faster                                                                   |
| xml_etree_iterparse        | 117 ms                                                                       | 112 ms: 1.04x faster                                                                   |
| scimark_sparse_mat_mult    | 6.35 ms                                                                      | 6.10 ms: 1.04x faster                                                                  |
| scimark_monte_carlo        | 85.2 ms                                                                      | 81.9 ms: 1.04x faster                                                                  |
| float                      | 98.8 ms                                                                      | 95.3 ms: 1.04x faster                                                                  |
| crypto_pyaes               | 84.5 ms                                                                      | 81.8 ms: 1.03x faster                                                                  |
| chaos                      | 76.2 ms                                                                      | 73.8 ms: 1.03x faster                                                                  |
| logging_simple             | 6.87 us                                                                      | 6.65 us: 1.03x faster                                                                  |
| unpickle_list              | 4.90 us                                                                      | 4.75 us: 1.03x faster                                                                  |
| nqueens                    | 107 ms                                                                       | 104 ms: 1.03x faster                                                                   |
| async_tree_none            | 449 ms                                                                       | 438 ms: 1.03x faster                                                                   |
| async_tree_memoization_tg  | 569 ms                                                                       | 555 ms: 1.03x faster                                                                   |
| async_tree_memoization     | 561 ms                                                                       | 549 ms: 1.02x faster                                                                   |
| richards_super             | 60.6 ms                                                                      | 59.4 ms: 1.02x faster                                                                  |
| async_tree_io              | 1.09 sec                                                                     | 1.07 sec: 1.02x faster                                                                 |
| asyncio_websockets         | 387 ms                                                                       | 380 ms: 1.02x faster                                                                   |
| pyflate                    | 570 ms                                                                       | 561 ms: 1.02x faster                                                                   |
| async_tree_none_tg         | 447 ms                                                                       | 441 ms: 1.01x faster                                                                   |
| telco                      | 8.39 ms                                                                      | 8.27 ms: 1.01x faster                                                                  |
| async_tree_cpu_io_mixed    | 711 ms                                                                       | 702 ms: 1.01x faster                                                                   |
| richards                   | 54.2 ms                                                                      | 53.5 ms: 1.01x faster                                                                  |
| async_tree_io_tg           | 1.09 sec                                                                     | 1.07 sec: 1.01x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 716 ms                                                                       | 707 ms: 1.01x faster                                                                   |
| mdp                        | 2.63 sec                                                                     | 2.61 sec: 1.01x faster                                                                 |
| go                         | 179 ms                                                                       | 177 ms: 1.01x faster                                                                   |
| sqlite_synth               | 2.82 us                                                                      | 2.81 us: 1.01x faster                                                                  |
| asyncio_tcp_ssl            | 1.59 sec                                                                     | 1.58 sec: 1.00x faster                                                                 |
| sqlglot_optimize           | 63.6 ms                                                                      | 63.4 ms: 1.00x faster                                                                  |
| xml_etree_generate         | 90.2 ms                                                                      | 89.9 ms: 1.00x faster                                                                  |
| sqlglot_normalize          | 122 ms                                                                       | 122 ms: 1.00x faster                                                                   |
| pidigits                   | 265 ms                                                                       | 264 ms: 1.00x faster                                                                   |
| docutils                   | 2.96 sec                                                                     | 2.95 sec: 1.00x faster                                                                 |
| 2to3                       | 309 ms                                                                       | 309 ms: 1.00x faster                                                                   |
| python_startup             | 12.7 ms                                                                      | 12.7 ms: 1.00x faster                                                                  |
| regex_v8                   | 26.2 ms                                                                      | 26.3 ms: 1.00x slower                                                                  |
| pprint_pformat             | 1.85 sec                                                                     | 1.85 sec: 1.00x slower                                                                 |
| python_startup_no_site     | 11.1 ms                                                                      | 11.2 ms: 1.00x slower                                                                  |
| sympy_integrate            | 25.0 ms                                                                      | 25.0 ms: 1.00x slower                                                                  |
| json_dumps                 | 10.8 ms                                                                      | 10.8 ms: 1.00x slower                                                                  |
| pprint_safe_repr           | 896 ms                                                                       | 901 ms: 1.01x slower                                                                   |
| sympy_str                  | 322 ms                                                                       | 325 ms: 1.01x slower                                                                   |
| regex_compile              | 168 ms                                                                       | 169 ms: 1.01x slower                                                                   |
| meteor_contest             | 136 ms                                                                       | 137 ms: 1.01x slower                                                                   |
| generators                 | 33.8 ms                                                                      | 34.2 ms: 1.01x slower                                                                  |
| async_generators           | 371 ms                                                                       | 375 ms: 1.01x slower                                                                   |
| json_loads                 | 24.6 us                                                                      | 24.9 us: 1.01x slower                                                                  |
| pathlib                    | 18.8 ms                                                                      | 19.1 ms: 1.01x slower                                                                  |
| pycparser                  | 1.33 sec                                                                     | 1.35 sec: 1.02x slower                                                                 |
| unpickle_pure_python       | 224 us                                                                       | 229 us: 1.02x slower                                                                   |
| sympy_expand               | 537 ms                                                                       | 547 ms: 1.02x slower                                                                   |
| unpack_sequence            | 41.3 ns                                                                      | 42.2 ns: 1.02x slower                                                                  |
| coverage                   | 77.5 ms                                                                      | 79.3 ms: 1.02x slower                                                                  |
| json                       | 5.18 ms                                                                      | 5.31 ms: 1.02x slower                                                                  |
| logging_silent             | 97.7 ns                                                                      | 100 ns: 1.03x slower                                                                   |
| chameleon                  | 7.86 ms                                                                      | 8.09 ms: 1.03x slower                                                                  |
| deepcopy_reduce            | 3.33 us                                                                      | 3.44 us: 1.03x slower                                                                  |
| pickle_pure_python         | 304 us                                                                       | 314 us: 1.03x slower                                                                   |
| scimark_lu                 | 102 ms                                                                       | 106 ms: 1.04x slower                                                                   |
| deepcopy_memo              | 39.6 us                                                                      | 41.3 us: 1.04x slower                                                                  |
| pickle                     | 10.3 us                                                                      | 10.7 us: 1.04x slower                                                                  |
| scimark_sor                | 142 ms                                                                       | 148 ms: 1.04x slower                                                                   |
| deepcopy                   | 374 us                                                                       | 391 us: 1.04x slower                                                                   |
| pickle_dict                | 32.6 us                                                                      | 34.6 us: 1.06x slower                                                                  |
| Geometric mean             | (ref)                                                                        | 1.01x faster                                                                           |

Benchmark hidden because not significant (19): tornado_http, coroutines, regex_effbot, bench_thread_pool, raytrace, regex_dna, unpickle, dulwich_log, sqlglot_parse, xml_etree_process, pickle_list, sqlglot_transpile, asyncio_tcp, sympy_sum, mypy2, create_gc_cycles, typing_runtime_protocols, dask, bench_mp_pool


# HPT report

- Reliability score: 99.76% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x