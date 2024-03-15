# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| chameleon      | 7.86 ms                                                                      | 7.83 ms: 1.00x faster                                                                  |
| docutils       | 2.96 sec                                                                     | 2.93 sec: 1.01x faster                                                                 |
| tornado_http   | 130 ms                                                                       | 127 ms: 1.02x faster                                                                   |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                                           |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|---------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none           | 449 ms                                                                       | 441 ms: 1.02x faster                                                                   |
| async_tree_memoization_tg | 569 ms                                                                       | 561 ms: 1.02x faster                                                                   |
| async_tree_memoization    | 561 ms                                                                       | 554 ms: 1.01x faster                                                                   |
| async_tree_none_tg        | 447 ms                                                                       | 441 ms: 1.01x faster                                                                   |
| async_tree_io_tg          | 1.09 sec                                                                     | 1.08 sec: 1.01x faster                                                                 |
| async_tree_cpu_io_mixed   | 711 ms                                                                       | 705 ms: 1.01x faster                                                                   |
| async_tree_io             | 1.09 sec                                                                     | 1.08 sec: 1.01x faster                                                                 |
| Geometric mean            | (ref)                                                                        | 1.01x faster                                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| nbody          | 125 ms                                                                       | 112 ms: 1.12x faster                                                                   |
| float          | 98.8 ms                                                                      | 94.0 ms: 1.05x faster                                                                  |
| Geometric mean | (ref)                                                                        | 1.05x faster                                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_dna      | 251 ms                                                                       | 241 ms: 1.04x faster                                                                   |
| regex_effbot   | 3.58 ms                                                                      | 3.47 ms: 1.03x faster                                                                  |
| regex_v8       | 26.2 ms                                                                      | 25.4 ms: 1.03x faster                                                                  |
| Geometric mean | (ref)                                                                        | 1.03x faster                                                                           |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| tomli_loads          | 2.74 sec                                                                     | 2.60 sec: 1.05x faster                                                                 |
| unpickle_list        | 4.90 us                                                                      | 4.74 us: 1.03x faster                                                                  |
| xml_etree_iterparse  | 117 ms                                                                       | 114 ms: 1.02x faster                                                                   |
| xml_etree_parse      | 151 ms                                                                       | 148 ms: 1.02x faster                                                                   |
| json_loads           | 24.6 us                                                                      | 24.8 us: 1.01x slower                                                                  |
| pickle_dict          | 32.6 us                                                                      | 32.8 us: 1.01x slower                                                                  |
| json_dumps           | 10.8 ms                                                                      | 10.9 ms: 1.01x slower                                                                  |
| pickle_list          | 4.43 us                                                                      | 4.52 us: 1.02x slower                                                                  |
| pickle_pure_python   | 304 us                                                                       | 314 us: 1.03x slower                                                                   |
| pickle               | 10.3 us                                                                      | 10.6 us: 1.04x slower                                                                  |
| unpickle             | 14.5 us                                                                      | 15.1 us: 1.04x slower                                                                  |
| unpickle_pure_python | 224 us                                                                       | 241 us: 1.08x slower                                                                   |
| Geometric mean       | (ref)                                                                        | 1.01x slower                                                                           |

Benchmark hidden because not significant (2): xml_etree_generate, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 12.7 ms                                                                      | 12.7 ms: 1.00x faster                                                                  |
| python_startup_no_site | 11.1 ms                                                                      | 11.2 ms: 1.01x slower                                                                  |
| Geometric mean         | (ref)                                                                        | 1.00x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.4 ms                                                                      | 13.3 ms: 1.08x faster                                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20240124-pythonperf2-x86_64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240127-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|---------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| spectral_norm             | 163 ms                                                                       | 138 ms: 1.18x faster                                                                   |
| gc_traversal              | 3.98 ms                                                                      | 3.53 ms: 1.13x faster                                                                  |
| nbody                     | 125 ms                                                                       | 112 ms: 1.12x faster                                                                   |
| deltablue                 | 5.35 ms                                                                      | 4.86 ms: 1.10x faster                                                                  |
| mako                      | 14.4 ms                                                                      | 13.3 ms: 1.08x faster                                                                  |
| comprehensions            | 24.9 us                                                                      | 23.0 us: 1.08x faster                                                                  |
| scimark_fft               | 417 ms                                                                       | 392 ms: 1.07x faster                                                                   |
| fannkuch                  | 471 ms                                                                       | 445 ms: 1.06x faster                                                                   |
| scimark_sparse_mat_mult   | 6.35 ms                                                                      | 6.01 ms: 1.06x faster                                                                  |
| tomli_loads               | 2.74 sec                                                                     | 2.60 sec: 1.05x faster                                                                 |
| float                     | 98.8 ms                                                                      | 94.0 ms: 1.05x faster                                                                  |
| scimark_monte_carlo       | 85.2 ms                                                                      | 81.1 ms: 1.05x faster                                                                  |
| crypto_pyaes              | 84.5 ms                                                                      | 80.5 ms: 1.05x faster                                                                  |
| chaos                     | 76.2 ms                                                                      | 72.8 ms: 1.05x faster                                                                  |
| nqueens                   | 107 ms                                                                       | 102 ms: 1.05x faster                                                                   |
| hexiom                    | 9.43 ms                                                                      | 9.05 ms: 1.04x faster                                                                  |
| regex_dna                 | 251 ms                                                                       | 241 ms: 1.04x faster                                                                   |
| unpickle_list             | 4.90 us                                                                      | 4.74 us: 1.03x faster                                                                  |
| regex_effbot              | 3.58 ms                                                                      | 3.47 ms: 1.03x faster                                                                  |
| regex_v8                  | 26.2 ms                                                                      | 25.4 ms: 1.03x faster                                                                  |
| richards_super            | 60.6 ms                                                                      | 59.1 ms: 1.03x faster                                                                  |
| xml_etree_iterparse       | 117 ms                                                                       | 114 ms: 1.02x faster                                                                   |
| dulwich_log               | 73.5 ms                                                                      | 72.0 ms: 1.02x faster                                                                  |
| tornado_http              | 130 ms                                                                       | 127 ms: 1.02x faster                                                                   |
| xml_etree_parse           | 151 ms                                                                       | 148 ms: 1.02x faster                                                                   |
| async_tree_none           | 449 ms                                                                       | 441 ms: 1.02x faster                                                                   |
| sqlglot_parse             | 1.43 ms                                                                      | 1.41 ms: 1.02x faster                                                                  |
| async_tree_memoization_tg | 569 ms                                                                       | 561 ms: 1.02x faster                                                                   |
| logging_format            | 7.61 us                                                                      | 7.50 us: 1.01x faster                                                                  |
| sqlglot_transpile         | 1.85 ms                                                                      | 1.82 ms: 1.01x faster                                                                  |
| sympy_sum                 | 169 ms                                                                       | 167 ms: 1.01x faster                                                                   |
| async_tree_memoization    | 561 ms                                                                       | 554 ms: 1.01x faster                                                                   |
| async_tree_none_tg        | 447 ms                                                                       | 441 ms: 1.01x faster                                                                   |
| richards                  | 54.2 ms                                                                      | 53.5 ms: 1.01x faster                                                                  |
| telco                     | 8.39 ms                                                                      | 8.29 ms: 1.01x faster                                                                  |
| coroutines                | 22.3 ms                                                                      | 22.0 ms: 1.01x faster                                                                  |
| mdp                       | 2.63 sec                                                                     | 2.60 sec: 1.01x faster                                                                 |
| sympy_integrate           | 25.0 ms                                                                      | 24.7 ms: 1.01x faster                                                                  |
| async_tree_io_tg          | 1.09 sec                                                                     | 1.08 sec: 1.01x faster                                                                 |
| async_tree_cpu_io_mixed   | 711 ms                                                                       | 705 ms: 1.01x faster                                                                   |
| async_tree_io             | 1.09 sec                                                                     | 1.08 sec: 1.01x faster                                                                 |
| docutils                  | 2.96 sec                                                                     | 2.93 sec: 1.01x faster                                                                 |
| asyncio_tcp               | 376 ms                                                                       | 373 ms: 1.01x faster                                                                   |
| sqlite_synth              | 2.82 us                                                                      | 2.80 us: 1.01x faster                                                                  |
| sympy_str                 | 322 ms                                                                       | 320 ms: 1.01x faster                                                                   |
| sqlglot_optimize          | 63.6 ms                                                                      | 63.3 ms: 1.00x faster                                                                  |
| chameleon                 | 7.86 ms                                                                      | 7.83 ms: 1.00x faster                                                                  |
| sqlglot_normalize         | 122 ms                                                                       | 122 ms: 1.00x faster                                                                   |
| python_startup            | 12.7 ms                                                                      | 12.7 ms: 1.00x faster                                                                  |
| meteor_contest            | 136 ms                                                                       | 136 ms: 1.00x slower                                                                   |
| pprint_safe_repr          | 896 ms                                                                       | 901 ms: 1.01x slower                                                                   |
| json_loads                | 24.6 us                                                                      | 24.8 us: 1.01x slower                                                                  |
| python_startup_no_site    | 11.1 ms                                                                      | 11.2 ms: 1.01x slower                                                                  |
| pickle_dict               | 32.6 us                                                                      | 32.8 us: 1.01x slower                                                                  |
| go                        | 179 ms                                                                       | 180 ms: 1.01x slower                                                                   |
| async_generators          | 371 ms                                                                       | 374 ms: 1.01x slower                                                                   |
| json_dumps                | 10.8 ms                                                                      | 10.9 ms: 1.01x slower                                                                  |
| generators                | 33.8 ms                                                                      | 34.2 ms: 1.01x slower                                                                  |
| scimark_sor               | 142 ms                                                                       | 143 ms: 1.01x slower                                                                   |
| pyflate                   | 570 ms                                                                       | 576 ms: 1.01x slower                                                                   |
| pathlib                   | 18.8 ms                                                                      | 19.0 ms: 1.01x slower                                                                  |
| json                      | 5.18 ms                                                                      | 5.25 ms: 1.01x slower                                                                  |
| logging_simple            | 6.87 us                                                                      | 6.98 us: 1.02x slower                                                                  |
| logging_silent            | 97.7 ns                                                                      | 99.6 ns: 1.02x slower                                                                  |
| pickle_list               | 4.43 us                                                                      | 4.52 us: 1.02x slower                                                                  |
| deepcopy                  | 374 us                                                                       | 383 us: 1.02x slower                                                                   |
| deepcopy_reduce           | 3.33 us                                                                      | 3.42 us: 1.03x slower                                                                  |
| scimark_lu                | 102 ms                                                                       | 104 ms: 1.03x slower                                                                   |
| deepcopy_memo             | 39.6 us                                                                      | 40.7 us: 1.03x slower                                                                  |
| pickle_pure_python        | 304 us                                                                       | 314 us: 1.03x slower                                                                   |
| pickle                    | 10.3 us                                                                      | 10.6 us: 1.04x slower                                                                  |
| coverage                  | 77.5 ms                                                                      | 80.4 ms: 1.04x slower                                                                  |
| unpickle                  | 14.5 us                                                                      | 15.1 us: 1.04x slower                                                                  |
| unpickle_pure_python      | 224 us                                                                       | 241 us: 1.08x slower                                                                   |
| unpack_sequence           | 41.3 ns                                                                      | 46.5 ns: 1.13x slower                                                                  |
| Geometric mean            | (ref)                                                                        | 1.01x faster                                                                           |

Benchmark hidden because not significant (18): bench_mp_pool, async_tree_cpu_io_mixed_tg, asyncio_websockets, bench_thread_pool, raytrace, dask, typing_runtime_protocols, xml_etree_generate, regex_compile, create_gc_cycles, asyncio_tcp_ssl, xml_etree_process, pidigits, 2to3, pprint_pformat, sympy_expand, pycparser, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x