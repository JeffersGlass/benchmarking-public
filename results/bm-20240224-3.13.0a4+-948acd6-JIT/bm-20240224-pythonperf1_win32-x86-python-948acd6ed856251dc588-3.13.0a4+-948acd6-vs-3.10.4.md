
# Results vs. 3.10.4

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.03x faster \*
- HPT reliability: 87.59%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 268 ms: 1.01x slower                                                            |
| chameleon      | 6.42 ms                                                         | 6.29 ms: 1.02x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.93 sec: 1.01x faster                                                          |
| tornado_http   | 118 ms                                                          | 99.6 ms: 1.18x faster                                                           |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 518 ms: 1.78x faster                                                            |
| async_tree_io           | 940 ms                                                          | 635 ms: 1.48x faster                                                            |
| async_tree_none         | 394 ms                                                          | 267 ms: 1.47x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 332 ms: 1.40x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.53x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 199 ms: 2.52x faster                                                            |
| float          | 69.6 ms                                                         | 55.3 ms: 1.26x faster                                                           |
| nbody          | 79.1 ms                                                         | 98.2 ms: 1.24x slower                                                           |
| Geometric mean | (ref)                                                           | 1.37x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 123 ms: 1.06x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.3 ms: 1.03x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| regex_compile  | 117 ms                                                          | 135 ms: 1.16x slower                                                            |
| Geometric mean | (ref)                                                           | 1.06x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 7.13 ms: 1.38x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 231 us: 1.21x faster                                                            |
| xml_etree_parse      | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 43.7 ms: 1.10x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.74 sec: 1.10x faster                                                          |
| json_loads           | 22.4 us                                                         | 20.7 us: 1.08x faster                                                           |
| unpickle_pure_python | 189 us                                                          | 178 us: 1.06x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 67.0 ms: 1.06x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.19 us: 1.01x faster                                                           |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.03x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 19.8 us: 1.08x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.07x faster                                                                    |

Benchmark hidden because not significant (3): unpickle_list, pickle, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 26.1 ms: 1.14x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 23.7 ms: 1.31x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.22x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.44 ms: 1.22x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 96.3 us: 4.11x faster                                                           |
| pidigits                 | 502 ms                                                          | 199 ms: 2.52x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 518 ms: 1.78x faster                                                            |
| async_tree_io            | 940 ms                                                          | 635 ms: 1.48x faster                                                            |
| async_tree_none          | 394 ms                                                          | 267 ms: 1.47x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.75 ms: 1.47x faster                                                           |
| logging_silent           | 97.9 ns                                                         | 67.6 ns: 1.45x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 332 ms: 1.40x faster                                                            |
| json_dumps               | 9.82 ms                                                         | 7.13 ms: 1.38x faster                                                           |
| generators               | 31.6 ms                                                         | 23.9 ms: 1.32x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 62.4 ms: 1.30x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 1.04 ms: 1.27x faster                                                           |
| float                    | 69.6 ms                                                         | 55.3 ms: 1.26x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.44 ms: 1.22x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 231 us: 1.21x faster                                                            |
| sqlglot_transpile        | 1.58 ms                                                         | 1.31 ms: 1.21x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.9 ms: 1.20x faster                                                           |
| chaos                    | 74.4 ms                                                         | 62.3 ms: 1.19x faster                                                           |
| tornado_http             | 118 ms                                                          | 99.6 ms: 1.18x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.96 us: 1.17x faster                                                           |
| pycparser                | 1.04 sec                                                        | 904 ms: 1.15x faster                                                            |
| asyncio_tcp              | 744 ms                                                          | 653 ms: 1.14x faster                                                            |
| json                     | 4.76 ms                                                         | 4.21 ms: 1.13x faster                                                           |
| richards_super           | 49.9 ms                                                         | 44.5 ms: 1.12x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| xml_etree_process        | 48.1 ms                                                         | 43.7 ms: 1.10x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.74 sec: 1.10x faster                                                          |
| deepcopy_memo            | 29.6 us                                                         | 27.0 us: 1.09x faster                                                           |
| comprehensions           | 17.7 us                                                         | 16.4 us: 1.09x faster                                                           |
| json_loads               | 22.4 us                                                         | 20.7 us: 1.08x faster                                                           |
| bench_thread_pool        | 1.12 ms                                                         | 1.03 ms: 1.08x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 649 us: 1.07x faster                                                            |
| spectral_norm            | 80.2 ms                                                         | 75.0 ms: 1.07x faster                                                           |
| raytrace                 | 303 ms                                                          | 283 ms: 1.07x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 178 us: 1.06x faster                                                            |
| regex_dna                | 131 ms                                                          | 123 ms: 1.06x faster                                                            |
| sympy_sum                | 122 ms                                                          | 116 ms: 1.06x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 67.0 ms: 1.06x faster                                                           |
| deepcopy                 | 310 us                                                          | 294 us: 1.05x faster                                                            |
| scimark_lu               | 89.8 ms                                                         | 86.0 ms: 1.04x faster                                                           |
| pyflate                  | 422 ms                                                          | 406 ms: 1.04x faster                                                            |
| go                       | 146 ms                                                          | 142 ms: 1.03x faster                                                            |
| chameleon                | 6.42 ms                                                         | 6.29 ms: 1.02x faster                                                           |
| docutils                 | 1.95 sec                                                        | 1.93 sec: 1.01x faster                                                          |
| pickle_list              | 3.22 us                                                         | 3.19 us: 1.01x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.67 us: 1.01x faster                                                           |
| 2to3                     | 265 ms                                                          | 268 ms: 1.01x slower                                                            |
| sympy_str                | 229 ms                                                          | 232 ms: 1.01x slower                                                            |
| richards                 | 40.3 ms                                                         | 40.8 ms: 1.01x slower                                                           |
| sympy_integrate          | 16.6 ms                                                         | 17.1 ms: 1.03x slower                                                           |
| sympy_expand             | 391 ms                                                          | 402 ms: 1.03x slower                                                            |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.03x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.3 ms: 1.03x slower                                                           |
| scimark_sor              | 115 ms                                                          | 120 ms: 1.04x slower                                                            |
| sqlglot_normalize        | 230 ms                                                          | 241 ms: 1.05x slower                                                            |
| pathlib                  | 81.2 ms                                                         | 85.0 ms: 1.05x slower                                                           |
| mdp                      | 1.83 sec                                                        | 1.92 sec: 1.05x slower                                                          |
| sqlglot_optimize         | 44.7 ms                                                         | 47.0 ms: 1.05x slower                                                           |
| fannkuch                 | 317 ms                                                          | 335 ms: 1.06x slower                                                            |
| nqueens                  | 87.1 ms                                                         | 93.7 ms: 1.08x slower                                                           |
| meteor_contest           | 80.0 ms                                                         | 86.6 ms: 1.08x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.39 ms: 1.08x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.8 us: 1.08x slower                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 67.5 ms: 1.09x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 74.8 ms: 1.13x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.56 sec: 1.14x slower                                                          |
| python_startup           | 22.9 ms                                                         | 26.1 ms: 1.14x slower                                                           |
| logging_format           | 7.91 us                                                         | 9.10 us: 1.15x slower                                                           |
| pprint_safe_repr         | 658 ms                                                          | 760 ms: 1.15x slower                                                            |
| regex_compile            | 117 ms                                                          | 135 ms: 1.16x slower                                                            |
| logging_simple           | 7.29 us                                                         | 8.50 us: 1.17x slower                                                           |
| scimark_fft              | 216 ms                                                          | 257 ms: 1.19x slower                                                            |
| nbody                    | 79.1 ms                                                         | 98.2 ms: 1.24x slower                                                           |
| telco                    | 4.83 ms                                                         | 6.21 ms: 1.28x slower                                                           |
| hexiom                   | 6.13 ms                                                         | 7.89 ms: 1.29x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 23.7 ms: 1.31x slower                                                           |
| async_generators         | 241 ms                                                          | 319 ms: 1.32x slower                                                            |
| unpack_sequence          | 40.0 ns                                                         | 85.7 ns: 2.14x slower                                                           |
| coverage                 | 46.6 ms                                                         | 496 ms: 10.65x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.03x faster                                                                    |

Benchmark hidden because not significant (5): unpickle_list, pickle, xml_etree_generate, scimark_sparse_mat_mult, asyncio_tcp_ssl
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 87.59% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown