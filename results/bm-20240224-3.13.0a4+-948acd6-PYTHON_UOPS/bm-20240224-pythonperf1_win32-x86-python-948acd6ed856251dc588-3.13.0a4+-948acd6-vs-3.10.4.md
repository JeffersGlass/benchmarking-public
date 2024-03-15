
# Results vs. 3.10.4

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-x86
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.12x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 246 ms: 1.08x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.94 ms: 1.08x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.84 sec: 1.06x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.4 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 504 ms: 1.83x faster                                                            |
| async_tree_none         | 394 ms                                                          | 248 ms: 1.59x faster                                                            |
| async_tree_io           | 940 ms                                                          | 600 ms: 1.57x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 311 ms: 1.50x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.62x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| float          | 69.6 ms                                                         | 61.6 ms: 1.13x faster                                                           |
| nbody          | 79.1 ms                                                         | 80.8 ms: 1.02x slower                                                           |
| Geometric mean | (ref)                                                           | 1.41x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 119 ms: 1.10x faster                                                            |
| regex_compile  | 117 ms                                                          | 121 ms: 1.04x slower                                                            |
| regex_v8       | 15.8 ms                                                         | 16.4 ms: 1.04x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.87 ms: 1.43x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 216 us: 1.30x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.66 sec: 1.15x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 42.4 ms: 1.13x faster                                                           |
| json_loads           | 22.4 us                                                         | 19.8 us: 1.13x faster                                                           |
| unpickle_pure_python | 189 us                                                          | 171 us: 1.11x faster                                                            |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| unpickle_list        | 2.98 us                                                         | 2.81 us: 1.06x faster                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.1 ms: 1.04x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 59.8 ms: 1.03x faster                                                           |
| pickle               | 7.83 us                                                         | 7.77 us: 1.01x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.27 us: 1.02x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.2 us: 1.11x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                    |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.1 ms: 1.04x faster                                                           |
| python_startup_no_site | 18.1 ms                                                         | 19.9 ms: 1.10x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.03x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.65 ms: 1.19x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 94.3 us: 4.20x faster                                                           |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 504 ms: 1.83x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.43 ms: 1.66x faster                                                           |
| logging_silent           | 97.9 ns                                                         | 61.6 ns: 1.59x faster                                                           |
| async_tree_none          | 394 ms                                                          | 248 ms: 1.59x faster                                                            |
| async_tree_io            | 940 ms                                                          | 600 ms: 1.57x faster                                                            |
| richards_super           | 49.9 ms                                                         | 33.2 ms: 1.50x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 311 ms: 1.50x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 55.4 ms: 1.47x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.87 ms: 1.43x faster                                                           |
| chaos                    | 74.4 ms                                                         | 52.2 ms: 1.43x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 948 us: 1.40x faster                                                            |
| richards                 | 40.3 ms                                                         | 29.6 ms: 1.36x faster                                                           |
| generators               | 31.6 ms                                                         | 23.2 ms: 1.36x faster                                                           |
| raytrace                 | 303 ms                                                          | 229 ms: 1.32x faster                                                            |
| sqlglot_transpile        | 1.58 ms                                                         | 1.20 ms: 1.32x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 216 us: 1.30x faster                                                            |
| go                       | 146 ms                                                          | 116 ms: 1.26x faster                                                            |
| comprehensions           | 17.7 us                                                         | 14.4 us: 1.23x faster                                                           |
| scimark_sor              | 115 ms                                                          | 93.9 ms: 1.23x faster                                                           |
| pyflate                  | 422 ms                                                          | 348 ms: 1.21x faster                                                            |
| tornado_http             | 118 ms                                                          | 97.4 ms: 1.21x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.9 ms: 1.21x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 624 ms: 1.19x faster                                                            |
| mako                     | 9.10 ms                                                         | 7.65 ms: 1.19x faster                                                           |
| pycparser                | 1.04 sec                                                        | 879 ms: 1.19x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 25.0 us: 1.18x faster                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 52.5 ms: 1.18x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.66 sec: 1.15x faster                                                          |
| fannkuch                 | 317 ms                                                          | 277 ms: 1.15x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 2.00 us: 1.14x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 42.4 ms: 1.13x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 79.3 ms: 1.13x faster                                                           |
| json_loads               | 22.4 us                                                         | 19.8 us: 1.13x faster                                                           |
| float                    | 69.6 ms                                                         | 61.6 ms: 1.13x faster                                                           |
| json                     | 4.76 ms                                                         | 4.25 ms: 1.12x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 171 us: 1.11x faster                                                            |
| sympy_sum                | 122 ms                                                          | 111 ms: 1.10x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.66 sec: 1.10x faster                                                          |
| regex_dna                | 131 ms                                                          | 119 ms: 1.10x faster                                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.25 sec: 1.10x faster                                                          |
| deepcopy                 | 310 us                                                          | 285 us: 1.09x faster                                                            |
| nqueens                  | 87.1 ms                                                         | 80.1 ms: 1.09x faster                                                           |
| pprint_safe_repr         | 658 ms                                                          | 608 ms: 1.08x faster                                                            |
| chameleon                | 6.42 ms                                                         | 5.94 ms: 1.08x faster                                                           |
| 2to3                     | 265 ms                                                          | 246 ms: 1.08x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.04 ms: 1.08x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.50 us: 1.07x faster                                                           |
| unpickle_list            | 2.98 us                                                         | 2.81 us: 1.06x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 5.80 ms: 1.06x faster                                                           |
| docutils                 | 1.95 sec                                                        | 1.84 sec: 1.06x faster                                                          |
| create_gc_cycles         | 694 us                                                          | 658 us: 1.06x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.8 ms: 1.05x faster                                                           |
| sympy_str                | 229 ms                                                          | 218 ms: 1.05x faster                                                            |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.10 ms: 1.04x faster                                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.1 ms: 1.04x faster                                                           |
| python_startup           | 22.9 ms                                                         | 22.1 ms: 1.04x faster                                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 43.3 ms: 1.03x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 59.8 ms: 1.03x faster                                                           |
| sqlglot_normalize        | 230 ms                                                          | 225 ms: 1.03x faster                                                            |
| spectral_norm            | 80.2 ms                                                         | 78.4 ms: 1.02x faster                                                           |
| scimark_fft              | 216 ms                                                          | 212 ms: 1.02x faster                                                            |
| sympy_expand             | 391 ms                                                          | 383 ms: 1.02x faster                                                            |
| pickle                   | 7.83 us                                                         | 7.77 us: 1.01x faster                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.9 sec: 1.01x faster                                                          |
| meteor_contest           | 80.0 ms                                                         | 80.7 ms: 1.01x slower                                                           |
| pickle_list              | 3.22 us                                                         | 3.27 us: 1.02x slower                                                           |
| nbody                    | 79.1 ms                                                         | 80.8 ms: 1.02x slower                                                           |
| regex_compile            | 117 ms                                                          | 121 ms: 1.04x slower                                                            |
| regex_v8                 | 15.8 ms                                                         | 16.4 ms: 1.04x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 70.1 ms: 1.06x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 85.8 ms: 1.06x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.59 us: 1.09x slower                                                           |
| logging_simple           | 7.29 us                                                         | 8.02 us: 1.10x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.41 ms: 1.10x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 19.9 ms: 1.10x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.2 us: 1.11x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| async_generators         | 241 ms                                                          | 280 ms: 1.16x slower                                                            |
| telco                    | 4.83 ms                                                         | 6.08 ms: 1.26x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 50.7 ns: 1.27x slower                                                           |
| coverage                 | 46.6 ms                                                         | 470 ms: 10.09x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.12x faster                                                                    |

Benchmark hidden because not significant (1): unpickle
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1_win32-x86-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown