
# Results vs. 3.10.4

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-x86
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.17x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 241 ms: 1.10x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.74 ms: 1.12x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.73 sec: 1.13x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.8 ms: 1.20x faster                                                           |
| Geometric mean | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 522 ms: 1.77x faster                                                            |
| async_tree_none         | 394 ms                                                          | 257 ms: 1.53x faster                                                            |
| async_tree_io           | 940 ms                                                          | 627 ms: 1.50x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 324 ms: 1.44x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.55x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 199 ms: 2.53x faster                                                            |
| float          | 69.6 ms                                                         | 54.5 ms: 1.28x faster                                                           |
| nbody          | 79.1 ms                                                         | 74.8 ms: 1.06x faster                                                           |
| Geometric mean | (ref)                                                           | 1.51x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 97.1 ms: 1.20x faster                                                           |
| regex_dna      | 131 ms                                                          | 123 ms: 1.06x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.01x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.94 ms: 1.17x slower                                                           |
| Geometric mean | (ref)                                                           | 1.02x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.71 ms: 1.46x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 198 us: 1.42x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 140 us: 1.36x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 40.9 ms: 1.18x faster                                                           |
| json_loads           | 22.4 us                                                         | 20.4 us: 1.10x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 112 ms: 1.07x faster                                                            |
| xml_etree_generate   | 61.6 ms                                                         | 59.0 ms: 1.05x faster                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.3 ms: 1.04x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.25 us: 1.01x slower                                                           |
| unpickle             | 9.82 us                                                         | 10.0 us: 1.02x slower                                                           |
| unpickle_list        | 2.98 us                                                         | 3.05 us: 1.02x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.0 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.9 ms: 1.04x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 21.5 ms: 1.19x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.11x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.12 ms: 1.28x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 89.6 us: 4.42x faster                                                           |
| pidigits                 | 502 ms                                                          | 199 ms: 2.53x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 522 ms: 1.77x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.34 ms: 1.72x faster                                                           |
| logging_silent           | 97.9 ns                                                         | 58.4 ns: 1.67x faster                                                           |
| comprehensions           | 17.7 us                                                         | 11.3 us: 1.57x faster                                                           |
| async_tree_none          | 394 ms                                                          | 257 ms: 1.53x faster                                                            |
| chaos                    | 74.4 ms                                                         | 48.9 ms: 1.52x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 53.9 ms: 1.51x faster                                                           |
| async_tree_io            | 940 ms                                                          | 627 ms: 1.50x faster                                                            |
| scimark_lu               | 89.8 ms                                                         | 59.9 ms: 1.50x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 4.17 ms: 1.47x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.71 ms: 1.46x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 324 ms: 1.44x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 923 us: 1.44x faster                                                            |
| raytrace                 | 303 ms                                                          | 212 ms: 1.43x faster                                                            |
| go                       | 146 ms                                                          | 103 ms: 1.42x faster                                                            |
| richards_super           | 49.9 ms                                                         | 35.1 ms: 1.42x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 198 us: 1.42x faster                                                            |
| generators               | 31.6 ms                                                         | 22.6 ms: 1.39x faster                                                           |
| scimark_sor              | 115 ms                                                          | 82.6 ms: 1.39x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.16 ms: 1.36x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 140 us: 1.36x faster                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 46.0 ms: 1.35x faster                                                           |
| pyflate                  | 422 ms                                                          | 319 ms: 1.32x faster                                                            |
| pycparser                | 1.04 sec                                                        | 791 ms: 1.32x faster                                                            |
| richards                 | 40.3 ms                                                         | 30.8 ms: 1.30x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.12 ms: 1.28x faster                                                           |
| float                    | 69.6 ms                                                         | 54.5 ms: 1.28x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 23.3 us: 1.27x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.82 us: 1.26x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 70.7 ms: 1.23x faster                                                           |
| tornado_http             | 118 ms                                                          | 97.8 ms: 1.20x faster                                                           |
| sympy_sum                | 122 ms                                                          | 102 ms: 1.20x faster                                                            |
| coroutines               | 17.9 ms                                                         | 14.9 ms: 1.20x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.23 us: 1.20x faster                                                           |
| regex_compile            | 117 ms                                                          | 97.1 ms: 1.20x faster                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.15 sec: 1.19x faster                                                          |
| fannkuch                 | 317 ms                                                          | 269 ms: 1.18x faster                                                            |
| tomli_loads              | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                          |
| deepcopy                 | 310 us                                                          | 263 us: 1.18x faster                                                            |
| spectral_norm            | 80.2 ms                                                         | 68.1 ms: 1.18x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 40.9 ms: 1.18x faster                                                           |
| json                     | 4.76 ms                                                         | 4.08 ms: 1.17x faster                                                           |
| sympy_str                | 229 ms                                                          | 197 ms: 1.16x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 14.3 ms: 1.16x faster                                                           |
| pprint_safe_repr         | 658 ms                                                          | 569 ms: 1.16x faster                                                            |
| sympy_expand             | 391 ms                                                          | 344 ms: 1.13x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.61 sec: 1.13x faster                                                          |
| docutils                 | 1.95 sec                                                        | 1.73 sec: 1.13x faster                                                          |
| dask                     | 341 ms                                                          | 304 ms: 1.12x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 205 ms: 1.12x faster                                                            |
| unpack_sequence          | 40.0 ns                                                         | 35.7 ns: 1.12x faster                                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 39.9 ms: 1.12x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.74 ms: 1.12x faster                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 2.90 ms: 1.12x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 671 ms: 1.11x faster                                                            |
| 2to3                     | 265 ms                                                          | 241 ms: 1.10x faster                                                            |
| json_loads               | 22.4 us                                                         | 20.4 us: 1.10x faster                                                           |
| scimark_fft              | 216 ms                                                          | 197 ms: 1.10x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.03 ms: 1.09x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 112 ms: 1.07x faster                                                            |
| regex_dna                | 131 ms                                                          | 123 ms: 1.06x faster                                                            |
| nbody                    | 79.1 ms                                                         | 74.8 ms: 1.06x faster                                                           |
| meteor_contest           | 80.0 ms                                                         | 75.7 ms: 1.06x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 657 us: 1.06x faster                                                            |
| xml_etree_generate       | 61.6 ms                                                         | 59.0 ms: 1.05x faster                                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.3 ms: 1.04x faster                                                           |
| pickle_list              | 3.22 us                                                         | 3.25 us: 1.01x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.01x slower                                                           |
| unpickle                 | 9.82 us                                                         | 10.0 us: 1.02x slower                                                           |
| unpickle_list            | 2.98 us                                                         | 3.05 us: 1.02x slower                                                           |
| python_startup           | 22.9 ms                                                         | 23.9 ms: 1.04x slower                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| logging_format           | 7.91 us                                                         | 8.43 us: 1.07x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.88 us: 1.08x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 88.8 ms: 1.09x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.0 us: 1.10x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.42 ms: 1.11x slower                                                           |
| async_generators         | 241 ms                                                          | 269 ms: 1.12x slower                                                            |
| bench_mp_pool            | 66.4 ms                                                         | 75.4 ms: 1.14x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.94 ms: 1.17x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 21.5 ms: 1.19x slower                                                           |
| telco                    | 4.83 ms                                                         | 5.97 ms: 1.24x slower                                                           |
| coverage                 | 46.6 ms                                                         | 484 ms: 10.39x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.17x faster                                                                    |

Benchmark hidden because not significant (1): pickle
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown