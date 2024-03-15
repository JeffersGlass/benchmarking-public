
# Results vs. 3.10.4

- fork: python
- ref: 68a7b78cd5185cbd9456
- machine: windows-x86
- commit hash: 68a7b78
- commit date: 2024-01-18
- overall geometric mean: 1.14x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 241 ms: 1.10x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.80 ms: 1.11x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.79 sec: 1.09x faster                                                          |
| tornado_http   | 118 ms                                                          | 101 ms: 1.16x faster                                                            |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 511 ms: 1.80x faster                                                            |
| async_tree_none         | 394 ms                                                          | 247 ms: 1.59x faster                                                            |
| async_tree_io           | 940 ms                                                          | 602 ms: 1.56x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 310 ms: 1.51x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.61x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 199 ms: 2.53x faster                                                            |
| float          | 69.6 ms                                                         | 59.3 ms: 1.17x faster                                                           |
| nbody          | 79.1 ms                                                         | 86.8 ms: 1.10x slower                                                           |
| Geometric mean | (ref)                                                           | 1.39x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 104 ms: 1.12x faster                                                            |
| regex_dna      | 131 ms                                                          | 121 ms: 1.08x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.01x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.01x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.72 ms: 1.46x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 210 us: 1.33x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 156 us: 1.22x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 41.2 ms: 1.17x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.65 sec: 1.16x faster                                                          |
| json_loads           | 22.4 us                                                         | 19.8 us: 1.13x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 111 ms: 1.08x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.0 ms: 1.04x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 59.9 ms: 1.03x faster                                                           |
| pickle               | 7.83 us                                                         | 7.89 us: 1.01x slower                                                           |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.02x slower                                                           |
| pickle_list          | 3.22 us                                                         | 3.31 us: 1.03x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.0 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                                    |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.3 ms: 1.02x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 21.0 ms: 1.16x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.09x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.77 ms: 1.17x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 90.3 us: 4.38x faster                                                           |
| pidigits                 | 502 ms                                                          | 199 ms: 2.53x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 511 ms: 1.80x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 60.1 ns: 1.63x faster                                                           |
| async_tree_none          | 394 ms                                                          | 247 ms: 1.59x faster                                                            |
| async_tree_io            | 940 ms                                                          | 602 ms: 1.56x faster                                                            |
| richards_super           | 49.9 ms                                                         | 32.5 ms: 1.53x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 310 ms: 1.51x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 900 us: 1.48x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 55.4 ms: 1.47x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.72 ms: 1.46x faster                                                           |
| raytrace                 | 303 ms                                                          | 207 ms: 1.46x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.81 ms: 1.44x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 62.7 ms: 1.43x faster                                                           |
| scimark_sor              | 115 ms                                                          | 81.2 ms: 1.42x faster                                                           |
| richards                 | 40.3 ms                                                         | 28.8 ms: 1.40x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.14 ms: 1.39x faster                                                           |
| chaos                    | 74.4 ms                                                         | 53.6 ms: 1.39x faster                                                           |
| go                       | 146 ms                                                          | 105 ms: 1.39x faster                                                            |
| generators               | 31.6 ms                                                         | 23.3 ms: 1.35x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 210 us: 1.33x faster                                                            |
| comprehensions           | 17.7 us                                                         | 13.6 us: 1.31x faster                                                           |
| pycparser                | 1.04 sec                                                        | 812 ms: 1.28x faster                                                            |
| coroutines               | 17.9 ms                                                         | 14.3 ms: 1.26x faster                                                           |
| pyflate                  | 422 ms                                                          | 337 ms: 1.25x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 24.1 us: 1.23x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 156 us: 1.22x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 1.91 us: 1.20x faster                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 52.5 ms: 1.18x faster                                                           |
| float                    | 69.6 ms                                                         | 59.3 ms: 1.17x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.77 ms: 1.17x faster                                                           |
| json                     | 4.76 ms                                                         | 4.07 ms: 1.17x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 41.2 ms: 1.17x faster                                                           |
| deepcopy                 | 310 us                                                          | 266 us: 1.17x faster                                                            |
| asyncio_tcp              | 744 ms                                                          | 639 ms: 1.16x faster                                                            |
| tornado_http             | 118 ms                                                          | 101 ms: 1.16x faster                                                            |
| hexiom                   | 6.13 ms                                                         | 5.29 ms: 1.16x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.65 sec: 1.16x faster                                                          |
| pprint_pformat           | 1.37 sec                                                        | 1.19 sec: 1.15x faster                                                          |
| sympy_sum                | 122 ms                                                          | 107 ms: 1.14x faster                                                            |
| json_loads               | 22.4 us                                                         | 19.8 us: 1.13x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 77.1 ms: 1.13x faster                                                           |
| dask                     | 341 ms                                                          | 303 ms: 1.13x faster                                                            |
| pprint_safe_repr         | 658 ms                                                          | 585 ms: 1.12x faster                                                            |
| regex_compile            | 117 ms                                                          | 104 ms: 1.12x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 207 ms: 1.11x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.41 us: 1.11x faster                                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 40.4 ms: 1.11x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.80 ms: 1.11x faster                                                           |
| 2to3                     | 265 ms                                                          | 241 ms: 1.10x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.2 ms: 1.09x faster                                                           |
| docutils                 | 1.95 sec                                                        | 1.79 sec: 1.09x faster                                                          |
| xml_etree_parse          | 120 ms                                                          | 111 ms: 1.08x faster                                                            |
| regex_dna                | 131 ms                                                          | 121 ms: 1.08x faster                                                            |
| sympy_str                | 229 ms                                                          | 212 ms: 1.08x faster                                                            |
| fannkuch                 | 317 ms                                                          | 294 ms: 1.08x faster                                                            |
| sympy_expand             | 391 ms                                                          | 365 ms: 1.07x faster                                                            |
| create_gc_cycles         | 694 us                                                          | 651 us: 1.07x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.06 ms: 1.06x faster                                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.0 ms: 1.04x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 59.9 ms: 1.03x faster                                                           |
| meteor_contest           | 80.0 ms                                                         | 78.8 ms: 1.01x faster                                                           |
| mdp                      | 1.83 sec                                                        | 1.80 sec: 1.01x faster                                                          |
| pickle                   | 7.83 us                                                         | 7.89 us: 1.01x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.01x slower                                                           |
| python_startup           | 22.9 ms                                                         | 23.3 ms: 1.02x slower                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.3 sec: 1.02x slower                                                          |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.02x slower                                                           |
| pickle_list              | 3.22 us                                                         | 3.31 us: 1.03x slower                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.37 ms: 1.04x slower                                                           |
| scimark_fft              | 216 ms                                                          | 231 ms: 1.07x slower                                                            |
| pathlib                  | 81.2 ms                                                         | 87.7 ms: 1.08x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.60 us: 1.09x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.39 ms: 1.09x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.94 us: 1.09x slower                                                           |
| nbody                    | 79.1 ms                                                         | 86.8 ms: 1.10x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.0 us: 1.10x slower                                                           |
| spectral_norm            | 80.2 ms                                                         | 89.4 ms: 1.11x slower                                                           |
| async_generators         | 241 ms                                                          | 272 ms: 1.13x slower                                                            |
| regex_effbot             | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 75.8 ms: 1.14x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 21.0 ms: 1.16x slower                                                           |
| telco                    | 4.83 ms                                                         | 5.65 ms: 1.17x slower                                                           |
| coverage                 | 46.6 ms                                                         | 474 ms: 10.17x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.14x faster                                                                    |

Benchmark hidden because not significant (2): unpickle_list, unpack_sequence
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240118-3.13.0a3+-68a7b78-PYTHON_UOPS/bm-20240118-pythonperf1_win32-x86-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown