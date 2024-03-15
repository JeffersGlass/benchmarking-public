# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.00x faster
- HPT reliability: 83.71%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 300 ms                                                                       | 303 ms: 1.01x slower                                                                   |
| chameleon      | 7.82 ms                                                                      | 7.67 ms: 1.02x faster                                                                  |
| docutils       | 2.89 sec                                                                     | 2.90 sec: 1.01x slower                                                                 |
| tornado_http   | 124 ms                                                                       | 126 ms: 1.02x slower                                                                   |
| Geometric mean | (ref)                                                                        | 1.00x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none_tg | 440 ms                                                                       | 438 ms: 1.01x faster                                                                   |
| Geometric mean     | (ref)                                                                        | 1.00x faster                                                                           |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_io_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| nbody          | 107 ms                                                                       | 104 ms: 1.03x faster                                                                   |
| pidigits       | 263 ms                                                                       | 263 ms: 1.00x slower                                                                   |
| float          | 81.6 ms                                                                      | 82.1 ms: 1.01x slower                                                                  |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_effbot   | 3.58 ms                                                                      | 3.59 ms: 1.00x slower                                                                  |
| regex_compile  | 146 ms                                                                       | 147 ms: 1.01x slower                                                                   |
| regex_v8       | 25.3 ms                                                                      | 25.6 ms: 1.01x slower                                                                  |
| regex_dna      | 236 ms                                                                       | 241 ms: 1.02x slower                                                                   |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| unpickle_pure_python | 229 us                                                                       | 224 us: 1.02x faster                                                                   |
| xml_etree_generate   | 86.3 ms                                                                      | 85.1 ms: 1.01x faster                                                                  |
| unpickle             | 15.5 us                                                                      | 15.3 us: 1.01x faster                                                                  |
| xml_etree_process    | 59.1 ms                                                                      | 58.6 ms: 1.01x faster                                                                  |
| unpickle_list        | 4.98 us                                                                      | 4.95 us: 1.01x faster                                                                  |
| json_dumps           | 10.6 ms                                                                      | 10.7 ms: 1.01x slower                                                                  |
| xml_etree_iterparse  | 106 ms                                                                       | 107 ms: 1.01x slower                                                                   |
| tomli_loads          | 2.32 sec                                                                     | 2.34 sec: 1.01x slower                                                                 |
| json_loads           | 25.1 us                                                                      | 25.3 us: 1.01x slower                                                                  |
| pickle               | 10.3 us                                                                      | 10.4 us: 1.02x slower                                                                  |
| pickle_list          | 4.25 us                                                                      | 4.37 us: 1.03x slower                                                                  |
| Geometric mean       | (ref)                                                                        | 1.00x slower                                                                           |

Benchmark hidden because not significant (3): pickle_pure_python, pickle_dict, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 12.7 ms                                                                      | 12.7 ms: 1.00x slower                                                                  |
| python_startup_no_site | 11.1 ms                                                                      | 11.2 ms: 1.01x slower                                                                  |
| Geometric mean         | (ref)                                                                        | 1.01x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                                      | 11.8 ms: 1.01x faster                                                                  |

All benchmarks:
===============

| Benchmark                | bm-20240129-pythonperf2-x86_64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| gc_traversal             | 3.67 ms                                                                      | 3.42 ms: 1.07x faster                                                                  |
| coverage                 | 86.4 ms                                                                      | 80.7 ms: 1.07x faster                                                                  |
| bench_mp_pool            | 5.28 ms                                                                      | 5.00 ms: 1.06x faster                                                                  |
| deepcopy                 | 380 us                                                                       | 363 us: 1.05x faster                                                                   |
| deepcopy_memo            | 39.0 us                                                                      | 37.5 us: 1.04x faster                                                                  |
| deepcopy_reduce          | 3.38 us                                                                      | 3.28 us: 1.03x faster                                                                  |
| pyflate                  | 534 ms                                                                       | 517 ms: 1.03x faster                                                                   |
| nbody                    | 107 ms                                                                       | 104 ms: 1.03x faster                                                                   |
| pycparser                | 1.30 sec                                                                     | 1.27 sec: 1.02x faster                                                                 |
| chameleon                | 7.82 ms                                                                      | 7.67 ms: 1.02x faster                                                                  |
| unpickle_pure_python     | 229 us                                                                       | 224 us: 1.02x faster                                                                   |
| typing_runtime_protocols | 124 us                                                                       | 122 us: 1.02x faster                                                                   |
| scimark_fft              | 366 ms                                                                       | 359 ms: 1.02x faster                                                                   |
| deltablue                | 4.01 ms                                                                      | 3.94 ms: 1.02x faster                                                                  |
| xml_etree_generate       | 86.3 ms                                                                      | 85.1 ms: 1.01x faster                                                                  |
| pathlib                  | 18.7 ms                                                                      | 18.4 ms: 1.01x faster                                                                  |
| unpickle                 | 15.5 us                                                                      | 15.3 us: 1.01x faster                                                                  |
| chaos                    | 70.6 ms                                                                      | 69.8 ms: 1.01x faster                                                                  |
| go                       | 170 ms                                                                       | 168 ms: 1.01x faster                                                                   |
| asyncio_websockets       | 386 ms                                                                       | 383 ms: 1.01x faster                                                                   |
| xml_etree_process        | 59.1 ms                                                                      | 58.6 ms: 1.01x faster                                                                  |
| logging_silent           | 96.3 ns                                                                      | 95.6 ns: 1.01x faster                                                                  |
| mako                     | 11.9 ms                                                                      | 11.8 ms: 1.01x faster                                                                  |
| async_tree_none_tg       | 440 ms                                                                       | 438 ms: 1.01x faster                                                                   |
| unpickle_list            | 4.98 us                                                                      | 4.95 us: 1.01x faster                                                                  |
| scimark_sparse_mat_mult  | 5.23 ms                                                                      | 5.22 ms: 1.00x faster                                                                  |
| pidigits                 | 263 ms                                                                       | 263 ms: 1.00x slower                                                                   |
| mdp                      | 2.54 sec                                                                     | 2.55 sec: 1.00x slower                                                                 |
| regex_effbot             | 3.58 ms                                                                      | 3.59 ms: 1.00x slower                                                                  |
| sqlglot_parse            | 1.37 ms                                                                      | 1.38 ms: 1.00x slower                                                                  |
| python_startup           | 12.7 ms                                                                      | 12.7 ms: 1.00x slower                                                                  |
| richards                 | 50.8 ms                                                                      | 51.0 ms: 1.01x slower                                                                  |
| regex_compile            | 146 ms                                                                       | 147 ms: 1.01x slower                                                                   |
| docutils                 | 2.89 sec                                                                     | 2.90 sec: 1.01x slower                                                                 |
| json_dumps               | 10.6 ms                                                                      | 10.7 ms: 1.01x slower                                                                  |
| sqlglot_normalize        | 120 ms                                                                       | 121 ms: 1.01x slower                                                                   |
| python_startup_no_site   | 11.1 ms                                                                      | 11.2 ms: 1.01x slower                                                                  |
| xml_etree_iterparse      | 106 ms                                                                       | 107 ms: 1.01x slower                                                                   |
| float                    | 81.6 ms                                                                      | 82.1 ms: 1.01x slower                                                                  |
| meteor_contest           | 133 ms                                                                       | 134 ms: 1.01x slower                                                                   |
| tomli_loads              | 2.32 sec                                                                     | 2.34 sec: 1.01x slower                                                                 |
| scimark_monte_carlo      | 78.3 ms                                                                      | 79.0 ms: 1.01x slower                                                                  |
| 2to3                     | 300 ms                                                                       | 303 ms: 1.01x slower                                                                   |
| sympy_expand             | 504 ms                                                                       | 509 ms: 1.01x slower                                                                   |
| crypto_pyaes             | 81.4 ms                                                                      | 82.1 ms: 1.01x slower                                                                  |
| sympy_integrate          | 24.2 ms                                                                      | 24.5 ms: 1.01x slower                                                                  |
| sqlglot_optimize         | 61.4 ms                                                                      | 62.1 ms: 1.01x slower                                                                  |
| json_loads               | 25.1 us                                                                      | 25.3 us: 1.01x slower                                                                  |
| richards_super           | 56.7 ms                                                                      | 57.4 ms: 1.01x slower                                                                  |
| generators               | 34.0 ms                                                                      | 34.4 ms: 1.01x slower                                                                  |
| regex_v8                 | 25.3 ms                                                                      | 25.6 ms: 1.01x slower                                                                  |
| sympy_sum                | 160 ms                                                                       | 163 ms: 1.02x slower                                                                   |
| sympy_str                | 299 ms                                                                       | 304 ms: 1.02x slower                                                                   |
| pickle                   | 10.3 us                                                                      | 10.4 us: 1.02x slower                                                                  |
| tornado_http             | 124 ms                                                                       | 126 ms: 1.02x slower                                                                   |
| logging_simple           | 6.51 us                                                                      | 6.65 us: 1.02x slower                                                                  |
| regex_dna                | 236 ms                                                                       | 241 ms: 1.02x slower                                                                   |
| logging_format           | 7.27 us                                                                      | 7.46 us: 1.03x slower                                                                  |
| pickle_list              | 4.25 us                                                                      | 4.37 us: 1.03x slower                                                                  |
| unpack_sequence          | 42.5 ns                                                                      | 43.7 ns: 1.03x slower                                                                  |
| hexiom                   | 7.79 ms                                                                      | 8.04 ms: 1.03x slower                                                                  |
| fannkuch                 | 415 ms                                                                       | 430 ms: 1.04x slower                                                                   |
| dulwich_log              | 67.9 ms                                                                      | 70.4 ms: 1.04x slower                                                                  |
| Geometric mean           | (ref)                                                                        | 1.00x faster                                                                           |

Benchmark hidden because not significant (30): spectral_norm, nqueens, async_tree_memoization_tg, bench_thread_pool, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none, raytrace, sqlglot_transpile, async_generators, asyncio_tcp, pickle_pure_python, telco, create_gc_cycles, pickle_dict, async_tree_io_tg, pprint_safe_repr, asyncio_tcp_ssl, async_tree_io, sqlite_synth, pprint_pformat, scimark_sor, comprehensions, scimark_lu, mypy2, coroutines, json, xml_etree_parse, dask


# HPT report

- Reliability score: 83.71% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x