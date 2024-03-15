
# Results vs. 3.10.4

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 232 ms: 1.15x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.76 ms: 1.12x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.71 sec: 1.14x faster                                                          |
| tornado_http   | 118 ms                                                          | 93.8 ms: 1.25x faster                                                           |
| Geometric mean | (ref)                                                           | 1.16x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 499 ms: 1.85x faster                                                            |
| async_tree_none         | 394 ms                                                          | 244 ms: 1.61x faster                                                            |
| async_tree_io           | 940 ms                                                          | 587 ms: 1.60x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 303 ms: 1.54x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.65x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 197 ms: 2.55x faster                                                            |
| float          | 69.6 ms                                                         | 54.4 ms: 1.28x faster                                                           |
| nbody          | 79.1 ms                                                         | 78.1 ms: 1.01x faster                                                           |
| Geometric mean | (ref)                                                           | 1.49x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 96.1 ms: 1.21x faster                                                           |
| regex_dna      | 131 ms                                                          | 119 ms: 1.10x faster                                                            |
| regex_effbot   | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                    |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.69 ms: 1.47x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 206 us: 1.36x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 141 us: 1.35x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.59 sec: 1.20x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 40.9 ms: 1.18x faster                                                           |
| json_loads           | 22.4 us                                                         | 19.8 us: 1.13x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.11x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 64.6 ms: 1.10x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 59.3 ms: 1.04x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.88 us: 1.03x faster                                                           |
| unpickle             | 9.82 us                                                         | 9.91 us: 1.01x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 19.9 us: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.12x faster                                                                    |

Benchmark hidden because not significant (2): pickle, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.7 ms: 1.01x faster                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.4 ms: 1.13x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 6.86 ms: 1.33x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 88.6 us: 4.46x faster                                                           |
| pidigits                 | 502 ms                                                          | 197 ms: 2.55x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.15 ms: 1.88x faster                                                           |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 499 ms: 1.85x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 57.3 ns: 1.71x faster                                                           |
| async_tree_none          | 394 ms                                                          | 244 ms: 1.61x faster                                                            |
| chaos                    | 74.4 ms                                                         | 46.3 ms: 1.61x faster                                                           |
| raytrace                 | 303 ms                                                          | 189 ms: 1.60x faster                                                            |
| async_tree_io            | 940 ms                                                          | 587 ms: 1.60x faster                                                            |
| comprehensions           | 17.7 us                                                         | 11.4 us: 1.56x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 853 us: 1.56x faster                                                            |
| async_tree_memoization   | 467 ms                                                          | 303 ms: 1.54x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 52.9 ms: 1.54x faster                                                           |
| richards_super           | 49.9 ms                                                         | 32.9 ms: 1.52x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 59.2 ms: 1.52x faster                                                           |
| go                       | 146 ms                                                          | 96.7 ms: 1.51x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.69 ms: 1.47x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.08 ms: 1.46x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 4.25 ms: 1.44x faster                                                           |
| generators               | 31.6 ms                                                         | 22.5 ms: 1.40x faster                                                           |
| richards                 | 40.3 ms                                                         | 28.9 ms: 1.39x faster                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 45.1 ms: 1.37x faster                                                           |
| scimark_sor              | 115 ms                                                          | 84.1 ms: 1.37x faster                                                           |
| pyflate                  | 422 ms                                                          | 309 ms: 1.36x faster                                                            |
| pickle_pure_python       | 280 us                                                          | 206 us: 1.36x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 141 us: 1.35x faster                                                            |
| mako                     | 9.10 ms                                                         | 6.86 ms: 1.33x faster                                                           |
| pycparser                | 1.04 sec                                                        | 794 ms: 1.31x faster                                                            |
| float                    | 69.6 ms                                                         | 54.4 ms: 1.28x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 23.6 us: 1.25x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 69.5 ms: 1.25x faster                                                           |
| tornado_http             | 118 ms                                                          | 93.8 ms: 1.25x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.4 ms: 1.25x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 64.4 ms: 1.25x faster                                                           |
| sympy_sum                | 122 ms                                                          | 100 ms: 1.22x faster                                                            |
| regex_compile            | 117 ms                                                          | 96.1 ms: 1.21x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.59 sec: 1.20x faster                                                          |
| json                     | 4.76 ms                                                         | 4.03 ms: 1.18x faster                                                           |
| fannkuch                 | 317 ms                                                          | 269 ms: 1.18x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 196 ms: 1.18x faster                                                            |
| xml_etree_process        | 48.1 ms                                                         | 40.9 ms: 1.18x faster                                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 38.2 ms: 1.17x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.96 us: 1.17x faster                                                           |
| sympy_integrate          | 16.6 ms                                                         | 14.3 ms: 1.17x faster                                                           |
| sympy_str                | 229 ms                                                          | 197 ms: 1.16x faster                                                            |
| asyncio_tcp              | 744 ms                                                          | 648 ms: 1.15x faster                                                            |
| 2to3                     | 265 ms                                                          | 232 ms: 1.15x faster                                                            |
| deepcopy                 | 310 us                                                          | 271 us: 1.14x faster                                                            |
| sympy_expand             | 391 ms                                                          | 343 ms: 1.14x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.60 sec: 1.14x faster                                                          |
| docutils                 | 1.95 sec                                                        | 1.71 sec: 1.14x faster                                                          |
| pprint_pformat           | 1.37 sec                                                        | 1.20 sec: 1.14x faster                                                          |
| bench_thread_pool        | 1.12 ms                                                         | 991 us: 1.13x faster                                                            |
| json_loads               | 22.4 us                                                         | 19.8 us: 1.13x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.40 us: 1.12x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.76 ms: 1.12x faster                                                           |
| pprint_safe_repr         | 658 ms                                                          | 591 ms: 1.11x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.11x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 64.6 ms: 1.10x faster                                                           |
| regex_dna                | 131 ms                                                          | 119 ms: 1.10x faster                                                            |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 2.98 ms: 1.09x faster                                                           |
| unpack_sequence          | 40.0 ns                                                         | 37.5 ns: 1.07x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 651 us: 1.07x faster                                                            |
| meteor_contest           | 80.0 ms                                                         | 75.8 ms: 1.06x faster                                                           |
| scimark_fft              | 216 ms                                                          | 206 ms: 1.05x faster                                                            |
| xml_etree_generate       | 61.6 ms                                                         | 59.3 ms: 1.04x faster                                                           |
| unpickle_list            | 2.98 us                                                         | 2.88 us: 1.03x faster                                                           |
| nbody                    | 79.1 ms                                                         | 78.1 ms: 1.01x faster                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| python_startup           | 22.9 ms                                                         | 22.7 ms: 1.01x faster                                                           |
| unpickle                 | 9.82 us                                                         | 9.91 us: 1.01x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 85.1 ms: 1.05x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.36 us: 1.06x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.79 us: 1.07x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.39 ms: 1.08x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 71.8 ms: 1.08x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.9 us: 1.09x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.4 ms: 1.13x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| async_generators         | 241 ms                                                          | 277 ms: 1.15x slower                                                            |
| telco                    | 4.83 ms                                                         | 5.84 ms: 1.21x slower                                                           |
| coverage                 | 46.6 ms                                                         | 474 ms: 10.19x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.19x faster                                                                    |

Benchmark hidden because not significant (3): regex_v8, pickle, pickle_list
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: unknown