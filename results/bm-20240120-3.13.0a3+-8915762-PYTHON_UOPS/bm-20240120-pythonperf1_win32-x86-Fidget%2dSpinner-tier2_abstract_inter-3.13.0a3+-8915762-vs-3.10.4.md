
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: 8915762
- commit date: 2024-01-20
- overall geometric mean: 1.14x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 252 ms: 1.05x faster                                                                      |
| chameleon      | 6.42 ms                                                         | 5.67 ms: 1.13x faster                                                                     |
| docutils       | 1.95 sec                                                        | 1.83 sec: 1.07x faster                                                                    |
| tornado_http   | 118 ms                                                          | 101 ms: 1.17x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 505 ms: 1.83x faster                                                                      |
| async_tree_none         | 394 ms                                                          | 249 ms: 1.58x faster                                                                      |
| async_tree_io           | 940 ms                                                          | 600 ms: 1.57x faster                                                                      |
| async_tree_memoization  | 467 ms                                                          | 310 ms: 1.51x faster                                                                      |
| Geometric mean          | (ref)                                                           | 1.62x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                                      |
| float          | 69.6 ms                                                         | 56.2 ms: 1.24x faster                                                                     |
| nbody          | 79.1 ms                                                         | 85.9 ms: 1.09x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.43x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 117 ms: 1.12x faster                                                                      |
| regex_compile  | 117 ms                                                          | 107 ms: 1.09x faster                                                                      |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.01x slower                                                                     |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.02x faster                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.64 ms: 1.48x faster                                                                     |
| pickle_pure_python   | 280 us                                                          | 209 us: 1.34x faster                                                                      |
| unpickle_pure_python | 189 us                                                          | 149 us: 1.27x faster                                                                      |
| tomli_loads          | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                                    |
| xml_etree_process    | 48.1 ms                                                         | 41.9 ms: 1.15x faster                                                                     |
| json_loads           | 22.4 us                                                         | 19.9 us: 1.13x faster                                                                     |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                                      |
| unpickle_list        | 2.98 us                                                         | 2.83 us: 1.05x faster                                                                     |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.1 ms: 1.04x faster                                                                     |
| xml_etree_generate   | 61.6 ms                                                         | 59.8 ms: 1.03x faster                                                                     |
| unpickle             | 9.82 us                                                         | 9.55 us: 1.03x faster                                                                     |
| pickle_list          | 3.22 us                                                         | 3.25 us: 1.01x slower                                                                     |
| pickle_dict          | 18.2 us                                                         | 20.2 us: 1.11x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                              |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.7 ms: 1.01x faster                                                                     |
| python_startup_no_site | 18.1 ms                                                         | 20.6 ms: 1.14x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.74 ms: 1.18x faster                                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 92.3 us: 4.29x faster                                                                     |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                                      |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 505 ms: 1.83x faster                                                                      |
| logging_silent           | 97.9 ns                                                         | 60.4 ns: 1.62x faster                                                                     |
| async_tree_none          | 394 ms                                                          | 249 ms: 1.58x faster                                                                      |
| async_tree_io            | 940 ms                                                          | 600 ms: 1.57x faster                                                                      |
| deltablue                | 4.04 ms                                                         | 2.67 ms: 1.51x faster                                                                     |
| async_tree_memoization   | 467 ms                                                          | 310 ms: 1.51x faster                                                                      |
| richards_super           | 49.9 ms                                                         | 33.3 ms: 1.50x faster                                                                     |
| json_dumps               | 9.82 ms                                                         | 6.64 ms: 1.48x faster                                                                     |
| crypto_pyaes             | 81.3 ms                                                         | 55.7 ms: 1.46x faster                                                                     |
| sqlglot_parse            | 1.33 ms                                                         | 913 us: 1.46x faster                                                                      |
| scimark_lu               | 89.8 ms                                                         | 62.0 ms: 1.45x faster                                                                     |
| raytrace                 | 303 ms                                                          | 211 ms: 1.44x faster                                                                      |
| chaos                    | 74.4 ms                                                         | 52.5 ms: 1.42x faster                                                                     |
| scimark_sor              | 115 ms                                                          | 82.1 ms: 1.40x faster                                                                     |
| go                       | 146 ms                                                          | 105 ms: 1.38x faster                                                                      |
| richards                 | 40.3 ms                                                         | 29.6 ms: 1.36x faster                                                                     |
| sqlglot_transpile        | 1.58 ms                                                         | 1.17 ms: 1.36x faster                                                                     |
| pickle_pure_python       | 280 us                                                          | 209 us: 1.34x faster                                                                      |
| comprehensions           | 17.7 us                                                         | 13.5 us: 1.31x faster                                                                     |
| generators               | 31.6 ms                                                         | 24.0 ms: 1.31x faster                                                                     |
| unpickle_pure_python     | 189 us                                                          | 149 us: 1.27x faster                                                                      |
| pyflate                  | 422 ms                                                          | 333 ms: 1.27x faster                                                                      |
| scimark_monte_carlo      | 61.9 ms                                                         | 49.6 ms: 1.25x faster                                                                     |
| pycparser                | 1.04 sec                                                        | 837 ms: 1.25x faster                                                                      |
| float                    | 69.6 ms                                                         | 56.2 ms: 1.24x faster                                                                     |
| sqlite_synth             | 2.29 us                                                         | 1.86 us: 1.23x faster                                                                     |
| coroutines               | 17.9 ms                                                         | 14.7 ms: 1.22x faster                                                                     |
| deepcopy_memo            | 29.6 us                                                         | 25.1 us: 1.18x faster                                                                     |
| tomli_loads              | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                                    |
| mako                     | 9.10 ms                                                         | 7.74 ms: 1.18x faster                                                                     |
| hexiom                   | 6.13 ms                                                         | 5.21 ms: 1.18x faster                                                                     |
| asyncio_tcp              | 744 ms                                                          | 634 ms: 1.17x faster                                                                      |
| tornado_http             | 118 ms                                                          | 101 ms: 1.17x faster                                                                      |
| json                     | 4.76 ms                                                         | 4.10 ms: 1.16x faster                                                                     |
| xml_etree_process        | 48.1 ms                                                         | 41.9 ms: 1.15x faster                                                                     |
| chameleon                | 6.42 ms                                                         | 5.67 ms: 1.13x faster                                                                     |
| json_loads               | 22.4 us                                                         | 19.9 us: 1.13x faster                                                                     |
| sympy_sum                | 122 ms                                                          | 109 ms: 1.12x faster                                                                      |
| nqueens                  | 87.1 ms                                                         | 77.8 ms: 1.12x faster                                                                     |
| regex_dna                | 131 ms                                                          | 117 ms: 1.12x faster                                                                      |
| dask                     | 341 ms                                                          | 307 ms: 1.11x faster                                                                      |
| deepcopy                 | 310 us                                                          | 279 us: 1.11x faster                                                                      |
| pprint_pformat           | 1.37 sec                                                        | 1.24 sec: 1.11x faster                                                                    |
| fannkuch                 | 317 ms                                                          | 288 ms: 1.10x faster                                                                      |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                                      |
| pprint_safe_repr         | 658 ms                                                          | 599 ms: 1.10x faster                                                                      |
| regex_compile            | 117 ms                                                          | 107 ms: 1.09x faster                                                                      |
| bench_thread_pool        | 1.12 ms                                                         | 1.03 ms: 1.09x faster                                                                     |
| sympy_integrate          | 16.6 ms                                                         | 15.4 ms: 1.08x faster                                                                     |
| create_gc_cycles         | 694 us                                                          | 642 us: 1.08x faster                                                                      |
| deepcopy_reduce          | 2.68 us                                                         | 2.49 us: 1.08x faster                                                                     |
| sympy_str                | 229 ms                                                          | 213 ms: 1.07x faster                                                                      |
| mdp                      | 1.83 sec                                                        | 1.71 sec: 1.07x faster                                                                    |
| sqlglot_optimize         | 44.7 ms                                                         | 41.8 ms: 1.07x faster                                                                     |
| docutils                 | 1.95 sec                                                        | 1.83 sec: 1.07x faster                                                                    |
| sqlglot_normalize        | 230 ms                                                          | 216 ms: 1.06x faster                                                                      |
| 2to3                     | 265 ms                                                          | 252 ms: 1.05x faster                                                                      |
| unpickle_list            | 2.98 us                                                         | 2.83 us: 1.05x faster                                                                     |
| scimark_fft              | 216 ms                                                          | 207 ms: 1.05x faster                                                                      |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.1 ms: 1.04x faster                                                                     |
| sympy_expand             | 391 ms                                                          | 376 ms: 1.04x faster                                                                      |
| xml_etree_generate       | 61.6 ms                                                         | 59.8 ms: 1.03x faster                                                                     |
| unpickle                 | 9.82 us                                                         | 9.55 us: 1.03x faster                                                                     |
| meteor_contest           | 80.0 ms                                                         | 78.1 ms: 1.02x faster                                                                     |
| python_startup           | 22.9 ms                                                         | 22.7 ms: 1.01x faster                                                                     |
| spectral_norm            | 80.2 ms                                                         | 79.8 ms: 1.01x faster                                                                     |
| pickle_list              | 3.22 us                                                         | 3.25 us: 1.01x slower                                                                     |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.01x slower                                                                     |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.28 ms: 1.01x slower                                                                     |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.4 sec: 1.03x slower                                                                    |
| unpack_sequence          | 40.0 ns                                                         | 41.6 ns: 1.04x slower                                                                     |
| pathlib                  | 81.2 ms                                                         | 88.1 ms: 1.08x slower                                                                     |
| nbody                    | 79.1 ms                                                         | 85.9 ms: 1.09x slower                                                                     |
| gc_traversal             | 1.28 ms                                                         | 1.41 ms: 1.10x slower                                                                     |
| logging_format           | 7.91 us                                                         | 8.71 us: 1.10x slower                                                                     |
| logging_simple           | 7.29 us                                                         | 8.06 us: 1.11x slower                                                                     |
| pickle_dict              | 18.2 us                                                         | 20.2 us: 1.11x slower                                                                     |
| async_generators         | 241 ms                                                          | 270 ms: 1.12x slower                                                                      |
| bench_mp_pool            | 66.4 ms                                                         | 74.9 ms: 1.13x slower                                                                     |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                                     |
| python_startup_no_site   | 18.1 ms                                                         | 20.6 ms: 1.14x slower                                                                     |
| telco                    | 4.83 ms                                                         | 6.14 ms: 1.27x slower                                                                     |
| coverage                 | 46.6 ms                                                         | 487 ms: 10.47x slower                                                                     |
| Geometric mean           | (ref)                                                           | 1.14x faster                                                                              |

Benchmark hidden because not significant (1): pickle
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-8915762-PYTHON_UOPS/bm-20240120-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown