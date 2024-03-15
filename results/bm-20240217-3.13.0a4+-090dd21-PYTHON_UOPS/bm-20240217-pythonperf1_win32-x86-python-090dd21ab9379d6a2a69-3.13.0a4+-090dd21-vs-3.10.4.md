
# Results vs. 3.10.4

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-x86
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 241 ms: 1.10x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.62 ms: 1.14x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.77 sec: 1.10x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.5 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 507 ms: 1.82x faster                                                            |
| async_tree_none         | 394 ms                                                          | 250 ms: 1.58x faster                                                            |
| async_tree_io           | 940 ms                                                          | 602 ms: 1.56x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 313 ms: 1.49x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.61x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| float          | 69.6 ms                                                         | 56.4 ms: 1.23x faster                                                           |
| Geometric mean | (ref)                                                           | 1.46x faster                                                                    |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 104 ms: 1.12x faster                                                            |
| regex_dna      | 131 ms                                                          | 120 ms: 1.09x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.1 ms: 1.02x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.01x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.72 ms: 1.46x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 206 us: 1.36x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 148 us: 1.28x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 40.4 ms: 1.19x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.65 sec: 1.16x faster                                                          |
| json_loads           | 22.4 us                                                         | 19.9 us: 1.12x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 66.3 ms: 1.07x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 58.5 ms: 1.05x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.89 us: 1.03x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.25 us: 1.01x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 19.9 us: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.12x faster                                                                    |

Benchmark hidden because not significant (2): unpickle, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.1 ms: 1.04x faster                                                           |
| python_startup_no_site | 18.1 ms                                                         | 19.9 ms: 1.10x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.03x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.57 ms: 1.20x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 88.4 us: 4.48x faster                                                           |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 507 ms: 1.82x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.31 ms: 1.75x faster                                                           |
| logging_silent           | 97.9 ns                                                         | 59.1 ns: 1.66x faster                                                           |
| async_tree_none          | 394 ms                                                          | 250 ms: 1.58x faster                                                            |
| async_tree_io            | 940 ms                                                          | 602 ms: 1.56x faster                                                            |
| richards_super           | 49.9 ms                                                         | 33.5 ms: 1.49x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 313 ms: 1.49x faster                                                            |
| raytrace                 | 303 ms                                                          | 205 ms: 1.48x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 905 us: 1.47x faster                                                            |
| scimark_sor              | 115 ms                                                          | 78.4 ms: 1.47x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.72 ms: 1.46x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 62.3 ms: 1.44x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 56.6 ms: 1.44x faster                                                           |
| generators               | 31.6 ms                                                         | 22.3 ms: 1.41x faster                                                           |
| go                       | 146 ms                                                          | 103 ms: 1.41x faster                                                            |
| comprehensions           | 17.7 us                                                         | 12.6 us: 1.40x faster                                                           |
| chaos                    | 74.4 ms                                                         | 53.5 ms: 1.39x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.14 ms: 1.38x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 206 us: 1.36x faster                                                            |
| richards                 | 40.3 ms                                                         | 29.8 ms: 1.35x faster                                                           |
| pyflate                  | 422 ms                                                          | 329 ms: 1.28x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 148 us: 1.28x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 23.1 us: 1.28x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.2 ms: 1.27x faster                                                           |
| pycparser                | 1.04 sec                                                        | 837 ms: 1.25x faster                                                            |
| float                    | 69.6 ms                                                         | 56.4 ms: 1.23x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.86 us: 1.23x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 611 ms: 1.22x faster                                                            |
| hexiom                   | 6.13 ms                                                         | 5.06 ms: 1.21x faster                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 51.3 ms: 1.21x faster                                                           |
| tornado_http             | 118 ms                                                          | 97.5 ms: 1.21x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.57 ms: 1.20x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 40.4 ms: 1.19x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 73.6 ms: 1.18x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.65 sec: 1.16x faster                                                          |
| deepcopy                 | 310 us                                                          | 270 us: 1.15x faster                                                            |
| chameleon                | 6.42 ms                                                         | 5.62 ms: 1.14x faster                                                           |
| sympy_sum                | 122 ms                                                          | 108 ms: 1.14x faster                                                            |
| json                     | 4.76 ms                                                         | 4.19 ms: 1.14x faster                                                           |
| dask                     | 341 ms                                                          | 302 ms: 1.13x faster                                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.22 sec: 1.13x faster                                                          |
| json_loads               | 22.4 us                                                         | 19.9 us: 1.12x faster                                                           |
| regex_compile            | 117 ms                                                          | 104 ms: 1.12x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.00 ms: 1.12x faster                                                           |
| sqlglot_normalize        | 230 ms                                                          | 207 ms: 1.11x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| fannkuch                 | 317 ms                                                          | 287 ms: 1.11x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.0 ms: 1.11x faster                                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 40.4 ms: 1.11x faster                                                           |
| pprint_safe_repr         | 658 ms                                                          | 598 ms: 1.10x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.77 sec: 1.10x faster                                                          |
| 2to3                     | 265 ms                                                          | 241 ms: 1.10x faster                                                            |
| regex_dna                | 131 ms                                                          | 120 ms: 1.09x faster                                                            |
| sympy_str                | 229 ms                                                          | 211 ms: 1.09x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.70 sec: 1.08x faster                                                          |
| create_gc_cycles         | 694 us                                                          | 646 us: 1.07x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 66.3 ms: 1.07x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.52 us: 1.06x faster                                                           |
| sympy_expand             | 391 ms                                                          | 369 ms: 1.06x faster                                                            |
| xml_etree_generate       | 61.6 ms                                                         | 58.5 ms: 1.05x faster                                                           |
| meteor_contest           | 80.0 ms                                                         | 76.8 ms: 1.04x faster                                                           |
| unpack_sequence          | 40.0 ns                                                         | 38.6 ns: 1.04x faster                                                           |
| python_startup           | 22.9 ms                                                         | 22.1 ms: 1.04x faster                                                           |
| unpickle_list            | 2.98 us                                                         | 2.89 us: 1.03x faster                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.15 ms: 1.03x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 78.1 ms: 1.03x faster                                                           |
| scimark_fft              | 216 ms                                                          | 211 ms: 1.02x faster                                                            |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| pickle_list              | 3.22 us                                                         | 3.25 us: 1.01x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.1 ms: 1.02x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 84.0 ms: 1.03x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 69.5 ms: 1.05x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.37 ms: 1.07x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.57 us: 1.08x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.9 us: 1.09x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.95 us: 1.09x slower                                                           |
| async_generators         | 241 ms                                                          | 265 ms: 1.10x slower                                                            |
| python_startup_no_site   | 18.1 ms                                                         | 19.9 ms: 1.10x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| telco                    | 4.83 ms                                                         | 5.86 ms: 1.21x slower                                                           |
| coverage                 | 46.6 ms                                                         | 469 ms: 10.08x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.16x faster                                                                    |

Benchmark hidden because not significant (3): unpickle, pickle, nbody
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1_win32-x86-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown