
# Results vs. 3.10.4

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-x86
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 247 ms: 1.08x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.87 ms: 1.09x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.80 sec: 1.08x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.9 ms: 1.20x faster                                                           |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 506 ms: 1.82x faster                                                            |
| async_tree_none         | 394 ms                                                          | 255 ms: 1.54x faster                                                            |
| async_tree_io           | 940 ms                                                          | 623 ms: 1.51x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 319 ms: 1.47x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.58x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| float          | 69.6 ms                                                         | 58.8 ms: 1.18x faster                                                           |
| nbody          | 79.1 ms                                                         | 84.7 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.41x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 106 ms: 1.10x faster                                                            |
| regex_dna      | 131 ms                                                          | 123 ms: 1.06x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.5 ms: 1.05x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.92 ms: 1.15x slower                                                           |
| Geometric mean | (ref)                                                           | 1.01x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.89 ms: 1.43x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 214 us: 1.31x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 152 us: 1.24x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.63 sec: 1.17x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 41.7 ms: 1.16x faster                                                           |
| json_loads           | 22.4 us                                                         | 20.1 us: 1.12x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.5 ms: 1.03x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 61.2 ms: 1.01x faster                                                           |
| pickle               | 7.83 us                                                         | 7.97 us: 1.02x slower                                                           |
| pickle_list          | 3.22 us                                                         | 3.28 us: 1.02x slower                                                           |
| unpickle_list        | 2.98 us                                                         | 3.15 us: 1.06x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                    |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.4 ms: 1.02x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.6 ms: 1.14x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.70 ms: 1.18x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 96.1 us: 4.12x faster                                                           |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 506 ms: 1.82x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 60.4 ns: 1.62x faster                                                           |
| async_tree_none          | 394 ms                                                          | 255 ms: 1.54x faster                                                            |
| richards_super           | 49.9 ms                                                         | 32.5 ms: 1.53x faster                                                           |
| deltablue                | 4.04 ms                                                         | 2.66 ms: 1.52x faster                                                           |
| async_tree_io            | 940 ms                                                          | 623 ms: 1.51x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 904 us: 1.47x faster                                                            |
| async_tree_memoization   | 467 ms                                                          | 319 ms: 1.47x faster                                                            |
| raytrace                 | 303 ms                                                          | 211 ms: 1.43x faster                                                            |
| json_dumps               | 9.82 ms                                                         | 6.89 ms: 1.43x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 57.1 ms: 1.42x faster                                                           |
| chaos                    | 74.4 ms                                                         | 52.3 ms: 1.42x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 64.0 ms: 1.40x faster                                                           |
| richards                 | 40.3 ms                                                         | 29.4 ms: 1.37x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.16 ms: 1.37x faster                                                           |
| generators               | 31.6 ms                                                         | 23.1 ms: 1.36x faster                                                           |
| comprehensions           | 17.7 us                                                         | 13.0 us: 1.36x faster                                                           |
| go                       | 146 ms                                                          | 107 ms: 1.36x faster                                                            |
| scimark_sor              | 115 ms                                                          | 84.9 ms: 1.35x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 214 us: 1.31x faster                                                            |
| pyflate                  | 422 ms                                                          | 337 ms: 1.25x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 152 us: 1.24x faster                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 50.3 ms: 1.23x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.88 us: 1.22x faster                                                           |
| pycparser                | 1.04 sec                                                        | 858 ms: 1.21x faster                                                            |
| coroutines               | 17.9 ms                                                         | 14.9 ms: 1.20x faster                                                           |
| tornado_http             | 118 ms                                                          | 97.9 ms: 1.20x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 24.8 us: 1.19x faster                                                           |
| float                    | 69.6 ms                                                         | 58.8 ms: 1.18x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.70 ms: 1.18x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 5.21 ms: 1.18x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.63 sec: 1.17x faster                                                          |
| xml_etree_process        | 48.1 ms                                                         | 41.7 ms: 1.16x faster                                                           |
| deepcopy                 | 310 us                                                          | 269 us: 1.15x faster                                                            |
| sympy_sum                | 122 ms                                                          | 108 ms: 1.13x faster                                                            |
| json                     | 4.76 ms                                                         | 4.22 ms: 1.13x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 660 ms: 1.13x faster                                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.22 sec: 1.12x faster                                                          |
| json_loads               | 22.4 us                                                         | 20.1 us: 1.12x faster                                                           |
| dask                     | 341 ms                                                          | 308 ms: 1.11x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| regex_compile            | 117 ms                                                          | 106 ms: 1.10x faster                                                            |
| chameleon                | 6.42 ms                                                         | 5.87 ms: 1.09x faster                                                           |
| pprint_safe_repr         | 658 ms                                                          | 604 ms: 1.09x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.68 sec: 1.09x faster                                                          |
| sqlglot_normalize        | 230 ms                                                          | 212 ms: 1.09x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.80 sec: 1.08x faster                                                          |
| sympy_str                | 229 ms                                                          | 213 ms: 1.08x faster                                                            |
| 2to3                     | 265 ms                                                          | 247 ms: 1.08x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 41.7 ms: 1.07x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.51 us: 1.07x faster                                                           |
| sympy_integrate          | 16.6 ms                                                         | 15.6 ms: 1.07x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 81.8 ms: 1.07x faster                                                           |
| sympy_expand             | 391 ms                                                          | 367 ms: 1.06x faster                                                            |
| fannkuch                 | 317 ms                                                          | 299 ms: 1.06x faster                                                            |
| create_gc_cycles         | 694 us                                                          | 655 us: 1.06x faster                                                            |
| regex_dna                | 131 ms                                                          | 123 ms: 1.06x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.08 ms: 1.04x faster                                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.5 ms: 1.03x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 61.2 ms: 1.01x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 79.7 ms: 1.01x faster                                                           |
| pickle                   | 7.83 us                                                         | 7.97 us: 1.02x slower                                                           |
| pickle_list              | 3.22 us                                                         | 3.28 us: 1.02x slower                                                           |
| python_startup           | 22.9 ms                                                         | 23.4 ms: 1.02x slower                                                           |
| scimark_fft              | 216 ms                                                          | 225 ms: 1.04x slower                                                            |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| regex_v8                 | 15.8 ms                                                         | 16.5 ms: 1.05x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 42.0 ns: 1.05x slower                                                           |
| unpickle_list            | 2.98 us                                                         | 3.15 us: 1.06x slower                                                           |
| nbody                    | 79.1 ms                                                         | 84.7 ms: 1.07x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.39 ms: 1.09x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 89.2 ms: 1.10x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 73.1 ms: 1.10x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.75 us: 1.11x slower                                                           |
| logging_simple           | 7.29 us                                                         | 8.24 us: 1.13x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.6 ms: 1.14x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.92 ms: 1.15x slower                                                           |
| async_generators         | 241 ms                                                          | 279 ms: 1.16x slower                                                            |
| telco                    | 4.83 ms                                                         | 5.92 ms: 1.23x slower                                                           |
| coverage                 | 46.6 ms                                                         | 489 ms: 10.50x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (3): meteor_contest, unpickle, scimark_sparse_mat_mult
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1_win32-x86-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown