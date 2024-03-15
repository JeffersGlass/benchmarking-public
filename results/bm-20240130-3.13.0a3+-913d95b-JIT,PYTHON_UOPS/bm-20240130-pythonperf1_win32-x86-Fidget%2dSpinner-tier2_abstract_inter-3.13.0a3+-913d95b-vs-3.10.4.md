
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.08x faster
- HPT reliability: 99.73%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 268 ms: 1.01x slower                                                                      |
| chameleon      | 6.42 ms                                                         | 6.17 ms: 1.04x faster                                                                     |
| docutils       | 1.95 sec                                                        | 1.86 sec: 1.05x faster                                                                    |
| tornado_http   | 118 ms                                                          | 103 ms: 1.15x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.06x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 527 ms: 1.75x faster                                                                      |
| async_tree_none         | 394 ms                                                          | 264 ms: 1.49x faster                                                                      |
| async_tree_io           | 940 ms                                                          | 634 ms: 1.48x faster                                                                      |
| async_tree_memoization  | 467 ms                                                          | 330 ms: 1.41x faster                                                                      |
| Geometric mean          | (ref)                                                           | 1.53x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 201 ms: 2.50x faster                                                                      |
| float          | 69.6 ms                                                         | 55.7 ms: 1.25x faster                                                                     |
| nbody          | 79.1 ms                                                         | 90.8 ms: 1.15x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.40x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 122 ms: 1.07x faster                                                                      |
| regex_compile  | 117 ms                                                          | 113 ms: 1.03x faster                                                                      |
| regex_v8       | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                                     |
| regex_effbot   | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.02x slower                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 7.14 ms: 1.38x faster                                                                     |
| pickle_pure_python   | 280 us                                                          | 227 us: 1.23x faster                                                                      |
| unpickle_pure_python | 189 us                                                          | 157 us: 1.20x faster                                                                      |
| tomli_loads          | 1.91 sec                                                        | 1.64 sec: 1.16x faster                                                                    |
| xml_etree_parse      | 120 ms                                                          | 104 ms: 1.15x faster                                                                      |
| xml_etree_process    | 48.1 ms                                                         | 42.8 ms: 1.12x faster                                                                     |
| json_loads           | 22.4 us                                                         | 20.1 us: 1.11x faster                                                                     |
| unpickle_list        | 2.98 us                                                         | 2.79 us: 1.07x faster                                                                     |
| xml_etree_iterparse  | 70.8 ms                                                         | 67.2 ms: 1.05x faster                                                                     |
| xml_etree_generate   | 61.6 ms                                                         | 62.3 ms: 1.01x slower                                                                     |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.02x slower                                                                     |
| pickle               | 7.83 us                                                         | 8.07 us: 1.03x slower                                                                     |
| pickle_list          | 3.22 us                                                         | 3.31 us: 1.03x slower                                                                     |
| pickle_dict          | 18.2 us                                                         | 20.5 us: 1.12x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.08x faster                                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.6 ms: 1.03x slower                                                                     |
| python_startup_no_site | 18.1 ms                                                         | 21.1 ms: 1.17x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.10x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 8.01 ms: 1.14x faster                                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 97.9 us: 4.04x faster                                                                     |
| pidigits                 | 502 ms                                                          | 201 ms: 2.50x faster                                                                      |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 527 ms: 1.75x faster                                                                      |
| deltablue                | 4.04 ms                                                         | 2.62 ms: 1.54x faster                                                                     |
| async_tree_none          | 394 ms                                                          | 264 ms: 1.49x faster                                                                      |
| async_tree_io            | 940 ms                                                          | 634 ms: 1.48x faster                                                                      |
| logging_silent           | 97.9 ns                                                         | 66.3 ns: 1.48x faster                                                                     |
| async_tree_memoization   | 467 ms                                                          | 330 ms: 1.41x faster                                                                      |
| richards_super           | 49.9 ms                                                         | 35.3 ms: 1.41x faster                                                                     |
| sqlglot_parse            | 1.33 ms                                                         | 965 us: 1.38x faster                                                                      |
| json_dumps               | 9.82 ms                                                         | 7.14 ms: 1.38x faster                                                                     |
| scimark_lu               | 89.8 ms                                                         | 68.7 ms: 1.31x faster                                                                     |
| richards                 | 40.3 ms                                                         | 31.1 ms: 1.29x faster                                                                     |
| sqlglot_transpile        | 1.58 ms                                                         | 1.23 ms: 1.29x faster                                                                     |
| chaos                    | 74.4 ms                                                         | 58.0 ms: 1.28x faster                                                                     |
| generators               | 31.6 ms                                                         | 25.0 ms: 1.26x faster                                                                     |
| raytrace                 | 303 ms                                                          | 240 ms: 1.26x faster                                                                      |
| crypto_pyaes             | 81.3 ms                                                         | 64.7 ms: 1.26x faster                                                                     |
| float                    | 69.6 ms                                                         | 55.7 ms: 1.25x faster                                                                     |
| sqlite_synth             | 2.29 us                                                         | 1.86 us: 1.23x faster                                                                     |
| scimark_sor              | 115 ms                                                          | 93.2 ms: 1.23x faster                                                                     |
| pickle_pure_python       | 280 us                                                          | 227 us: 1.23x faster                                                                      |
| unpickle_pure_python     | 189 us                                                          | 157 us: 1.20x faster                                                                      |
| pycparser                | 1.04 sec                                                        | 869 ms: 1.20x faster                                                                      |
| asyncio_tcp              | 744 ms                                                          | 622 ms: 1.20x faster                                                                      |
| go                       | 146 ms                                                          | 122 ms: 1.19x faster                                                                      |
| coroutines               | 17.9 ms                                                         | 15.2 ms: 1.18x faster                                                                     |
| tomli_loads              | 1.91 sec                                                        | 1.64 sec: 1.16x faster                                                                    |
| xml_etree_parse          | 120 ms                                                          | 104 ms: 1.15x faster                                                                      |
| tornado_http             | 118 ms                                                          | 103 ms: 1.15x faster                                                                      |
| mako                     | 9.10 ms                                                         | 8.01 ms: 1.14x faster                                                                     |
| deepcopy_memo            | 29.6 us                                                         | 26.1 us: 1.14x faster                                                                     |
| xml_etree_process        | 48.1 ms                                                         | 42.8 ms: 1.12x faster                                                                     |
| comprehensions           | 17.7 us                                                         | 15.9 us: 1.11x faster                                                                     |
| json_loads               | 22.4 us                                                         | 20.1 us: 1.11x faster                                                                     |
| pyflate                  | 422 ms                                                          | 383 ms: 1.10x faster                                                                      |
| dask                     | 341 ms                                                          | 311 ms: 1.10x faster                                                                      |
| deepcopy_reduce          | 2.68 us                                                         | 2.45 us: 1.10x faster                                                                     |
| deepcopy                 | 310 us                                                          | 284 us: 1.09x faster                                                                      |
| regex_dna                | 131 ms                                                          | 122 ms: 1.07x faster                                                                      |
| unpickle_list            | 2.98 us                                                         | 2.79 us: 1.07x faster                                                                     |
| sympy_sum                | 122 ms                                                          | 116 ms: 1.06x faster                                                                      |
| xml_etree_iterparse      | 70.8 ms                                                         | 67.2 ms: 1.05x faster                                                                     |
| docutils                 | 1.95 sec                                                        | 1.86 sec: 1.05x faster                                                                    |
| bench_thread_pool        | 1.12 ms                                                         | 1.07 ms: 1.05x faster                                                                     |
| chameleon                | 6.42 ms                                                         | 6.17 ms: 1.04x faster                                                                     |
| create_gc_cycles         | 694 us                                                          | 668 us: 1.04x faster                                                                      |
| spectral_norm            | 80.2 ms                                                         | 77.4 ms: 1.04x faster                                                                     |
| sympy_str                | 229 ms                                                          | 221 ms: 1.04x faster                                                                      |
| regex_compile            | 117 ms                                                          | 113 ms: 1.03x faster                                                                      |
| sympy_expand             | 391 ms                                                          | 378 ms: 1.03x faster                                                                      |
| fannkuch                 | 317 ms                                                          | 310 ms: 1.02x faster                                                                      |
| sqlglot_normalize        | 230 ms                                                          | 227 ms: 1.02x faster                                                                      |
| sqlglot_optimize         | 44.7 ms                                                         | 44.3 ms: 1.01x faster                                                                     |
| 2to3                     | 265 ms                                                          | 268 ms: 1.01x slower                                                                      |
| xml_etree_generate       | 61.6 ms                                                         | 62.3 ms: 1.01x slower                                                                     |
| mdp                      | 1.83 sec                                                        | 1.87 sec: 1.02x slower                                                                    |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.02x slower                                                                     |
| python_startup           | 22.9 ms                                                         | 23.6 ms: 1.03x slower                                                                     |
| nqueens                  | 87.1 ms                                                         | 89.6 ms: 1.03x slower                                                                     |
| regex_v8                 | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                                     |
| pickle                   | 7.83 us                                                         | 8.07 us: 1.03x slower                                                                     |
| pickle_list              | 3.22 us                                                         | 3.31 us: 1.03x slower                                                                     |
| sympy_integrate          | 16.6 ms                                                         | 17.2 ms: 1.03x slower                                                                     |
| unpack_sequence          | 40.0 ns                                                         | 41.9 ns: 1.05x slower                                                                     |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.8 sec: 1.05x slower                                                                    |
| pprint_pformat           | 1.37 sec                                                        | 1.46 sec: 1.07x slower                                                                    |
| pprint_safe_repr         | 658 ms                                                          | 711 ms: 1.08x slower                                                                      |
| pathlib                  | 81.2 ms                                                         | 89.2 ms: 1.10x slower                                                                     |
| gc_traversal             | 1.28 ms                                                         | 1.41 ms: 1.10x slower                                                                     |
| meteor_contest           | 80.0 ms                                                         | 88.3 ms: 1.10x slower                                                                     |
| pickle_dict              | 18.2 us                                                         | 20.5 us: 1.12x slower                                                                     |
| scimark_monte_carlo      | 61.9 ms                                                         | 70.3 ms: 1.13x slower                                                                     |
| logging_format           | 7.91 us                                                         | 9.01 us: 1.14x slower                                                                     |
| regex_effbot             | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                                     |
| nbody                    | 79.1 ms                                                         | 90.8 ms: 1.15x slower                                                                     |
| logging_simple           | 7.29 us                                                         | 8.37 us: 1.15x slower                                                                     |
| bench_mp_pool            | 66.4 ms                                                         | 76.3 ms: 1.15x slower                                                                     |
| hexiom                   | 6.13 ms                                                         | 7.09 ms: 1.16x slower                                                                     |
| python_startup_no_site   | 18.1 ms                                                         | 21.1 ms: 1.17x slower                                                                     |
| scimark_fft              | 216 ms                                                          | 257 ms: 1.19x slower                                                                      |
| async_generators         | 241 ms                                                          | 303 ms: 1.26x slower                                                                      |
| telco                    | 4.83 ms                                                         | 6.44 ms: 1.33x slower                                                                     |
| coverage                 | 46.6 ms                                                         | 483 ms: 10.38x slower                                                                     |
| Geometric mean           | (ref)                                                           | 1.08x faster                                                                              |

Benchmark hidden because not significant (2): json, scimark_sparse_mat_mult
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240130-3.13.0a3+-913d95b-JIT,PYTHON_UOPS/bm-20240130-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.73% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown