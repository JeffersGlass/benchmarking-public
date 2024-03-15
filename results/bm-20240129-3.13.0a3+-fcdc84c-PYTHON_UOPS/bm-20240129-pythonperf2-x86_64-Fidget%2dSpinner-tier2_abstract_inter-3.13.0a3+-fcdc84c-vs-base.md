# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 309 ms                                                                       | 309 ms: 1.00x faster                                                                   |
| chameleon      | 7.86 ms                                                                      | 8.13 ms: 1.03x slower                                                                  |
| docutils       | 2.96 sec                                                                     | 2.93 sec: 1.01x faster                                                                 |
| tornado_http   | 130 ms                                                                       | 126 ms: 1.03x faster                                                                   |
| Geometric mean | (ref)                                                                        | 1.00x faster                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 449 ms                                                                       | 440 ms: 1.02x faster                                                                   |
| async_tree_memoization     | 561 ms                                                                       | 550 ms: 1.02x faster                                                                   |
| async_tree_none_tg         | 447 ms                                                                       | 440 ms: 1.01x faster                                                                   |
| async_tree_io_tg           | 1.09 sec                                                                     | 1.07 sec: 1.01x faster                                                                 |
| async_tree_io              | 1.09 sec                                                                     | 1.08 sec: 1.01x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 716 ms                                                                       | 709 ms: 1.01x faster                                                                   |
| async_tree_cpu_io_mixed    | 711 ms                                                                       | 705 ms: 1.01x faster                                                                   |
| Geometric mean             | (ref)                                                                        | 1.01x faster                                                                           |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| nbody          | 125 ms                                                                       | 111 ms: 1.13x faster                                                                   |
| float          | 98.8 ms                                                                      | 94.5 ms: 1.05x faster                                                                  |
| pidigits       | 265 ms                                                                       | 264 ms: 1.00x faster                                                                   |
| Geometric mean | (ref)                                                                        | 1.06x faster                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_dna      | 251 ms                                                                       | 236 ms: 1.06x faster                                                                   |
| regex_effbot   | 3.58 ms                                                                      | 3.42 ms: 1.05x faster                                                                  |
| regex_v8       | 26.2 ms                                                                      | 25.8 ms: 1.02x faster                                                                  |
| Geometric mean | (ref)                                                                        | 1.03x faster                                                                           |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| tomli_loads          | 2.74 sec                                                                     | 2.58 sec: 1.06x faster                                                                 |
| xml_etree_iterparse  | 117 ms                                                                       | 113 ms: 1.04x faster                                                                   |
| unpickle_list        | 4.90 us                                                                      | 4.76 us: 1.03x faster                                                                  |
| xml_etree_parse      | 151 ms                                                                       | 147 ms: 1.02x faster                                                                   |
| pickle_list          | 4.43 us                                                                      | 4.40 us: 1.01x faster                                                                  |
| xml_etree_process    | 61.6 ms                                                                      | 61.2 ms: 1.01x faster                                                                  |
| pickle_dict          | 32.6 us                                                                      | 32.4 us: 1.01x faster                                                                  |
| pickle               | 10.3 us                                                                      | 10.5 us: 1.02x slower                                                                  |
| unpickle_pure_python | 224 us                                                                       | 229 us: 1.02x slower                                                                   |
| unpickle             | 14.5 us                                                                      | 14.9 us: 1.03x slower                                                                  |
| pickle_pure_python   | 304 us                                                                       | 312 us: 1.03x slower                                                                   |
| Geometric mean       | (ref)                                                                        | 1.01x faster                                                                           |

Benchmark hidden because not significant (3): json_loads, json_dumps, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 12.7 ms                                                                      | 12.6 ms: 1.01x faster                                                                  |
| python_startup_no_site | 11.1 ms                                                                      | 11.1 ms: 1.01x faster                                                                  |
| Geometric mean         | (ref)                                                                        | 1.01x faster                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.4 ms                                                                      | 14.0 ms: 1.03x faster                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240129-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| spectral_norm              | 163 ms                                                                       | 135 ms: 1.20x faster                                                                   |
| nbody                      | 125 ms                                                                       | 111 ms: 1.13x faster                                                                   |
| gc_traversal               | 3.98 ms                                                                      | 3.53 ms: 1.13x faster                                                                  |
| deltablue                  | 5.35 ms                                                                      | 4.81 ms: 1.11x faster                                                                  |
| scimark_fft                | 417 ms                                                                       | 379 ms: 1.10x faster                                                                   |
| scimark_sparse_mat_mult    | 6.35 ms                                                                      | 5.82 ms: 1.09x faster                                                                  |
| fannkuch                   | 471 ms                                                                       | 438 ms: 1.08x faster                                                                   |
| comprehensions             | 24.9 us                                                                      | 23.2 us: 1.07x faster                                                                  |
| tomli_loads                | 2.74 sec                                                                     | 2.58 sec: 1.06x faster                                                                 |
| regex_dna                  | 251 ms                                                                       | 236 ms: 1.06x faster                                                                   |
| chaos                      | 76.2 ms                                                                      | 72.0 ms: 1.06x faster                                                                  |
| hexiom                     | 9.43 ms                                                                      | 8.99 ms: 1.05x faster                                                                  |
| regex_effbot               | 3.58 ms                                                                      | 3.42 ms: 1.05x faster                                                                  |
| logging_format             | 7.61 us                                                                      | 7.28 us: 1.05x faster                                                                  |
| float                      | 98.8 ms                                                                      | 94.5 ms: 1.05x faster                                                                  |
| nqueens                    | 107 ms                                                                       | 103 ms: 1.04x faster                                                                   |
| scimark_monte_carlo        | 85.2 ms                                                                      | 81.8 ms: 1.04x faster                                                                  |
| xml_etree_iterparse        | 117 ms                                                                       | 113 ms: 1.04x faster                                                                   |
| pyflate                    | 570 ms                                                                       | 554 ms: 1.03x faster                                                                   |
| mako                       | 14.4 ms                                                                      | 14.0 ms: 1.03x faster                                                                  |
| unpickle_list              | 4.90 us                                                                      | 4.76 us: 1.03x faster                                                                  |
| tornado_http               | 130 ms                                                                       | 126 ms: 1.03x faster                                                                   |
| dulwich_log                | 73.5 ms                                                                      | 71.7 ms: 1.03x faster                                                                  |
| crypto_pyaes               | 84.5 ms                                                                      | 82.5 ms: 1.02x faster                                                                  |
| xml_etree_parse            | 151 ms                                                                       | 147 ms: 1.02x faster                                                                   |
| logging_simple             | 6.87 us                                                                      | 6.73 us: 1.02x faster                                                                  |
| async_tree_none            | 449 ms                                                                       | 440 ms: 1.02x faster                                                                   |
| async_tree_memoization     | 561 ms                                                                       | 550 ms: 1.02x faster                                                                   |
| regex_v8                   | 26.2 ms                                                                      | 25.8 ms: 1.02x faster                                                                  |
| async_tree_none_tg         | 447 ms                                                                       | 440 ms: 1.01x faster                                                                   |
| async_tree_io_tg           | 1.09 sec                                                                     | 1.07 sec: 1.01x faster                                                                 |
| async_tree_io              | 1.09 sec                                                                     | 1.08 sec: 1.01x faster                                                                 |
| sympy_sum                  | 169 ms                                                                       | 167 ms: 1.01x faster                                                                   |
| sympy_integrate            | 25.0 ms                                                                      | 24.7 ms: 1.01x faster                                                                  |
| sympy_str                  | 322 ms                                                                       | 319 ms: 1.01x faster                                                                   |
| python_startup             | 12.7 ms                                                                      | 12.6 ms: 1.01x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 716 ms                                                                       | 709 ms: 1.01x faster                                                                   |
| sqlglot_parse              | 1.43 ms                                                                      | 1.42 ms: 1.01x faster                                                                  |
| async_tree_cpu_io_mixed    | 711 ms                                                                       | 705 ms: 1.01x faster                                                                   |
| asyncio_websockets         | 387 ms                                                                       | 384 ms: 1.01x faster                                                                   |
| pickle_list                | 4.43 us                                                                      | 4.40 us: 1.01x faster                                                                  |
| sqlglot_transpile          | 1.85 ms                                                                      | 1.84 ms: 1.01x faster                                                                  |
| docutils                   | 2.96 sec                                                                     | 2.93 sec: 1.01x faster                                                                 |
| asyncio_tcp                | 376 ms                                                                       | 373 ms: 1.01x faster                                                                   |
| xml_etree_process          | 61.6 ms                                                                      | 61.2 ms: 1.01x faster                                                                  |
| go                         | 179 ms                                                                       | 177 ms: 1.01x faster                                                                   |
| sqlglot_optimize           | 63.6 ms                                                                      | 63.2 ms: 1.01x faster                                                                  |
| python_startup_no_site     | 11.1 ms                                                                      | 11.1 ms: 1.01x faster                                                                  |
| pickle_dict                | 32.6 us                                                                      | 32.4 us: 1.01x faster                                                                  |
| 2to3                       | 309 ms                                                                       | 309 ms: 1.00x faster                                                                   |
| pidigits                   | 265 ms                                                                       | 264 ms: 1.00x faster                                                                   |
| asyncio_tcp_ssl            | 1.59 sec                                                                     | 1.59 sec: 1.00x faster                                                                 |
| meteor_contest             | 136 ms                                                                       | 136 ms: 1.00x slower                                                                   |
| generators                 | 33.8 ms                                                                      | 34.1 ms: 1.01x slower                                                                  |
| mdp                        | 2.63 sec                                                                     | 2.66 sec: 1.01x slower                                                                 |
| coverage                   | 77.5 ms                                                                      | 78.5 ms: 1.01x slower                                                                  |
| logging_silent             | 97.7 ns                                                                      | 99.5 ns: 1.02x slower                                                                  |
| pickle                     | 10.3 us                                                                      | 10.5 us: 1.02x slower                                                                  |
| typing_runtime_protocols   | 126 us                                                                       | 129 us: 1.02x slower                                                                   |
| async_generators           | 371 ms                                                                       | 379 ms: 1.02x slower                                                                   |
| unpickle_pure_python       | 224 us                                                                       | 229 us: 1.02x slower                                                                   |
| pathlib                    | 18.8 ms                                                                      | 19.2 ms: 1.02x slower                                                                  |
| deepcopy_reduce            | 3.33 us                                                                      | 3.41 us: 1.02x slower                                                                  |
| scimark_lu                 | 102 ms                                                                       | 104 ms: 1.02x slower                                                                   |
| unpickle                   | 14.5 us                                                                      | 14.9 us: 1.03x slower                                                                  |
| deepcopy                   | 374 us                                                                       | 384 us: 1.03x slower                                                                   |
| pickle_pure_python         | 304 us                                                                       | 312 us: 1.03x slower                                                                   |
| chameleon                  | 7.86 ms                                                                      | 8.13 ms: 1.03x slower                                                                  |
| scimark_sor                | 142 ms                                                                       | 147 ms: 1.04x slower                                                                   |
| deepcopy_memo              | 39.6 us                                                                      | 41.2 us: 1.04x slower                                                                  |
| unpack_sequence            | 41.3 ns                                                                      | 43.3 ns: 1.05x slower                                                                  |
| Geometric mean             | (ref)                                                                        | 1.02x faster                                                                           |

Benchmark hidden because not significant (22): bench_mp_pool, bench_thread_pool, async_tree_memoization_tg, create_gc_cycles, dask, telco, mypy2, sqlite_synth, richards_super, sympy_expand, json_loads, pprint_pformat, pprint_safe_repr, json_dumps, xml_etree_generate, pycparser, regex_compile, richards, sqlglot_normalize, raytrace, json, coroutines


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x