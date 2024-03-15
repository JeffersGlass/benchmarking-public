
# Results vs. 3.10.4

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 252 ms: 1.05x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.98 ms: 1.07x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                          |
| tornado_http   | 118 ms                                                          | 98.6 ms: 1.19x faster                                                           |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 512 ms: 1.80x faster                                                            |
| async_tree_none         | 394 ms                                                          | 259 ms: 1.52x faster                                                            |
| async_tree_io           | 940 ms                                                          | 620 ms: 1.52x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 327 ms: 1.43x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.56x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 201 ms: 2.51x faster                                                            |
| float          | 69.6 ms                                                         | 53.8 ms: 1.30x faster                                                           |
| nbody          | 79.1 ms                                                         | 94.2 ms: 1.19x slower                                                           |
| Geometric mean | (ref)                                                           | 1.40x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 120 ms: 1.09x faster                                                            |
| regex_compile  | 117 ms                                                          | 108 ms: 1.08x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 15.7 ms: 1.00x faster                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.87 ms: 1.13x slower                                                           |
| Geometric mean | (ref)                                                           | 1.01x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.88 ms: 1.43x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 219 us: 1.28x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 158 us: 1.20x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.66 sec: 1.15x faster                                                          |
| json_loads           | 22.4 us                                                         | 19.8 us: 1.13x faster                                                           |
| xml_etree_process    | 48.1 ms                                                         | 42.6 ms: 1.13x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 65.7 ms: 1.08x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 60.8 ms: 1.01x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.96 us: 1.01x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.28 us: 1.02x slower                                                           |
| pickle               | 7.83 us                                                         | 8.09 us: 1.03x slower                                                           |
| unpickle             | 9.82 us                                                         | 10.3 us: 1.05x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 18.1 ms                                                         | 20.8 ms: 1.15x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.31 ms: 1.24x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 97.1 us: 4.08x faster                                                           |
| pidigits                 | 502 ms                                                          | 201 ms: 2.51x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 512 ms: 1.80x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.57 ms: 1.57x faster                                                           |
| async_tree_none          | 394 ms                                                          | 259 ms: 1.52x faster                                                            |
| async_tree_io            | 940 ms                                                          | 620 ms: 1.52x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 67.7 ns: 1.45x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 327 ms: 1.43x faster                                                            |
| json_dumps               | 9.82 ms                                                         | 6.88 ms: 1.43x faster                                                           |
| richards_super           | 49.9 ms                                                         | 35.1 ms: 1.42x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 957 us: 1.39x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 60.7 ms: 1.34x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 68.4 ms: 1.31x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.21 ms: 1.31x faster                                                           |
| scimark_sor              | 115 ms                                                          | 88.3 ms: 1.30x faster                                                           |
| float                    | 69.6 ms                                                         | 53.8 ms: 1.30x faster                                                           |
| generators               | 31.6 ms                                                         | 24.5 ms: 1.29x faster                                                           |
| richards                 | 40.3 ms                                                         | 31.5 ms: 1.28x faster                                                           |
| comprehensions           | 17.7 us                                                         | 13.9 us: 1.28x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 219 us: 1.28x faster                                                            |
| raytrace                 | 303 ms                                                          | 238 ms: 1.27x faster                                                            |
| chaos                    | 74.4 ms                                                         | 59.0 ms: 1.26x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.31 ms: 1.24x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.87 us: 1.23x faster                                                           |
| go                       | 146 ms                                                          | 119 ms: 1.22x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 158 us: 1.20x faster                                                            |
| tornado_http             | 118 ms                                                          | 98.6 ms: 1.19x faster                                                           |
| pycparser                | 1.04 sec                                                        | 876 ms: 1.19x faster                                                            |
| coroutines               | 17.9 ms                                                         | 15.1 ms: 1.18x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 632 ms: 1.18x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 25.3 us: 1.17x faster                                                           |
| json                     | 4.76 ms                                                         | 4.14 ms: 1.15x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.66 sec: 1.15x faster                                                          |
| pyflate                  | 422 ms                                                          | 369 ms: 1.14x faster                                                            |
| json_loads               | 22.4 us                                                         | 19.8 us: 1.13x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 42.6 ms: 1.13x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 71.2 ms: 1.13x faster                                                           |
| sympy_sum                | 122 ms                                                          | 110 ms: 1.11x faster                                                            |
| dask                     | 341 ms                                                          | 307 ms: 1.11x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| regex_dna                | 131 ms                                                          | 120 ms: 1.09x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.03 ms: 1.09x faster                                                           |
| deepcopy                 | 310 us                                                          | 285 us: 1.09x faster                                                            |
| regex_compile            | 117 ms                                                          | 108 ms: 1.08x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                          |
| xml_etree_iterparse      | 70.8 ms                                                         | 65.7 ms: 1.08x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.98 ms: 1.07x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 646 us: 1.07x faster                                                            |
| sympy_str                | 229 ms                                                          | 216 ms: 1.06x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.7 ms: 1.06x faster                                                           |
| sqlglot_normalize        | 230 ms                                                          | 218 ms: 1.06x faster                                                            |
| 2to3                     | 265 ms                                                          | 252 ms: 1.05x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.55 us: 1.05x faster                                                           |
| fannkuch                 | 317 ms                                                          | 303 ms: 1.05x faster                                                            |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.11 ms: 1.04x faster                                                           |
| sympy_expand             | 391 ms                                                          | 376 ms: 1.04x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 43.2 ms: 1.04x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 60.8 ms: 1.01x faster                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.7 sec: 1.01x faster                                                          |
| unpickle_list            | 2.98 us                                                         | 2.96 us: 1.01x faster                                                           |
| regex_v8                 | 15.8 ms                                                         | 15.7 ms: 1.00x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 87.7 ms: 1.01x slower                                                           |
| mdp                      | 1.83 sec                                                        | 1.84 sec: 1.01x slower                                                          |
| pickle_list              | 3.22 us                                                         | 3.28 us: 1.02x slower                                                           |
| pickle                   | 7.83 us                                                         | 8.09 us: 1.03x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 84.1 ms: 1.04x slower                                                           |
| meteor_contest           | 80.0 ms                                                         | 83.5 ms: 1.04x slower                                                           |
| unpickle                 | 9.82 us                                                         | 10.3 us: 1.05x slower                                                           |
| hexiom                   | 6.13 ms                                                         | 6.47 ms: 1.05x slower                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.44 sec: 1.06x slower                                                          |
| pprint_safe_repr         | 658 ms                                                          | 702 ms: 1.07x slower                                                            |
| gc_traversal             | 1.28 ms                                                         | 1.37 ms: 1.07x slower                                                           |
| scimark_fft              | 216 ms                                                          | 235 ms: 1.09x slower                                                            |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 44.1 ns: 1.10x slower                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 68.7 ms: 1.11x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.87 ms: 1.13x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 74.7 ms: 1.13x slower                                                           |
| logging_format           | 7.91 us                                                         | 9.00 us: 1.14x slower                                                           |
| logging_simple           | 7.29 us                                                         | 8.30 us: 1.14x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.8 ms: 1.15x slower                                                           |
| nbody                    | 79.1 ms                                                         | 94.2 ms: 1.19x slower                                                           |
| async_generators         | 241 ms                                                          | 289 ms: 1.20x slower                                                            |
| telco                    | 4.83 ms                                                         | 5.98 ms: 1.24x slower                                                           |
| coverage                 | 46.6 ms                                                         | 466 ms: 10.01x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.10x faster                                                                    |

Benchmark hidden because not significant (1): python_startup
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown