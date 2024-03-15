
# Results vs. 3.10.4

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 229 ms: 1.16x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.63 ms: 1.14x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.69 sec: 1.15x faster                                                          |
| tornado_http   | 118 ms                                                          | 93.9 ms: 1.25x faster                                                           |
| Geometric mean | (ref)                                                           | 1.17x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 486 ms: 1.90x faster                                                            |
| async_tree_none         | 394 ms                                                          | 241 ms: 1.63x faster                                                            |
| async_tree_io           | 940 ms                                                          | 582 ms: 1.62x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 300 ms: 1.55x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.67x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| float          | 69.6 ms                                                         | 54.9 ms: 1.27x faster                                                           |
| nbody          | 79.1 ms                                                         | 76.1 ms: 1.04x faster                                                           |
| Geometric mean | (ref)                                                           | 1.50x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 94.6 ms: 1.23x faster                                                           |
| regex_dna      | 131 ms                                                          | 120 ms: 1.09x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 15.9 ms: 1.01x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.45 ms: 1.52x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 205 us: 1.37x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 143 us: 1.33x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 40.2 ms: 1.20x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                          |
| json_loads           | 22.4 us                                                         | 19.6 us: 1.14x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 64.8 ms: 1.09x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.78 us: 1.07x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 57.6 ms: 1.07x faster                                                           |
| unpickle             | 9.82 us                                                         | 9.96 us: 1.01x slower                                                           |
| pickle               | 7.83 us                                                         | 7.98 us: 1.02x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 19.9 us: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.4 ms: 1.02x faster                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.2 ms: 1.12x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 6.94 ms: 1.31x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 88.7 us: 4.46x faster                                                           |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 486 ms: 1.90x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.20 ms: 1.83x faster                                                           |
| logging_silent           | 97.9 ns                                                         | 58.5 ns: 1.67x faster                                                           |
| async_tree_none          | 394 ms                                                          | 241 ms: 1.63x faster                                                            |
| async_tree_io            | 940 ms                                                          | 582 ms: 1.62x faster                                                            |
| raytrace                 | 303 ms                                                          | 191 ms: 1.58x faster                                                            |
| chaos                    | 74.4 ms                                                         | 47.2 ms: 1.58x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 52.2 ms: 1.56x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 300 ms: 1.55x faster                                                            |
| comprehensions           | 17.7 us                                                         | 11.5 us: 1.55x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 58.7 ms: 1.53x faster                                                           |
| go                       | 146 ms                                                          | 95.3 ms: 1.53x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.45 ms: 1.52x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 876 us: 1.52x faster                                                            |
| richards_super           | 49.9 ms                                                         | 33.4 ms: 1.49x faster                                                           |
| generators               | 31.6 ms                                                         | 21.7 ms: 1.45x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.11 ms: 1.43x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 4.28 ms: 1.43x faster                                                           |
| richards                 | 40.3 ms                                                         | 28.6 ms: 1.41x faster                                                           |
| scimark_sor              | 115 ms                                                          | 83.8 ms: 1.37x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 205 us: 1.37x faster                                                            |
| pyflate                  | 422 ms                                                          | 309 ms: 1.37x faster                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 45.8 ms: 1.35x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 143 us: 1.33x faster                                                            |
| mako                     | 9.10 ms                                                         | 6.94 ms: 1.31x faster                                                           |
| pycparser                | 1.04 sec                                                        | 805 ms: 1.29x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 23.1 us: 1.28x faster                                                           |
| float                    | 69.6 ms                                                         | 54.9 ms: 1.27x faster                                                           |
| tornado_http             | 118 ms                                                          | 93.9 ms: 1.25x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.4 ms: 1.25x faster                                                           |
| regex_compile            | 117 ms                                                          | 94.6 ms: 1.23x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 65.4 ms: 1.23x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.87 us: 1.22x faster                                                           |
| sympy_sum                | 122 ms                                                          | 100 ms: 1.22x faster                                                            |
| nqueens                  | 87.1 ms                                                         | 71.7 ms: 1.22x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 40.2 ms: 1.20x faster                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.15 sec: 1.19x faster                                                          |
| sqlglot_normalize        | 230 ms                                                          | 194 ms: 1.19x faster                                                            |
| deepcopy                 | 310 us                                                          | 263 us: 1.18x faster                                                            |
| tomli_loads              | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                          |
| sqlglot_optimize         | 44.7 ms                                                         | 38.1 ms: 1.17x faster                                                           |
| dask                     | 341 ms                                                          | 291 ms: 1.17x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 14.2 ms: 1.17x faster                                                           |
| sympy_str                | 229 ms                                                          | 196 ms: 1.17x faster                                                            |
| pprint_safe_repr         | 658 ms                                                          | 565 ms: 1.16x faster                                                            |
| asyncio_tcp              | 744 ms                                                          | 639 ms: 1.16x faster                                                            |
| 2to3                     | 265 ms                                                          | 229 ms: 1.16x faster                                                            |
| json                     | 4.76 ms                                                         | 4.13 ms: 1.15x faster                                                           |
| docutils                 | 1.95 sec                                                        | 1.69 sec: 1.15x faster                                                          |
| fannkuch                 | 317 ms                                                          | 276 ms: 1.15x faster                                                            |
| json_loads               | 22.4 us                                                         | 19.6 us: 1.14x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.63 ms: 1.14x faster                                                           |
| bench_thread_pool        | 1.12 ms                                                         | 982 us: 1.14x faster                                                            |
| sympy_expand             | 391 ms                                                          | 343 ms: 1.14x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.37 us: 1.13x faster                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 2.87 ms: 1.13x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.65 sec: 1.11x faster                                                          |
| scimark_fft              | 216 ms                                                          | 197 ms: 1.10x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 64.8 ms: 1.09x faster                                                           |
| regex_dna                | 131 ms                                                          | 120 ms: 1.09x faster                                                            |
| create_gc_cycles         | 694 us                                                          | 641 us: 1.08x faster                                                            |
| unpickle_list            | 2.98 us                                                         | 2.78 us: 1.07x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 57.6 ms: 1.07x faster                                                           |
| meteor_contest           | 80.0 ms                                                         | 75.6 ms: 1.06x faster                                                           |
| nbody                    | 79.1 ms                                                         | 76.1 ms: 1.04x faster                                                           |
| unpack_sequence          | 40.0 ns                                                         | 39.0 ns: 1.03x faster                                                           |
| python_startup           | 22.9 ms                                                         | 22.4 ms: 1.02x faster                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| regex_v8                 | 15.8 ms                                                         | 15.9 ms: 1.01x slower                                                           |
| unpickle                 | 9.82 us                                                         | 9.96 us: 1.01x slower                                                           |
| pickle                   | 7.83 us                                                         | 7.98 us: 1.02x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.10 us: 1.02x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.48 us: 1.03x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 84.0 ms: 1.03x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 71.5 ms: 1.08x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.38 ms: 1.08x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.9 us: 1.09x slower                                                           |
| async_generators         | 241 ms                                                          | 267 ms: 1.11x slower                                                            |
| python_startup_no_site   | 18.1 ms                                                         | 20.2 ms: 1.12x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| telco                    | 4.83 ms                                                         | 5.84 ms: 1.21x slower                                                           |
| coverage                 | 46.6 ms                                                         | 463 ms: 9.95x slower                                                            |
| Geometric mean           | (ref)                                                           | 1.20x faster                                                                    |

Benchmark hidden because not significant (1): pickle_list
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown