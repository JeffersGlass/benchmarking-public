
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.07x faster
- HPT reliability: 99.09%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 263 ms: 1.01x faster                                                            |
| docutils       | 1.95 sec                                                        | 1.87 sec: 1.04x faster                                                          |
| tornado_http   | 118 ms                                                          | 101 ms: 1.16x faster                                                            |
| Geometric mean | (ref)                                                           | 1.05x faster                                                                    |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 529 ms: 1.74x faster                                                            |
| async_tree_none         | 394 ms                                                          | 265 ms: 1.49x faster                                                            |
| async_tree_io           | 940 ms                                                          | 640 ms: 1.47x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 333 ms: 1.40x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.52x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 202 ms: 2.49x faster                                                            |
| float          | 69.6 ms                                                         | 56.2 ms: 1.24x faster                                                           |
| nbody          | 79.1 ms                                                         | 93.7 ms: 1.18x slower                                                           |
| Geometric mean | (ref)                                                           | 1.38x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 124 ms: 1.05x faster                                                            |
| regex_compile  | 117 ms                                                          | 114 ms: 1.03x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.92 ms: 1.16x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 7.06 ms: 1.39x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 224 us: 1.25x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 159 us: 1.19x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.69 sec: 1.13x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 42.8 ms: 1.12x faster                                                           |
| json_loads           | 22.4 us                                                         | 20.3 us: 1.10x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 110 ms: 1.09x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 69.4 ms: 1.02x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.26 us: 1.01x slower                                                           |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.03x slower                                                           |
| pickle               | 7.83 us                                                         | 8.16 us: 1.04x slower                                                           |
| unpickle_list        | 2.98 us                                                         | 3.12 us: 1.05x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.07x faster                                                                    |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.3 ms: 1.02x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 21.0 ms: 1.16x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.09x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.84 ms: 1.16x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 99.3 us: 3.99x faster                                                           |
| pidigits                 | 502 ms                                                          | 202 ms: 2.49x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 529 ms: 1.74x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.58 ms: 1.56x faster                                                           |
| async_tree_none          | 394 ms                                                          | 265 ms: 1.49x faster                                                            |
| async_tree_io            | 940 ms                                                          | 640 ms: 1.47x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 67.1 ns: 1.46x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 333 ms: 1.40x faster                                                            |
| json_dumps               | 9.82 ms                                                         | 7.06 ms: 1.39x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 980 us: 1.36x faster                                                            |
| richards_super           | 49.9 ms                                                         | 37.5 ms: 1.33x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 67.6 ms: 1.33x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 61.9 ms: 1.31x faster                                                           |
| generators               | 31.6 ms                                                         | 24.2 ms: 1.31x faster                                                           |
| scimark_sor              | 115 ms                                                          | 88.3 ms: 1.30x faster                                                           |
| raytrace                 | 303 ms                                                          | 237 ms: 1.27x faster                                                            |
| sqlglot_transpile        | 1.58 ms                                                         | 1.25 ms: 1.27x faster                                                           |
| richards                 | 40.3 ms                                                         | 32.1 ms: 1.25x faster                                                           |
| chaos                    | 74.4 ms                                                         | 59.4 ms: 1.25x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 224 us: 1.25x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 1.84 us: 1.25x faster                                                           |
| float                    | 69.6 ms                                                         | 56.2 ms: 1.24x faster                                                           |
| pycparser                | 1.04 sec                                                        | 869 ms: 1.20x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 159 us: 1.19x faster                                                            |
| coroutines               | 17.9 ms                                                         | 15.1 ms: 1.18x faster                                                           |
| go                       | 146 ms                                                          | 124 ms: 1.18x faster                                                            |
| comprehensions           | 17.7 us                                                         | 15.2 us: 1.17x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.84 ms: 1.16x faster                                                           |
| tornado_http             | 118 ms                                                          | 101 ms: 1.16x faster                                                            |
| tomli_loads              | 1.91 sec                                                        | 1.69 sec: 1.13x faster                                                          |
| json                     | 4.76 ms                                                         | 4.22 ms: 1.13x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 26.3 us: 1.13x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 42.8 ms: 1.12x faster                                                           |
| json_loads               | 22.4 us                                                         | 20.3 us: 1.10x faster                                                           |
| pyflate                  | 422 ms                                                          | 384 ms: 1.10x faster                                                            |
| asyncio_tcp              | 744 ms                                                          | 678 ms: 1.10x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 110 ms: 1.09x faster                                                            |
| dask                     | 341 ms                                                          | 315 ms: 1.08x faster                                                            |
| sympy_sum                | 122 ms                                                          | 114 ms: 1.07x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.52 us: 1.06x faster                                                           |
| deepcopy                 | 310 us                                                          | 292 us: 1.06x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.06 ms: 1.06x faster                                                           |
| regex_dna                | 131 ms                                                          | 124 ms: 1.05x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.87 sec: 1.04x faster                                                          |
| spectral_norm            | 80.2 ms                                                         | 77.0 ms: 1.04x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 667 us: 1.04x faster                                                            |
| sympy_str                | 229 ms                                                          | 221 ms: 1.04x faster                                                            |
| sympy_expand             | 391 ms                                                          | 380 ms: 1.03x faster                                                            |
| regex_compile            | 117 ms                                                          | 114 ms: 1.03x faster                                                            |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.17 ms: 1.02x faster                                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 69.4 ms: 1.02x faster                                                           |
| 2to3                     | 265 ms                                                          | 263 ms: 1.01x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 16.7 ms: 1.01x slower                                                           |
| sqlglot_normalize        | 230 ms                                                          | 232 ms: 1.01x slower                                                            |
| pickle_list              | 3.22 us                                                         | 3.26 us: 1.01x slower                                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 45.4 ms: 1.01x slower                                                           |
| python_startup           | 22.9 ms                                                         | 23.3 ms: 1.02x slower                                                           |
| nqueens                  | 87.1 ms                                                         | 89.0 ms: 1.02x slower                                                           |
| mdp                      | 1.83 sec                                                        | 1.87 sec: 1.02x slower                                                          |
| fannkuch                 | 317 ms                                                          | 325 ms: 1.03x slower                                                            |
| regex_v8                 | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                           |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.03x slower                                                           |
| pickle                   | 7.83 us                                                         | 8.16 us: 1.04x slower                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| unpickle_list            | 2.98 us                                                         | 3.12 us: 1.05x slower                                                           |
| meteor_contest           | 80.0 ms                                                         | 85.6 ms: 1.07x slower                                                           |
| hexiom                   | 6.13 ms                                                         | 6.71 ms: 1.09x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.41 ms: 1.10x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 89.6 ms: 1.10x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.52 sec: 1.11x slower                                                          |
| pprint_safe_repr         | 658 ms                                                          | 743 ms: 1.13x slower                                                            |
| bench_mp_pool            | 66.4 ms                                                         | 75.1 ms: 1.13x slower                                                           |
| logging_simple           | 7.29 us                                                         | 8.29 us: 1.14x slower                                                           |
| logging_format           | 7.91 us                                                         | 9.01 us: 1.14x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.92 ms: 1.16x slower                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 71.6 ms: 1.16x slower                                                           |
| scimark_fft              | 216 ms                                                          | 250 ms: 1.16x slower                                                            |
| python_startup_no_site   | 18.1 ms                                                         | 21.0 ms: 1.16x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 47.1 ns: 1.18x slower                                                           |
| nbody                    | 79.1 ms                                                         | 93.7 ms: 1.18x slower                                                           |
| async_generators         | 241 ms                                                          | 299 ms: 1.24x slower                                                            |
| telco                    | 4.83 ms                                                         | 6.51 ms: 1.35x slower                                                           |
| coverage                 | 46.6 ms                                                         | 483 ms: 10.37x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.07x faster                                                                    |

Benchmark hidden because not significant (2): xml_etree_generate, chameleon
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.09% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown