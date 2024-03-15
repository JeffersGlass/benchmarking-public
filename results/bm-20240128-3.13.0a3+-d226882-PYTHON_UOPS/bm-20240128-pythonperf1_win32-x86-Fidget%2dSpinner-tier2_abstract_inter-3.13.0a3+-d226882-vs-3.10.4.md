
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-x86
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.12x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 250 ms: 1.06x faster                                                                      |
| chameleon      | 6.42 ms                                                         | 5.82 ms: 1.10x faster                                                                     |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                                    |
| tornado_http   | 118 ms                                                          | 98.8 ms: 1.19x faster                                                                     |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 521 ms: 1.77x faster                                                                      |
| async_tree_none         | 394 ms                                                          | 255 ms: 1.54x faster                                                                      |
| async_tree_io           | 940 ms                                                          | 620 ms: 1.52x faster                                                                      |
| async_tree_memoization  | 467 ms                                                          | 316 ms: 1.48x faster                                                                      |
| Geometric mean          | (ref)                                                           | 1.57x faster                                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 204 ms: 2.47x faster                                                                      |
| float          | 69.6 ms                                                         | 61.2 ms: 1.14x faster                                                                     |
| nbody          | 79.1 ms                                                         | 87.0 ms: 1.10x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.37x faster                                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 108 ms: 1.08x faster                                                                      |
| regex_dna      | 131 ms                                                          | 123 ms: 1.06x faster                                                                      |
| regex_v8       | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                                     |
| regex_effbot   | 1.66 ms                                                         | 1.92 ms: 1.16x slower                                                                     |
| Geometric mean | (ref)                                                           | 1.01x slower                                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.87 ms: 1.43x faster                                                                     |
| pickle_pure_python   | 280 us                                                          | 209 us: 1.34x faster                                                                      |
| unpickle_pure_python | 189 us                                                          | 153 us: 1.24x faster                                                                      |
| tomli_loads          | 1.91 sec                                                        | 1.65 sec: 1.16x faster                                                                    |
| xml_etree_process    | 48.1 ms                                                         | 42.2 ms: 1.14x faster                                                                     |
| json_loads           | 22.4 us                                                         | 20.0 us: 1.12x faster                                                                     |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                                      |
| xml_etree_generate   | 61.6 ms                                                         | 61.2 ms: 1.01x faster                                                                     |
| pickle               | 7.83 us                                                         | 7.78 us: 1.01x faster                                                                     |
| xml_etree_iterparse  | 70.8 ms                                                         | 70.5 ms: 1.00x faster                                                                     |
| unpickle             | 9.82 us                                                         | 9.90 us: 1.01x slower                                                                     |
| unpickle_list        | 2.98 us                                                         | 3.05 us: 1.02x slower                                                                     |
| pickle_dict          | 18.2 us                                                         | 20.2 us: 1.11x slower                                                                     |
| pickle_list          | 3.22 us                                                         | 3.69 us: 1.15x slower                                                                     |
| Geometric mean       | (ref)                                                           | 1.08x faster                                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.8 ms: 1.04x slower                                                                     |
| python_startup_no_site | 18.1 ms                                                         | 21.5 ms: 1.19x slower                                                                     |
| Geometric mean         | (ref)                                                           | 1.11x slower                                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 8.34 ms: 1.09x faster                                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 95.4 us: 4.15x faster                                                                     |
| pidigits                 | 502 ms                                                          | 204 ms: 2.47x faster                                                                      |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 521 ms: 1.77x faster                                                                      |
| logging_silent           | 97.9 ns                                                         | 60.2 ns: 1.63x faster                                                                     |
| async_tree_none          | 394 ms                                                          | 255 ms: 1.54x faster                                                                      |
| async_tree_io            | 940 ms                                                          | 620 ms: 1.52x faster                                                                      |
| richards_super           | 49.9 ms                                                         | 33.1 ms: 1.51x faster                                                                     |
| sqlglot_parse            | 1.33 ms                                                         | 883 us: 1.51x faster                                                                      |
| async_tree_memoization   | 467 ms                                                          | 316 ms: 1.48x faster                                                                      |
| raytrace                 | 303 ms                                                          | 209 ms: 1.45x faster                                                                      |
| crypto_pyaes             | 81.3 ms                                                         | 56.7 ms: 1.43x faster                                                                     |
| scimark_lu               | 89.8 ms                                                         | 62.6 ms: 1.43x faster                                                                     |
| json_dumps               | 9.82 ms                                                         | 6.87 ms: 1.43x faster                                                                     |
| chaos                    | 74.4 ms                                                         | 52.1 ms: 1.43x faster                                                                     |
| sqlglot_transpile        | 1.58 ms                                                         | 1.13 ms: 1.41x faster                                                                     |
| scimark_sor              | 115 ms                                                          | 82.3 ms: 1.40x faster                                                                     |
| deltablue                | 4.04 ms                                                         | 2.89 ms: 1.40x faster                                                                     |
| go                       | 146 ms                                                          | 106 ms: 1.38x faster                                                                      |
| richards                 | 40.3 ms                                                         | 29.4 ms: 1.37x faster                                                                     |
| generators               | 31.6 ms                                                         | 23.2 ms: 1.36x faster                                                                     |
| pickle_pure_python       | 280 us                                                          | 209 us: 1.34x faster                                                                      |
| comprehensions           | 17.7 us                                                         | 14.0 us: 1.27x faster                                                                     |
| coroutines               | 17.9 ms                                                         | 14.2 ms: 1.26x faster                                                                     |
| pycparser                | 1.04 sec                                                        | 832 ms: 1.25x faster                                                                      |
| unpickle_pure_python     | 189 us                                                          | 153 us: 1.24x faster                                                                      |
| pyflate                  | 422 ms                                                          | 341 ms: 1.24x faster                                                                      |
| deepcopy_memo            | 29.6 us                                                         | 24.6 us: 1.20x faster                                                                     |
| sqlite_synth             | 2.29 us                                                         | 1.90 us: 1.20x faster                                                                     |
| tornado_http             | 118 ms                                                          | 98.8 ms: 1.19x faster                                                                     |
| scimark_monte_carlo      | 61.9 ms                                                         | 52.2 ms: 1.19x faster                                                                     |
| json                     | 4.76 ms                                                         | 4.10 ms: 1.16x faster                                                                     |
| tomli_loads              | 1.91 sec                                                        | 1.65 sec: 1.16x faster                                                                    |
| xml_etree_process        | 48.1 ms                                                         | 42.2 ms: 1.14x faster                                                                     |
| float                    | 69.6 ms                                                         | 61.2 ms: 1.14x faster                                                                     |
| deepcopy                 | 310 us                                                          | 275 us: 1.13x faster                                                                      |
| nqueens                  | 87.1 ms                                                         | 77.5 ms: 1.12x faster                                                                     |
| hexiom                   | 6.13 ms                                                         | 5.47 ms: 1.12x faster                                                                     |
| deepcopy_reduce          | 2.68 us                                                         | 2.39 us: 1.12x faster                                                                     |
| json_loads               | 22.4 us                                                         | 20.0 us: 1.12x faster                                                                     |
| sympy_sum                | 122 ms                                                          | 110 ms: 1.11x faster                                                                      |
| dask                     | 341 ms                                                          | 308 ms: 1.11x faster                                                                      |
| mdp                      | 1.83 sec                                                        | 1.65 sec: 1.11x faster                                                                    |
| chameleon                | 6.42 ms                                                         | 5.82 ms: 1.10x faster                                                                     |
| fannkuch                 | 317 ms                                                          | 288 ms: 1.10x faster                                                                      |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                                      |
| asyncio_tcp              | 744 ms                                                          | 680 ms: 1.09x faster                                                                      |
| mako                     | 9.10 ms                                                         | 8.34 ms: 1.09x faster                                                                     |
| pprint_pformat           | 1.37 sec                                                        | 1.26 sec: 1.08x faster                                                                    |
| sqlglot_normalize        | 230 ms                                                          | 213 ms: 1.08x faster                                                                      |
| regex_compile            | 117 ms                                                          | 108 ms: 1.08x faster                                                                      |
| sympy_integrate          | 16.6 ms                                                         | 15.4 ms: 1.08x faster                                                                     |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                                    |
| sqlglot_optimize         | 44.7 ms                                                         | 41.7 ms: 1.07x faster                                                                     |
| sympy_str                | 229 ms                                                          | 214 ms: 1.07x faster                                                                      |
| 2to3                     | 265 ms                                                          | 250 ms: 1.06x faster                                                                      |
| regex_dna                | 131 ms                                                          | 123 ms: 1.06x faster                                                                      |
| sympy_expand             | 391 ms                                                          | 369 ms: 1.06x faster                                                                      |
| pprint_safe_repr         | 658 ms                                                          | 622 ms: 1.06x faster                                                                      |
| bench_thread_pool        | 1.12 ms                                                         | 1.08 ms: 1.04x faster                                                                     |
| create_gc_cycles         | 694 us                                                          | 671 us: 1.03x faster                                                                      |
| xml_etree_generate       | 61.6 ms                                                         | 61.2 ms: 1.01x faster                                                                     |
| pickle                   | 7.83 us                                                         | 7.78 us: 1.01x faster                                                                     |
| xml_etree_iterparse      | 70.8 ms                                                         | 70.5 ms: 1.00x faster                                                                     |
| unpickle                 | 9.82 us                                                         | 9.90 us: 1.01x slower                                                                     |
| unpickle_list            | 2.98 us                                                         | 3.05 us: 1.02x slower                                                                     |
| regex_v8                 | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                                     |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.5 sec: 1.03x slower                                                                    |
| unpack_sequence          | 40.0 ns                                                         | 41.4 ns: 1.04x slower                                                                     |
| python_startup           | 22.9 ms                                                         | 23.8 ms: 1.04x slower                                                                     |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.37 ms: 1.04x slower                                                                     |
| spectral_norm            | 80.2 ms                                                         | 85.0 ms: 1.06x slower                                                                     |
| gc_traversal             | 1.28 ms                                                         | 1.40 ms: 1.09x slower                                                                     |
| nbody                    | 79.1 ms                                                         | 87.0 ms: 1.10x slower                                                                     |
| pathlib                  | 81.2 ms                                                         | 89.5 ms: 1.10x slower                                                                     |
| logging_format           | 7.91 us                                                         | 8.72 us: 1.10x slower                                                                     |
| pickle_dict              | 18.2 us                                                         | 20.2 us: 1.11x slower                                                                     |
| bench_mp_pool            | 66.4 ms                                                         | 74.6 ms: 1.12x slower                                                                     |
| logging_simple           | 7.29 us                                                         | 8.28 us: 1.14x slower                                                                     |
| async_generators         | 241 ms                                                          | 275 ms: 1.14x slower                                                                      |
| pickle_list              | 3.22 us                                                         | 3.69 us: 1.15x slower                                                                     |
| regex_effbot             | 1.66 ms                                                         | 1.92 ms: 1.16x slower                                                                     |
| telco                    | 4.83 ms                                                         | 5.75 ms: 1.19x slower                                                                     |
| python_startup_no_site   | 18.1 ms                                                         | 21.5 ms: 1.19x slower                                                                     |
| coverage                 | 46.6 ms                                                         | 505 ms: 10.85x slower                                                                     |
| Geometric mean           | (ref)                                                           | 1.12x faster                                                                              |

Benchmark hidden because not significant (2): meteor_contest, scimark_fft
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240128-3.13.0a3+-d226882-PYTHON_UOPS/bm-20240128-pythonperf1_win32-x86-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown