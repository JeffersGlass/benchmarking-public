
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.12x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 247 ms: 1.07x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.94 ms: 1.08x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.4 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 516 ms: 1.79x faster                                                            |
| async_tree_none         | 394 ms                                                          | 252 ms: 1.56x faster                                                            |
| async_tree_io           | 940 ms                                                          | 611 ms: 1.54x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 318 ms: 1.47x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.58x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 199 ms: 2.53x faster                                                            |
| float          | 69.6 ms                                                         | 61.4 ms: 1.13x faster                                                           |
| nbody          | 79.1 ms                                                         | 87.6 ms: 1.11x slower                                                           |
| Geometric mean | (ref)                                                           | 1.37x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 107 ms: 1.09x faster                                                            |
| regex_dna      | 131 ms                                                          | 122 ms: 1.07x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.3 ms: 1.04x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.00x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.94 ms: 1.42x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 213 us: 1.31x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 152 us: 1.25x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 42.0 ms: 1.15x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                                          |
| json_loads           | 22.4 us                                                         | 20.5 us: 1.09x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 111 ms: 1.08x faster                                                            |
| xml_etree_generate   | 61.6 ms                                                         | 59.6 ms: 1.03x faster                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 69.7 ms: 1.02x faster                                                           |
| unpickle             | 9.82 us                                                         | 9.92 us: 1.01x slower                                                           |
| pickle_list          | 3.22 us                                                         | 3.35 us: 1.04x slower                                                           |
| unpickle_list        | 2.98 us                                                         | 3.13 us: 1.05x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.08x faster                                                                    |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.3 ms: 1.02x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.9 ms: 1.16x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 8.19 ms: 1.11x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 91.3 us: 4.34x faster                                                           |
| pidigits                 | 502 ms                                                          | 199 ms: 2.53x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 516 ms: 1.79x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 60.2 ns: 1.63x faster                                                           |
| async_tree_none          | 394 ms                                                          | 252 ms: 1.56x faster                                                            |
| async_tree_io            | 940 ms                                                          | 611 ms: 1.54x faster                                                            |
| richards_super           | 49.9 ms                                                         | 33.6 ms: 1.48x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 318 ms: 1.47x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 921 us: 1.44x faster                                                            |
| raytrace                 | 303 ms                                                          | 211 ms: 1.43x faster                                                            |
| scimark_lu               | 89.8 ms                                                         | 62.8 ms: 1.43x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.94 ms: 1.42x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 57.5 ms: 1.41x faster                                                           |
| deltablue                | 4.04 ms                                                         | 2.88 ms: 1.40x faster                                                           |
| scimark_sor              | 115 ms                                                          | 82.6 ms: 1.39x faster                                                           |
| go                       | 146 ms                                                          | 105 ms: 1.39x faster                                                            |
| chaos                    | 74.4 ms                                                         | 54.5 ms: 1.37x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.16 ms: 1.36x faster                                                           |
| generators               | 31.6 ms                                                         | 23.2 ms: 1.36x faster                                                           |
| richards                 | 40.3 ms                                                         | 30.4 ms: 1.32x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 213 us: 1.31x faster                                                            |
| comprehensions           | 17.7 us                                                         | 13.8 us: 1.28x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.3 ms: 1.25x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 152 us: 1.25x faster                                                            |
| pyflate                  | 422 ms                                                          | 340 ms: 1.24x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 1.87 us: 1.23x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 24.4 us: 1.21x faster                                                           |
| tornado_http             | 118 ms                                                          | 97.4 ms: 1.21x faster                                                           |
| pycparser                | 1.04 sec                                                        | 871 ms: 1.20x faster                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 52.3 ms: 1.18x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 42.0 ms: 1.15x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                                          |
| deepcopy_reduce          | 2.68 us                                                         | 2.36 us: 1.14x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 5.39 ms: 1.14x faster                                                           |
| json                     | 4.76 ms                                                         | 4.20 ms: 1.13x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 656 ms: 1.13x faster                                                            |
| float                    | 69.6 ms                                                         | 61.4 ms: 1.13x faster                                                           |
| deepcopy                 | 310 us                                                          | 274 us: 1.13x faster                                                            |
| sympy_sum                | 122 ms                                                          | 109 ms: 1.13x faster                                                            |
| nqueens                  | 87.1 ms                                                         | 78.2 ms: 1.11x faster                                                           |
| mako                     | 9.10 ms                                                         | 8.19 ms: 1.11x faster                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.24 sec: 1.10x faster                                                          |
| dask                     | 341 ms                                                          | 311 ms: 1.10x faster                                                            |
| json_loads               | 22.4 us                                                         | 20.5 us: 1.09x faster                                                           |
| regex_compile            | 117 ms                                                          | 107 ms: 1.09x faster                                                            |
| pprint_safe_repr         | 658 ms                                                          | 607 ms: 1.08x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 41.3 ms: 1.08x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.94 ms: 1.08x faster                                                           |
| sqlglot_normalize        | 230 ms                                                          | 213 ms: 1.08x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.4 ms: 1.08x faster                                                           |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                          |
| xml_etree_parse          | 120 ms                                                          | 111 ms: 1.08x faster                                                            |
| fannkuch                 | 317 ms                                                          | 295 ms: 1.08x faster                                                            |
| 2to3                     | 265 ms                                                          | 247 ms: 1.07x faster                                                            |
| regex_dna                | 131 ms                                                          | 122 ms: 1.07x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.05 ms: 1.07x faster                                                           |
| mdp                      | 1.83 sec                                                        | 1.71 sec: 1.06x faster                                                          |
| sympy_str                | 229 ms                                                          | 216 ms: 1.06x faster                                                            |
| create_gc_cycles         | 694 us                                                          | 664 us: 1.04x faster                                                            |
| xml_etree_generate       | 61.6 ms                                                         | 59.6 ms: 1.03x faster                                                           |
| sympy_expand             | 391 ms                                                          | 378 ms: 1.03x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 69.7 ms: 1.02x faster                                                           |
| meteor_contest           | 80.0 ms                                                         | 80.5 ms: 1.01x slower                                                           |
| unpickle                 | 9.82 us                                                         | 9.92 us: 1.01x slower                                                           |
| python_startup           | 22.9 ms                                                         | 23.3 ms: 1.02x slower                                                           |
| scimark_fft              | 216 ms                                                          | 224 ms: 1.03x slower                                                            |
| regex_v8                 | 15.8 ms                                                         | 16.3 ms: 1.04x slower                                                           |
| pickle_list              | 3.22 us                                                         | 3.35 us: 1.04x slower                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| unpickle_list            | 2.98 us                                                         | 3.13 us: 1.05x slower                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.41 ms: 1.05x slower                                                           |
| spectral_norm            | 80.2 ms                                                         | 87.2 ms: 1.09x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 88.7 ms: 1.09x slower                                                           |
| async_generators         | 241 ms                                                          | 264 ms: 1.09x slower                                                            |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                                           |
| logging_simple           | 7.29 us                                                         | 8.06 us: 1.11x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 73.4 ms: 1.11x slower                                                           |
| nbody                    | 79.1 ms                                                         | 87.6 ms: 1.11x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.42 ms: 1.11x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.84 us: 1.12x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.9 ms: 1.16x slower                                                           |
| telco                    | 4.83 ms                                                         | 6.18 ms: 1.28x slower                                                           |
| coverage                 | 46.6 ms                                                         | 481 ms: 10.33x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.12x faster                                                                    |

Benchmark hidden because not significant (2): pickle, unpack_sequence
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown