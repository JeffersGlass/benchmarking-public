
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 250 ms: 1.06x faster                                                                      |
| chameleon      | 6.42 ms                                                         | 5.86 ms: 1.10x faster                                                                     |
| docutils       | 1.95 sec                                                        | 1.83 sec: 1.07x faster                                                                    |
| tornado_http   | 118 ms                                                          | 101 ms: 1.17x faster                                                                      |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 522 ms: 1.77x faster                                                                      |
| async_tree_none         | 394 ms                                                          | 261 ms: 1.51x faster                                                                      |
| async_tree_io           | 940 ms                                                          | 628 ms: 1.50x faster                                                                      |
| async_tree_memoization  | 467 ms                                                          | 325 ms: 1.43x faster                                                                      |
| Geometric mean          | (ref)                                                           | 1.55x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 202 ms: 2.49x faster                                                                      |
| float          | 69.6 ms                                                         | 58.5 ms: 1.19x faster                                                                     |
| nbody          | 79.1 ms                                                         | 85.2 ms: 1.08x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.40x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 108 ms: 1.08x faster                                                                      |
| regex_dna      | 131 ms                                                          | 126 ms: 1.03x faster                                                                      |
| regex_v8       | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                                     |
| regex_effbot   | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.01x slower                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.62 ms: 1.48x faster                                                                     |
| pickle_pure_python   | 280 us                                                          | 209 us: 1.34x faster                                                                      |
| unpickle_pure_python | 189 us                                                          | 149 us: 1.27x faster                                                                      |
| xml_etree_process    | 48.1 ms                                                         | 41.3 ms: 1.16x faster                                                                     |
| tomli_loads          | 1.91 sec                                                        | 1.64 sec: 1.16x faster                                                                    |
| json_loads           | 22.4 us                                                         | 19.9 us: 1.13x faster                                                                     |
| xml_etree_parse      | 120 ms                                                          | 110 ms: 1.09x faster                                                                      |
| unpickle_list        | 2.98 us                                                         | 2.87 us: 1.04x faster                                                                     |
| pickle               | 7.83 us                                                         | 7.64 us: 1.02x faster                                                                     |
| xml_etree_iterparse  | 70.8 ms                                                         | 69.2 ms: 1.02x faster                                                                     |
| xml_etree_generate   | 61.6 ms                                                         | 60.6 ms: 1.02x faster                                                                     |
| unpickle             | 9.82 us                                                         | 9.88 us: 1.01x slower                                                                     |
| pickle_list          | 3.22 us                                                         | 3.48 us: 1.08x slower                                                                     |
| pickle_dict          | 18.2 us                                                         | 20.2 us: 1.11x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.5 ms: 1.03x slower                                                                     |
| python_startup_no_site | 18.1 ms                                                         | 21.1 ms: 1.17x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.10x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.86 ms: 1.16x faster                                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 94.8 us: 4.17x faster                                                                     |
| pidigits                 | 502 ms                                                          | 202 ms: 2.49x faster                                                                      |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 522 ms: 1.77x faster                                                                      |
| logging_silent           | 97.9 ns                                                         | 59.5 ns: 1.64x faster                                                                     |
| deltablue                | 4.04 ms                                                         | 2.65 ms: 1.53x faster                                                                     |
| async_tree_none          | 394 ms                                                          | 261 ms: 1.51x faster                                                                      |
| async_tree_io            | 940 ms                                                          | 628 ms: 1.50x faster                                                                      |
| richards_super           | 49.9 ms                                                         | 33.5 ms: 1.49x faster                                                                     |
| json_dumps               | 9.82 ms                                                         | 6.62 ms: 1.48x faster                                                                     |
| scimark_lu               | 89.8 ms                                                         | 62.1 ms: 1.45x faster                                                                     |
| sqlglot_parse            | 1.33 ms                                                         | 920 us: 1.45x faster                                                                      |
| async_tree_memoization   | 467 ms                                                          | 325 ms: 1.43x faster                                                                      |
| chaos                    | 74.4 ms                                                         | 52.1 ms: 1.43x faster                                                                     |
| raytrace                 | 303 ms                                                          | 216 ms: 1.40x faster                                                                      |
| crypto_pyaes             | 81.3 ms                                                         | 58.3 ms: 1.39x faster                                                                     |
| richards                 | 40.3 ms                                                         | 29.3 ms: 1.38x faster                                                                     |
| scimark_sor              | 115 ms                                                          | 83.7 ms: 1.37x faster                                                                     |
| generators               | 31.6 ms                                                         | 23.2 ms: 1.36x faster                                                                     |
| go                       | 146 ms                                                          | 107 ms: 1.36x faster                                                                      |
| sqlglot_transpile        | 1.58 ms                                                         | 1.17 ms: 1.35x faster                                                                     |
| pickle_pure_python       | 280 us                                                          | 209 us: 1.34x faster                                                                      |
| comprehensions           | 17.7 us                                                         | 13.2 us: 1.34x faster                                                                     |
| unpickle_pure_python     | 189 us                                                          | 149 us: 1.27x faster                                                                      |
| pyflate                  | 422 ms                                                          | 337 ms: 1.25x faster                                                                      |
| sqlite_synth             | 2.29 us                                                         | 1.84 us: 1.25x faster                                                                     |
| coroutines               | 17.9 ms                                                         | 14.6 ms: 1.23x faster                                                                     |
| pycparser                | 1.04 sec                                                        | 854 ms: 1.22x faster                                                                      |
| scimark_monte_carlo      | 61.9 ms                                                         | 51.3 ms: 1.21x faster                                                                     |
| float                    | 69.6 ms                                                         | 58.5 ms: 1.19x faster                                                                     |
| hexiom                   | 6.13 ms                                                         | 5.18 ms: 1.18x faster                                                                     |
| tornado_http             | 118 ms                                                          | 101 ms: 1.17x faster                                                                      |
| deepcopy_memo            | 29.6 us                                                         | 25.4 us: 1.17x faster                                                                     |
| xml_etree_process        | 48.1 ms                                                         | 41.3 ms: 1.16x faster                                                                     |
| tomli_loads              | 1.91 sec                                                        | 1.64 sec: 1.16x faster                                                                    |
| mako                     | 9.10 ms                                                         | 7.86 ms: 1.16x faster                                                                     |
| json                     | 4.76 ms                                                         | 4.14 ms: 1.15x faster                                                                     |
| nqueens                  | 87.1 ms                                                         | 77.0 ms: 1.13x faster                                                                     |
| json_loads               | 22.4 us                                                         | 19.9 us: 1.13x faster                                                                     |
| deepcopy                 | 310 us                                                          | 280 us: 1.11x faster                                                                      |
| asyncio_tcp              | 744 ms                                                          | 673 ms: 1.11x faster                                                                      |
| sympy_sum                | 122 ms                                                          | 111 ms: 1.10x faster                                                                      |
| chameleon                | 6.42 ms                                                         | 5.86 ms: 1.10x faster                                                                     |
| deepcopy_reduce          | 2.68 us                                                         | 2.45 us: 1.09x faster                                                                     |
| mdp                      | 1.83 sec                                                        | 1.67 sec: 1.09x faster                                                                    |
| dask                     | 341 ms                                                          | 312 ms: 1.09x faster                                                                      |
| xml_etree_parse          | 120 ms                                                          | 110 ms: 1.09x faster                                                                      |
| pprint_pformat           | 1.37 sec                                                        | 1.26 sec: 1.09x faster                                                                    |
| sqlglot_normalize        | 230 ms                                                          | 213 ms: 1.08x faster                                                                      |
| regex_compile            | 117 ms                                                          | 108 ms: 1.08x faster                                                                      |
| create_gc_cycles         | 694 us                                                          | 647 us: 1.07x faster                                                                      |
| fannkuch                 | 317 ms                                                          | 296 ms: 1.07x faster                                                                      |
| sqlglot_optimize         | 44.7 ms                                                         | 41.8 ms: 1.07x faster                                                                     |
| sympy_str                | 229 ms                                                          | 214 ms: 1.07x faster                                                                      |
| sympy_integrate          | 16.6 ms                                                         | 15.6 ms: 1.07x faster                                                                     |
| docutils                 | 1.95 sec                                                        | 1.83 sec: 1.07x faster                                                                    |
| pprint_safe_repr         | 658 ms                                                          | 621 ms: 1.06x faster                                                                      |
| 2to3                     | 265 ms                                                          | 250 ms: 1.06x faster                                                                      |
| sympy_expand             | 391 ms                                                          | 372 ms: 1.05x faster                                                                      |
| bench_thread_pool        | 1.12 ms                                                         | 1.07 ms: 1.05x faster                                                                     |
| unpickle_list            | 2.98 us                                                         | 2.87 us: 1.04x faster                                                                     |
| regex_dna                | 131 ms                                                          | 126 ms: 1.03x faster                                                                      |
| meteor_contest           | 80.0 ms                                                         | 77.6 ms: 1.03x faster                                                                     |
| pickle                   | 7.83 us                                                         | 7.64 us: 1.02x faster                                                                     |
| xml_etree_iterparse      | 70.8 ms                                                         | 69.2 ms: 1.02x faster                                                                     |
| xml_etree_generate       | 61.6 ms                                                         | 60.6 ms: 1.02x faster                                                                     |
| unpack_sequence          | 40.0 ns                                                         | 39.5 ns: 1.01x faster                                                                     |
| unpickle                 | 9.82 us                                                         | 9.88 us: 1.01x slower                                                                     |
| spectral_norm            | 80.2 ms                                                         | 81.6 ms: 1.02x slower                                                                     |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.30 ms: 1.02x slower                                                                     |
| python_startup           | 22.9 ms                                                         | 23.5 ms: 1.03x slower                                                                     |
| regex_v8                 | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                                     |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                                    |
| nbody                    | 79.1 ms                                                         | 85.2 ms: 1.08x slower                                                                     |
| pickle_list              | 3.22 us                                                         | 3.48 us: 1.08x slower                                                                     |
| pathlib                  | 81.2 ms                                                         | 88.7 ms: 1.09x slower                                                                     |
| gc_traversal             | 1.28 ms                                                         | 1.40 ms: 1.10x slower                                                                     |
| pickle_dict              | 18.2 us                                                         | 20.2 us: 1.11x slower                                                                     |
| async_generators         | 241 ms                                                          | 271 ms: 1.13x slower                                                                      |
| logging_format           | 7.91 us                                                         | 8.99 us: 1.14x slower                                                                     |
| bench_mp_pool            | 66.4 ms                                                         | 75.5 ms: 1.14x slower                                                                     |
| regex_effbot             | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                                     |
| logging_simple           | 7.29 us                                                         | 8.37 us: 1.15x slower                                                                     |
| python_startup_no_site   | 18.1 ms                                                         | 21.1 ms: 1.17x slower                                                                     |
| telco                    | 4.83 ms                                                         | 6.07 ms: 1.26x slower                                                                     |
| coverage                 | 46.6 ms                                                         | 485 ms: 10.42x slower                                                                     |
| Geometric mean           | (ref)                                                           | 1.13x faster                                                                              |

Benchmark hidden because not significant (1): scimark_fft
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-cf59bba-PYTHON_UOPS/bm-20240127-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown