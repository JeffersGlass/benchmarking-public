
# Results vs. 3.10.4

- fork: python
- ref: 384429d1c0cf011dcf88
- machine: windows-x86
- commit hash: 384429d
- commit date: 2024-01-24
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 246 ms: 1.08x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.79 ms: 1.11x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.84 sec: 1.06x faster                                                          |
| tornado_http   | 118 ms                                                          | 99.1 ms: 1.19x faster                                                           |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 511 ms: 1.81x faster                                                            |
| async_tree_none         | 394 ms                                                          | 261 ms: 1.51x faster                                                            |
| async_tree_io           | 940 ms                                                          | 628 ms: 1.50x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 328 ms: 1.42x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.55x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 200 ms: 2.52x faster                                                            |
| float          | 69.6 ms                                                         | 59.3 ms: 1.17x faster                                                           |
| nbody          | 79.1 ms                                                         | 88.5 ms: 1.12x slower                                                           |
| Geometric mean | (ref)                                                           | 1.38x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 119 ms: 1.10x faster                                                            |
| regex_compile  | 117 ms                                                          | 107 ms: 1.09x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.01x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.51 ms: 1.51x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 208 us: 1.34x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 150 us: 1.26x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 42.2 ms: 1.14x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.68 sec: 1.14x faster                                                          |
| json_loads           | 22.4 us                                                         | 19.7 us: 1.13x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 113 ms: 1.06x faster                                                            |
| unpickle             | 9.82 us                                                         | 9.57 us: 1.03x faster                                                           |
| pickle               | 7.83 us                                                         | 7.74 us: 1.01x faster                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 71.1 ms: 1.00x slower                                                           |
| unpickle_list        | 2.98 us                                                         | 3.07 us: 1.03x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 19.8 us: 1.09x slower                                                           |
| pickle_list          | 3.22 us                                                         | 3.74 us: 1.16x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                    |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.2 ms: 1.01x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.7 ms: 1.15x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 8.03 ms: 1.13x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 93.5 us: 4.23x faster                                                           |
| pidigits                 | 502 ms                                                          | 200 ms: 2.52x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 511 ms: 1.81x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 61.8 ns: 1.58x faster                                                           |
| richards_super           | 49.9 ms                                                         | 33.0 ms: 1.51x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.51 ms: 1.51x faster                                                           |
| async_tree_none          | 394 ms                                                          | 261 ms: 1.51x faster                                                            |
| async_tree_io            | 940 ms                                                          | 628 ms: 1.50x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 910 us: 1.46x faster                                                            |
| raytrace                 | 303 ms                                                          | 210 ms: 1.44x faster                                                            |
| scimark_lu               | 89.8 ms                                                         | 62.3 ms: 1.44x faster                                                           |
| deltablue                | 4.04 ms                                                         | 2.80 ms: 1.44x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 328 ms: 1.42x faster                                                            |
| scimark_sor              | 115 ms                                                          | 81.0 ms: 1.42x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 57.7 ms: 1.41x faster                                                           |
| chaos                    | 74.4 ms                                                         | 53.0 ms: 1.40x faster                                                           |
| richards                 | 40.3 ms                                                         | 28.9 ms: 1.39x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.15 ms: 1.37x faster                                                           |
| go                       | 146 ms                                                          | 106 ms: 1.37x faster                                                            |
| pickle_pure_python       | 280 us                                                          | 208 us: 1.34x faster                                                            |
| generators               | 31.6 ms                                                         | 23.6 ms: 1.34x faster                                                           |
| comprehensions           | 17.7 us                                                         | 14.0 us: 1.27x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 150 us: 1.26x faster                                                            |
| pycparser                | 1.04 sec                                                        | 839 ms: 1.24x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 1.85 us: 1.24x faster                                                           |
| pyflate                  | 422 ms                                                          | 342 ms: 1.23x faster                                                            |
| coroutines               | 17.9 ms                                                         | 14.5 ms: 1.23x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 24.0 us: 1.23x faster                                                           |
| json                     | 4.76 ms                                                         | 3.98 ms: 1.20x faster                                                           |
| tornado_http             | 118 ms                                                          | 99.1 ms: 1.19x faster                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 52.7 ms: 1.17x faster                                                           |
| float                    | 69.6 ms                                                         | 59.3 ms: 1.17x faster                                                           |
| deepcopy                 | 310 us                                                          | 268 us: 1.16x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.34 us: 1.15x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 42.2 ms: 1.14x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.68 sec: 1.14x faster                                                          |
| json_loads               | 22.4 us                                                         | 19.7 us: 1.13x faster                                                           |
| mako                     | 9.10 ms                                                         | 8.03 ms: 1.13x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 5.41 ms: 1.13x faster                                                           |
| sympy_sum                | 122 ms                                                          | 108 ms: 1.13x faster                                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.22 sec: 1.12x faster                                                          |
| mdp                      | 1.83 sec                                                        | 1.64 sec: 1.11x faster                                                          |
| chameleon                | 6.42 ms                                                         | 5.79 ms: 1.11x faster                                                           |
| pprint_safe_repr         | 658 ms                                                          | 598 ms: 1.10x faster                                                            |
| dask                     | 341 ms                                                          | 311 ms: 1.10x faster                                                            |
| regex_dna                | 131 ms                                                          | 119 ms: 1.10x faster                                                            |
| asyncio_tcp              | 744 ms                                                          | 680 ms: 1.09x faster                                                            |
| regex_compile            | 117 ms                                                          | 107 ms: 1.09x faster                                                            |
| nqueens                  | 87.1 ms                                                         | 79.8 ms: 1.09x faster                                                           |
| sqlglot_normalize        | 230 ms                                                          | 211 ms: 1.09x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 41.1 ms: 1.09x faster                                                           |
| sympy_str                | 229 ms                                                          | 211 ms: 1.08x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.4 ms: 1.08x faster                                                           |
| 2to3                     | 265 ms                                                          | 246 ms: 1.08x faster                                                            |
| sympy_expand             | 391 ms                                                          | 367 ms: 1.06x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 113 ms: 1.06x faster                                                            |
| create_gc_cycles         | 694 us                                                          | 655 us: 1.06x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.84 sec: 1.06x faster                                                          |
| bench_thread_pool        | 1.12 ms                                                         | 1.06 ms: 1.05x faster                                                           |
| unpickle                 | 9.82 us                                                         | 9.57 us: 1.03x faster                                                           |
| pickle                   | 7.83 us                                                         | 7.74 us: 1.01x faster                                                           |
| fannkuch                 | 317 ms                                                          | 314 ms: 1.01x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 71.1 ms: 1.00x slower                                                           |
| python_startup           | 22.9 ms                                                         | 23.2 ms: 1.01x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                           |
| unpickle_list            | 2.98 us                                                         | 3.07 us: 1.03x slower                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.35 ms: 1.03x slower                                                           |
| scimark_fft              | 216 ms                                                          | 225 ms: 1.04x slower                                                            |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.6 sec: 1.04x slower                                                          |
| spectral_norm            | 80.2 ms                                                         | 84.6 ms: 1.05x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 42.6 ns: 1.06x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.8 us: 1.09x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 89.2 ms: 1.10x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 73.0 ms: 1.10x slower                                                           |
| logging_simple           | 7.29 us                                                         | 8.08 us: 1.11x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.77 us: 1.11x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.42 ms: 1.11x slower                                                           |
| nbody                    | 79.1 ms                                                         | 88.5 ms: 1.12x slower                                                           |
| async_generators         | 241 ms                                                          | 273 ms: 1.13x slower                                                            |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.7 ms: 1.15x slower                                                           |
| pickle_list              | 3.22 us                                                         | 3.74 us: 1.16x slower                                                           |
| telco                    | 4.83 ms                                                         | 6.23 ms: 1.29x slower                                                           |
| coverage                 | 46.6 ms                                                         | 477 ms: 10.24x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.13x faster                                                                    |

Benchmark hidden because not significant (2): meteor_contest, xml_etree_generate
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240124-3.13.0a3+-384429d-PYTHON_UOPS/bm-20240124-pythonperf1_win32-x86-python-384429d1c0cf011dcf88-3.13.0a3+-384429d.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown