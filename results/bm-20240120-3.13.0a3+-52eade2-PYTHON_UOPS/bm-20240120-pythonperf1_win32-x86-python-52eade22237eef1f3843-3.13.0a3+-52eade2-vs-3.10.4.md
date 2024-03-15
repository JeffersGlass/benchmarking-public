
# Results vs. 3.10.4

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-x86
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.15x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 241 ms: 1.10x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.80 ms: 1.11x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.80 sec: 1.08x faster                                                          |
| tornado_http   | 118 ms                                                          | 101 ms: 1.17x faster                                                            |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 510 ms: 1.81x faster                                                            |
| async_tree_none         | 394 ms                                                          | 252 ms: 1.56x faster                                                            |
| async_tree_io           | 940 ms                                                          | 605 ms: 1.56x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 316 ms: 1.48x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.60x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 197 ms: 2.55x faster                                                            |
| float          | 69.6 ms                                                         | 57.4 ms: 1.21x faster                                                           |
| nbody          | 79.1 ms                                                         | 85.3 ms: 1.08x slower                                                           |
| Geometric mean | (ref)                                                           | 1.42x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 103 ms: 1.13x faster                                                            |
| regex_dna      | 131 ms                                                          | 116 ms: 1.12x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 15.9 ms: 1.01x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.87 ms: 1.13x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.75 ms: 1.46x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 212 us: 1.32x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 153 us: 1.24x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.61 sec: 1.19x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 41.0 ms: 1.17x faster                                                           |
| json_loads           | 22.4 us                                                         | 19.7 us: 1.14x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| xml_etree_generate   | 61.6 ms                                                         | 59.2 ms: 1.04x faster                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.4 ms: 1.04x faster                                                           |
| pickle               | 7.83 us                                                         | 7.67 us: 1.02x faster                                                           |
| unpickle             | 9.82 us                                                         | 9.68 us: 1.01x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.94 us: 1.01x faster                                                           |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 18.1 ms                                                         | 20.6 ms: 1.14x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.57 ms: 1.20x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 91.6 us: 4.32x faster                                                           |
| pidigits                 | 502 ms                                                          | 197 ms: 2.55x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 510 ms: 1.81x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 60.6 ns: 1.62x faster                                                           |
| async_tree_none          | 394 ms                                                          | 252 ms: 1.56x faster                                                            |
| async_tree_io            | 940 ms                                                          | 605 ms: 1.56x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.63 ms: 1.53x faster                                                           |
| richards_super           | 49.9 ms                                                         | 32.8 ms: 1.52x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 53.8 ms: 1.51x faster                                                           |
| raytrace                 | 303 ms                                                          | 201 ms: 1.51x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 887 us: 1.50x faster                                                            |
| async_tree_memoization   | 467 ms                                                          | 316 ms: 1.48x faster                                                            |
| json_dumps               | 9.82 ms                                                         | 6.75 ms: 1.46x faster                                                           |
| chaos                    | 74.4 ms                                                         | 51.4 ms: 1.45x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 62.2 ms: 1.44x faster                                                           |
| richards                 | 40.3 ms                                                         | 28.5 ms: 1.41x faster                                                           |
| generators               | 31.6 ms                                                         | 22.4 ms: 1.41x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.13 ms: 1.40x faster                                                           |
| go                       | 146 ms                                                          | 104 ms: 1.40x faster                                                            |
| scimark_sor              | 115 ms                                                          | 84.1 ms: 1.37x faster                                                           |
| comprehensions           | 17.7 us                                                         | 13.2 us: 1.34x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 212 us: 1.32x faster                                                            |
| pycparser                | 1.04 sec                                                        | 816 ms: 1.28x faster                                                            |
| coroutines               | 17.9 ms                                                         | 14.2 ms: 1.26x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.84 us: 1.25x faster                                                           |
| pyflate                  | 422 ms                                                          | 338 ms: 1.25x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 153 us: 1.24x faster                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 50.1 ms: 1.24x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 608 ms: 1.22x faster                                                            |
| float                    | 69.6 ms                                                         | 57.4 ms: 1.21x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 5.07 ms: 1.21x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 24.5 us: 1.21x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.57 ms: 1.20x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.61 sec: 1.19x faster                                                          |
| xml_etree_process        | 48.1 ms                                                         | 41.0 ms: 1.17x faster                                                           |
| json                     | 4.76 ms                                                         | 4.06 ms: 1.17x faster                                                           |
| tornado_http             | 118 ms                                                          | 101 ms: 1.17x faster                                                            |
| sympy_sum                | 122 ms                                                          | 106 ms: 1.15x faster                                                            |
| deepcopy                 | 310 us                                                          | 271 us: 1.14x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 202 ms: 1.14x faster                                                            |
| json_loads               | 22.4 us                                                         | 19.7 us: 1.14x faster                                                           |
| dask                     | 341 ms                                                          | 302 ms: 1.13x faster                                                            |
| regex_compile            | 117 ms                                                          | 103 ms: 1.13x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 39.6 ms: 1.13x faster                                                           |
| mdp                      | 1.83 sec                                                        | 1.62 sec: 1.13x faster                                                          |
| pprint_pformat           | 1.37 sec                                                        | 1.22 sec: 1.12x faster                                                          |
| regex_dna                | 131 ms                                                          | 116 ms: 1.12x faster                                                            |
| nqueens                  | 87.1 ms                                                         | 77.8 ms: 1.12x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.80 ms: 1.11x faster                                                           |
| pprint_safe_repr         | 658 ms                                                          | 596 ms: 1.10x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.43 us: 1.10x faster                                                           |
| sympy_integrate          | 16.6 ms                                                         | 15.1 ms: 1.10x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| sympy_str                | 229 ms                                                          | 208 ms: 1.10x faster                                                            |
| 2to3                     | 265 ms                                                          | 241 ms: 1.10x faster                                                            |
| sympy_expand             | 391 ms                                                          | 359 ms: 1.09x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.80 sec: 1.08x faster                                                          |
| bench_thread_pool        | 1.12 ms                                                         | 1.04 ms: 1.08x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 655 us: 1.06x faster                                                            |
| xml_etree_generate       | 61.6 ms                                                         | 59.2 ms: 1.04x faster                                                           |
| fannkuch                 | 317 ms                                                          | 305 ms: 1.04x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.4 ms: 1.04x faster                                                           |
| meteor_contest           | 80.0 ms                                                         | 77.3 ms: 1.04x faster                                                           |
| pickle                   | 7.83 us                                                         | 7.67 us: 1.02x faster                                                           |
| unpickle                 | 9.82 us                                                         | 9.68 us: 1.01x faster                                                           |
| unpickle_list            | 2.98 us                                                         | 2.94 us: 1.01x faster                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.21 ms: 1.01x faster                                                           |
| regex_v8                 | 15.8 ms                                                         | 15.9 ms: 1.01x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 40.4 ns: 1.01x slower                                                           |
| scimark_fft              | 216 ms                                                          | 220 ms: 1.02x slower                                                            |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.4 sec: 1.02x slower                                                          |
| logging_format           | 7.91 us                                                         | 8.34 us: 1.05x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.79 us: 1.07x slower                                                           |
| spectral_norm            | 80.2 ms                                                         | 85.7 ms: 1.07x slower                                                           |
| nbody                    | 79.1 ms                                                         | 85.3 ms: 1.08x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 87.6 ms: 1.08x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.38 ms: 1.08x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 72.5 ms: 1.09x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| async_generators         | 241 ms                                                          | 268 ms: 1.11x slower                                                            |
| regex_effbot             | 1.66 ms                                                         | 1.87 ms: 1.13x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.6 ms: 1.14x slower                                                           |
| telco                    | 4.83 ms                                                         | 5.82 ms: 1.21x slower                                                           |
| coverage                 | 46.6 ms                                                         | 474 ms: 10.18x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.15x faster                                                                    |

Benchmark hidden because not significant (2): pickle_list, python_startup
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown