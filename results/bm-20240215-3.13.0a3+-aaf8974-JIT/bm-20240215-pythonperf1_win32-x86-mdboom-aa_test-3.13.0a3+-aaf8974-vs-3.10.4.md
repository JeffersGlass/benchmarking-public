
# Results vs. 3.10.4

- fork: mdboom
- ref: aa_test
- machine: windows-x86
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 252 ms: 1.05x faster                                               |
| chameleon      | 6.42 ms                                                         | 5.83 ms: 1.10x faster                                              |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                             |
| tornado_http   | 118 ms                                                          | 98.6 ms: 1.19x faster                                              |
| Geometric mean | (ref)                                                           | 1.10x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 517 ms: 1.78x faster                                               |
| async_tree_none         | 394 ms                                                          | 255 ms: 1.54x faster                                               |
| async_tree_io           | 940 ms                                                          | 615 ms: 1.53x faster                                               |
| async_tree_memoization  | 467 ms                                                          | 317 ms: 1.47x faster                                               |
| Geometric mean          | (ref)                                                           | 1.58x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 199 ms: 2.52x faster                                               |
| float          | 69.6 ms                                                         | 54.0 ms: 1.29x faster                                              |
| nbody          | 79.1 ms                                                         | 88.6 ms: 1.12x slower                                              |
| Geometric mean | (ref)                                                           | 1.43x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 108 ms: 1.08x faster                                               |
| regex_dna      | 131 ms                                                          | 122 ms: 1.07x faster                                               |
| regex_v8       | 15.8 ms                                                         | 15.8 ms: 1.01x slower                                              |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.13x slower                                              |
| Geometric mean | (ref)                                                           | 1.00x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.96 ms: 1.41x faster                                              |
| pickle_pure_python   | 280 us                                                          | 222 us: 1.26x faster                                               |
| unpickle_pure_python | 189 us                                                          | 158 us: 1.20x faster                                               |
| tomli_loads          | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                             |
| xml_etree_process    | 48.1 ms                                                         | 42.6 ms: 1.13x faster                                              |
| json_loads           | 22.4 us                                                         | 20.0 us: 1.12x faster                                              |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                               |
| xml_etree_iterparse  | 70.8 ms                                                         | 66.6 ms: 1.06x faster                                              |
| pickle_list          | 3.22 us                                                         | 3.18 us: 1.01x faster                                              |
| xml_etree_generate   | 61.6 ms                                                         | 61.1 ms: 1.01x faster                                              |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.03x slower                                              |
| pickle               | 7.83 us                                                         | 8.07 us: 1.03x slower                                              |
| unpickle_list        | 2.98 us                                                         | 3.13 us: 1.05x slower                                              |
| pickle_dict          | 18.2 us                                                         | 20.0 us: 1.10x slower                                              |
| Geometric mean       | (ref)                                                           | 1.08x faster                                                       |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup_no_site | 18.1 ms                                                         | 20.8 ms: 1.15x slower                                              |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                       |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.44 ms: 1.22x faster                                              |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:---------------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 98.6 us: 4.01x faster                                              |
| pidigits                 | 502 ms                                                          | 199 ms: 2.52x faster                                               |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 517 ms: 1.78x faster                                               |
| deltablue                | 4.04 ms                                                         | 2.55 ms: 1.58x faster                                              |
| async_tree_none          | 394 ms                                                          | 255 ms: 1.54x faster                                               |
| async_tree_io            | 940 ms                                                          | 615 ms: 1.53x faster                                               |
| async_tree_memoization   | 467 ms                                                          | 317 ms: 1.47x faster                                               |
| logging_silent           | 97.9 ns                                                         | 67.8 ns: 1.44x faster                                              |
| json_dumps               | 9.82 ms                                                         | 6.96 ms: 1.41x faster                                              |
| richards_super           | 49.9 ms                                                         | 35.5 ms: 1.41x faster                                              |
| sqlglot_parse            | 1.33 ms                                                         | 961 us: 1.38x faster                                               |
| crypto_pyaes             | 81.3 ms                                                         | 61.4 ms: 1.32x faster                                              |
| scimark_lu               | 89.8 ms                                                         | 68.2 ms: 1.32x faster                                              |
| richards                 | 40.3 ms                                                         | 30.9 ms: 1.30x faster                                              |
| scimark_sor              | 115 ms                                                          | 88.3 ms: 1.30x faster                                              |
| sqlglot_transpile        | 1.58 ms                                                         | 1.21 ms: 1.30x faster                                              |
| float                    | 69.6 ms                                                         | 54.0 ms: 1.29x faster                                              |
| generators               | 31.6 ms                                                         | 24.5 ms: 1.29x faster                                              |
| raytrace                 | 303 ms                                                          | 238 ms: 1.27x faster                                               |
| pickle_pure_python       | 280 us                                                          | 222 us: 1.26x faster                                               |
| comprehensions           | 17.7 us                                                         | 14.1 us: 1.26x faster                                              |
| chaos                    | 74.4 ms                                                         | 60.2 ms: 1.24x faster                                              |
| mako                     | 9.10 ms                                                         | 7.44 ms: 1.22x faster                                              |
| sqlite_synth             | 2.29 us                                                         | 1.87 us: 1.22x faster                                              |
| go                       | 146 ms                                                          | 120 ms: 1.22x faster                                               |
| coroutines               | 17.9 ms                                                         | 14.8 ms: 1.21x faster                                              |
| asyncio_tcp              | 744 ms                                                          | 615 ms: 1.21x faster                                               |
| unpickle_pure_python     | 189 us                                                          | 158 us: 1.20x faster                                               |
| pycparser                | 1.04 sec                                                        | 872 ms: 1.19x faster                                               |
| tornado_http             | 118 ms                                                          | 98.6 ms: 1.19x faster                                              |
| deepcopy_memo            | 29.6 us                                                         | 25.7 us: 1.15x faster                                              |
| tomli_loads              | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                             |
| json                     | 4.76 ms                                                         | 4.19 ms: 1.14x faster                                              |
| xml_etree_process        | 48.1 ms                                                         | 42.6 ms: 1.13x faster                                              |
| dask                     | 341 ms                                                          | 305 ms: 1.12x faster                                               |
| json_loads               | 22.4 us                                                         | 20.0 us: 1.12x faster                                              |
| pyflate                  | 422 ms                                                          | 379 ms: 1.11x faster                                               |
| sympy_sum                | 122 ms                                                          | 110 ms: 1.11x faster                                               |
| deepcopy_reduce          | 2.68 us                                                         | 2.43 us: 1.11x faster                                              |
| bench_thread_pool        | 1.12 ms                                                         | 1.01 ms: 1.11x faster                                              |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                               |
| chameleon                | 6.42 ms                                                         | 5.83 ms: 1.10x faster                                              |
| deepcopy                 | 310 us                                                          | 286 us: 1.08x faster                                               |
| spectral_norm            | 80.2 ms                                                         | 74.1 ms: 1.08x faster                                              |
| regex_compile            | 117 ms                                                          | 108 ms: 1.08x faster                                               |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                             |
| regex_dna                | 131 ms                                                          | 122 ms: 1.07x faster                                               |
| create_gc_cycles         | 694 us                                                          | 652 us: 1.06x faster                                               |
| xml_etree_iterparse      | 70.8 ms                                                         | 66.6 ms: 1.06x faster                                              |
| sympy_str                | 229 ms                                                          | 216 ms: 1.06x faster                                               |
| sympy_integrate          | 16.6 ms                                                         | 15.7 ms: 1.06x faster                                              |
| 2to3                     | 265 ms                                                          | 252 ms: 1.05x faster                                               |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.11 ms: 1.04x faster                                              |
| sqlglot_normalize        | 230 ms                                                          | 221 ms: 1.04x faster                                               |
| sympy_expand             | 391 ms                                                          | 379 ms: 1.03x faster                                               |
| sqlglot_optimize         | 44.7 ms                                                         | 43.5 ms: 1.03x faster                                              |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.7 sec: 1.02x faster                                             |
| pickle_list              | 3.22 us                                                         | 3.18 us: 1.01x faster                                              |
| xml_etree_generate       | 61.6 ms                                                         | 61.1 ms: 1.01x faster                                              |
| fannkuch                 | 317 ms                                                          | 315 ms: 1.01x faster                                               |
| regex_v8                 | 15.8 ms                                                         | 15.8 ms: 1.01x slower                                              |
| nqueens                  | 87.1 ms                                                         | 87.8 ms: 1.01x slower                                              |
| mdp                      | 1.83 sec                                                        | 1.84 sec: 1.01x slower                                             |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.03x slower                                              |
| pathlib                  | 81.2 ms                                                         | 83.6 ms: 1.03x slower                                              |
| pickle                   | 7.83 us                                                         | 8.07 us: 1.03x slower                                              |
| unpickle_list            | 2.98 us                                                         | 3.13 us: 1.05x slower                                              |
| pprint_pformat           | 1.37 sec                                                        | 1.43 sec: 1.05x slower                                             |
| meteor_contest           | 80.0 ms                                                         | 84.6 ms: 1.06x slower                                              |
| pprint_safe_repr         | 658 ms                                                          | 700 ms: 1.06x slower                                               |
| hexiom                   | 6.13 ms                                                         | 6.54 ms: 1.07x slower                                              |
| gc_traversal             | 1.28 ms                                                         | 1.38 ms: 1.08x slower                                              |
| pickle_dict              | 18.2 us                                                         | 20.0 us: 1.10x slower                                              |
| scimark_fft              | 216 ms                                                          | 241 ms: 1.11x slower                                               |
| scimark_monte_carlo      | 61.9 ms                                                         | 69.3 ms: 1.12x slower                                              |
| nbody                    | 79.1 ms                                                         | 88.6 ms: 1.12x slower                                              |
| bench_mp_pool            | 66.4 ms                                                         | 74.7 ms: 1.13x slower                                              |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.13x slower                                              |
| logging_format           | 7.91 us                                                         | 9.07 us: 1.15x slower                                              |
| python_startup_no_site   | 18.1 ms                                                         | 20.8 ms: 1.15x slower                                              |
| logging_simple           | 7.29 us                                                         | 8.42 us: 1.15x slower                                              |
| unpack_sequence          | 40.0 ns                                                         | 46.5 ns: 1.16x slower                                              |
| async_generators         | 241 ms                                                          | 291 ms: 1.21x slower                                               |
| telco                    | 4.83 ms                                                         | 6.35 ms: 1.31x slower                                              |
| coverage                 | 46.6 ms                                                         | 474 ms: 10.18x slower                                              |
| Geometric mean           | (ref)                                                           | 1.10x faster                                                       |

Benchmark hidden because not significant (1): python_startup
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-aaf8974-JIT/bm-20240215-pythonperf1_win32-x86-mdboom-aa_test-3.13.0a3+-aaf8974.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown