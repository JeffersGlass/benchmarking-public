
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 252 ms: 1.05x faster                                                                      |
| chameleon      | 6.42 ms                                                         | 5.72 ms: 1.12x faster                                                                     |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.07x faster                                                                    |
| tornado_http   | 118 ms                                                          | 99.9 ms: 1.18x faster                                                                     |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 501 ms: 1.84x faster                                                                      |
| async_tree_none         | 394 ms                                                          | 256 ms: 1.54x faster                                                                      |
| async_tree_io           | 940 ms                                                          | 614 ms: 1.53x faster                                                                      |
| async_tree_memoization  | 467 ms                                                          | 320 ms: 1.46x faster                                                                      |
| Geometric mean          | (ref)                                                           | 1.59x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 199 ms: 2.52x faster                                                                      |
| float          | 69.6 ms                                                         | 56.6 ms: 1.23x faster                                                                     |
| nbody          | 79.1 ms                                                         | 82.3 ms: 1.04x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.44x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 107 ms: 1.09x faster                                                                      |
| regex_dna      | 131 ms                                                          | 120 ms: 1.08x faster                                                                      |
| regex_v8       | 15.8 ms                                                         | 16.3 ms: 1.03x slower                                                                     |
| regex_effbot   | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.00x slower                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.84 ms: 1.44x faster                                                                     |
| pickle_pure_python   | 280 us                                                          | 211 us: 1.33x faster                                                                      |
| unpickle_pure_python | 189 us                                                          | 150 us: 1.26x faster                                                                      |
| xml_etree_process    | 48.1 ms                                                         | 41.1 ms: 1.17x faster                                                                     |
| tomli_loads          | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                                                    |
| json_loads           | 22.4 us                                                         | 20.2 us: 1.11x faster                                                                     |
| xml_etree_parse      | 120 ms                                                          | 112 ms: 1.08x faster                                                                      |
| xml_etree_generate   | 61.6 ms                                                         | 60.3 ms: 1.02x faster                                                                     |
| unpickle             | 9.82 us                                                         | 9.62 us: 1.02x faster                                                                     |
| xml_etree_iterparse  | 70.8 ms                                                         | 69.9 ms: 1.01x faster                                                                     |
| pickle               | 7.83 us                                                         | 7.88 us: 1.01x slower                                                                     |
| unpickle_list        | 2.98 us                                                         | 3.01 us: 1.01x slower                                                                     |
| pickle_list          | 3.22 us                                                         | 3.52 us: 1.09x slower                                                                     |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup_no_site | 18.1 ms                                                         | 20.7 ms: 1.15x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                              |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.73 ms: 1.18x faster                                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 93.4 us: 4.24x faster                                                                     |
| pidigits                 | 502 ms                                                          | 199 ms: 2.52x faster                                                                      |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 501 ms: 1.84x faster                                                                      |
| logging_silent           | 97.9 ns                                                         | 60.6 ns: 1.62x faster                                                                     |
| async_tree_none          | 394 ms                                                          | 256 ms: 1.54x faster                                                                      |
| async_tree_io            | 940 ms                                                          | 614 ms: 1.53x faster                                                                      |
| deltablue                | 4.04 ms                                                         | 2.68 ms: 1.51x faster                                                                     |
| raytrace                 | 303 ms                                                          | 203 ms: 1.49x faster                                                                      |
| async_tree_memoization   | 467 ms                                                          | 320 ms: 1.46x faster                                                                      |
| richards_super           | 49.9 ms                                                         | 34.7 ms: 1.44x faster                                                                     |
| json_dumps               | 9.82 ms                                                         | 6.84 ms: 1.44x faster                                                                     |
| scimark_lu               | 89.8 ms                                                         | 62.7 ms: 1.43x faster                                                                     |
| sqlglot_parse            | 1.33 ms                                                         | 935 us: 1.42x faster                                                                      |
| scimark_sor              | 115 ms                                                          | 81.5 ms: 1.41x faster                                                                     |
| chaos                    | 74.4 ms                                                         | 53.6 ms: 1.39x faster                                                                     |
| go                       | 146 ms                                                          | 107 ms: 1.36x faster                                                                      |
| crypto_pyaes             | 81.3 ms                                                         | 59.7 ms: 1.36x faster                                                                     |
| generators               | 31.6 ms                                                         | 23.3 ms: 1.35x faster                                                                     |
| sqlglot_transpile        | 1.58 ms                                                         | 1.17 ms: 1.35x faster                                                                     |
| comprehensions           | 17.7 us                                                         | 13.3 us: 1.34x faster                                                                     |
| richards                 | 40.3 ms                                                         | 30.3 ms: 1.33x faster                                                                     |
| pickle_pure_python       | 280 us                                                          | 211 us: 1.33x faster                                                                      |
| unpickle_pure_python     | 189 us                                                          | 150 us: 1.26x faster                                                                      |
| pyflate                  | 422 ms                                                          | 335 ms: 1.26x faster                                                                      |
| coroutines               | 17.9 ms                                                         | 14.4 ms: 1.24x faster                                                                     |
| sqlite_synth             | 2.29 us                                                         | 1.85 us: 1.24x faster                                                                     |
| float                    | 69.6 ms                                                         | 56.6 ms: 1.23x faster                                                                     |
| deepcopy_memo            | 29.6 us                                                         | 24.3 us: 1.22x faster                                                                     |
| scimark_monte_carlo      | 61.9 ms                                                         | 50.9 ms: 1.22x faster                                                                     |
| pycparser                | 1.04 sec                                                        | 857 ms: 1.22x faster                                                                      |
| hexiom                   | 6.13 ms                                                         | 5.08 ms: 1.21x faster                                                                     |
| asyncio_tcp              | 744 ms                                                          | 622 ms: 1.20x faster                                                                      |
| mako                     | 9.10 ms                                                         | 7.73 ms: 1.18x faster                                                                     |
| tornado_http             | 118 ms                                                          | 99.9 ms: 1.18x faster                                                                     |
| json                     | 4.76 ms                                                         | 4.06 ms: 1.17x faster                                                                     |
| xml_etree_process        | 48.1 ms                                                         | 41.1 ms: 1.17x faster                                                                     |
| deepcopy                 | 310 us                                                          | 266 us: 1.16x faster                                                                      |
| deepcopy_reduce          | 2.68 us                                                         | 2.33 us: 1.15x faster                                                                     |
| tomli_loads              | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                                                    |
| nqueens                  | 87.1 ms                                                         | 77.0 ms: 1.13x faster                                                                     |
| sympy_sum                | 122 ms                                                          | 109 ms: 1.12x faster                                                                      |
| chameleon                | 6.42 ms                                                         | 5.72 ms: 1.12x faster                                                                     |
| pprint_pformat           | 1.37 sec                                                        | 1.22 sec: 1.12x faster                                                                    |
| mdp                      | 1.83 sec                                                        | 1.64 sec: 1.11x faster                                                                    |
| json_loads               | 22.4 us                                                         | 20.2 us: 1.11x faster                                                                     |
| pprint_safe_repr         | 658 ms                                                          | 600 ms: 1.10x faster                                                                      |
| fannkuch                 | 317 ms                                                          | 289 ms: 1.10x faster                                                                      |
| sympy_str                | 229 ms                                                          | 209 ms: 1.09x faster                                                                      |
| dask                     | 341 ms                                                          | 312 ms: 1.09x faster                                                                      |
| regex_compile            | 117 ms                                                          | 107 ms: 1.09x faster                                                                      |
| regex_dna                | 131 ms                                                          | 120 ms: 1.08x faster                                                                      |
| sqlglot_normalize        | 230 ms                                                          | 214 ms: 1.08x faster                                                                      |
| sympy_integrate          | 16.6 ms                                                         | 15.5 ms: 1.08x faster                                                                     |
| xml_etree_parse          | 120 ms                                                          | 112 ms: 1.08x faster                                                                      |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.07x faster                                                                    |
| sqlglot_optimize         | 44.7 ms                                                         | 41.8 ms: 1.07x faster                                                                     |
| sympy_expand             | 391 ms                                                          | 366 ms: 1.07x faster                                                                      |
| create_gc_cycles         | 694 us                                                          | 653 us: 1.06x faster                                                                      |
| 2to3                     | 265 ms                                                          | 252 ms: 1.05x faster                                                                      |
| bench_thread_pool        | 1.12 ms                                                         | 1.09 ms: 1.03x faster                                                                     |
| spectral_norm            | 80.2 ms                                                         | 78.2 ms: 1.03x faster                                                                     |
| xml_etree_generate       | 61.6 ms                                                         | 60.3 ms: 1.02x faster                                                                     |
| unpickle                 | 9.82 us                                                         | 9.62 us: 1.02x faster                                                                     |
| scimark_fft              | 216 ms                                                          | 212 ms: 1.02x faster                                                                      |
| xml_etree_iterparse      | 70.8 ms                                                         | 69.9 ms: 1.01x faster                                                                     |
| meteor_contest           | 80.0 ms                                                         | 79.3 ms: 1.01x faster                                                                     |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.26 ms: 1.01x slower                                                                     |
| pickle                   | 7.83 us                                                         | 7.88 us: 1.01x slower                                                                     |
| unpickle_list            | 2.98 us                                                         | 3.01 us: 1.01x slower                                                                     |
| regex_v8                 | 15.8 ms                                                         | 16.3 ms: 1.03x slower                                                                     |
| nbody                    | 79.1 ms                                                         | 82.3 ms: 1.04x slower                                                                     |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                                    |
| pickle_list              | 3.22 us                                                         | 3.52 us: 1.09x slower                                                                     |
| logging_format           | 7.91 us                                                         | 8.66 us: 1.09x slower                                                                     |
| pathlib                  | 81.2 ms                                                         | 89.2 ms: 1.10x slower                                                                     |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                                                     |
| gc_traversal             | 1.28 ms                                                         | 1.42 ms: 1.11x slower                                                                     |
| logging_simple           | 7.29 us                                                         | 8.12 us: 1.11x slower                                                                     |
| bench_mp_pool            | 66.4 ms                                                         | 75.3 ms: 1.14x slower                                                                     |
| regex_effbot             | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                                     |
| python_startup_no_site   | 18.1 ms                                                         | 20.7 ms: 1.15x slower                                                                     |
| unpack_sequence          | 40.0 ns                                                         | 46.1 ns: 1.15x slower                                                                     |
| async_generators         | 241 ms                                                          | 283 ms: 1.17x slower                                                                      |
| telco                    | 4.83 ms                                                         | 5.92 ms: 1.23x slower                                                                     |
| coverage                 | 46.6 ms                                                         | 461 ms: 9.91x slower                                                                      |
| Geometric mean           | (ref)                                                           | 1.13x faster                                                                              |

Benchmark hidden because not significant (1): python_startup
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240129-3.13.0a3+-fcdc84c-PYTHON_UOPS/bm-20240129-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown