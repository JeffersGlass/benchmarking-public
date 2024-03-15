
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-x86
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.19x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 233 ms: 1.14x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.65 ms: 1.14x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.73 sec: 1.13x faster                                                          |
| tornado_http   | 118 ms                                                          | 93.7 ms: 1.25x faster                                                           |
| Geometric mean | (ref)                                                           | 1.16x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 505 ms: 1.83x faster                                                            |
| async_tree_none         | 394 ms                                                          | 250 ms: 1.58x faster                                                            |
| async_tree_io           | 940 ms                                                          | 613 ms: 1.53x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 314 ms: 1.48x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.60x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 197 ms: 2.55x faster                                                            |
| float          | 69.6 ms                                                         | 52.4 ms: 1.33x faster                                                           |
| nbody          | 79.1 ms                                                         | 72.6 ms: 1.09x faster                                                           |
| Geometric mean | (ref)                                                           | 1.55x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 95.4 ms: 1.22x faster                                                           |
| regex_v8       | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                           |
| regex_dna      | 131 ms                                                          | 138 ms: 1.06x slower                                                            |
| regex_effbot   | 1.66 ms                                                         | 1.98 ms: 1.19x slower                                                           |
| Geometric mean | (ref)                                                           | 1.02x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.65 ms: 1.48x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 205 us: 1.36x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 139 us: 1.36x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 40.8 ms: 1.18x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                          |
| json_loads           | 22.4 us                                                         | 19.9 us: 1.13x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 111 ms: 1.08x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 66.6 ms: 1.06x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 58.5 ms: 1.05x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.24 us: 1.01x slower                                                           |
| pickle               | 7.83 us                                                         | 7.92 us: 1.01x slower                                                           |
| unpickle             | 9.82 us                                                         | 10.0 us: 1.02x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.2 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.1 ms: 1.01x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.4 ms: 1.13x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.01 ms: 1.30x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 93.8 us: 4.22x faster                                                           |
| pidigits                 | 502 ms                                                          | 197 ms: 2.55x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 505 ms: 1.83x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.23 ms: 1.81x faster                                                           |
| logging_silent           | 97.9 ns                                                         | 57.6 ns: 1.70x faster                                                           |
| chaos                    | 74.4 ms                                                         | 46.7 ms: 1.59x faster                                                           |
| comprehensions           | 17.7 us                                                         | 11.1 us: 1.59x faster                                                           |
| raytrace                 | 303 ms                                                          | 191 ms: 1.58x faster                                                            |
| async_tree_none          | 394 ms                                                          | 250 ms: 1.58x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 52.3 ms: 1.55x faster                                                           |
| richards_super           | 49.9 ms                                                         | 32.4 ms: 1.54x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 866 us: 1.54x faster                                                            |
| async_tree_io            | 940 ms                                                          | 613 ms: 1.53x faster                                                            |
| go                       | 146 ms                                                          | 95.3 ms: 1.53x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 59.8 ms: 1.50x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 314 ms: 1.48x faster                                                            |
| json_dumps               | 9.82 ms                                                         | 6.65 ms: 1.48x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.09 ms: 1.45x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 4.24 ms: 1.45x faster                                                           |
| scimark_sor              | 115 ms                                                          | 80.8 ms: 1.42x faster                                                           |
| richards                 | 40.3 ms                                                         | 28.8 ms: 1.40x faster                                                           |
| pyflate                  | 422 ms                                                          | 307 ms: 1.38x faster                                                            |
| generators               | 31.6 ms                                                         | 23.1 ms: 1.36x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 205 us: 1.36x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 139 us: 1.36x faster                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 46.2 ms: 1.34x faster                                                           |
| float                    | 69.6 ms                                                         | 52.4 ms: 1.33x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 22.4 us: 1.32x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.01 ms: 1.30x faster                                                           |
| unpack_sequence          | 40.0 ns                                                         | 31.1 ns: 1.29x faster                                                           |
| pycparser                | 1.04 sec                                                        | 812 ms: 1.28x faster                                                            |
| tornado_http             | 118 ms                                                          | 93.7 ms: 1.25x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.83 us: 1.25x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 64.3 ms: 1.25x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.5 ms: 1.23x faster                                                           |
| regex_compile            | 117 ms                                                          | 95.4 ms: 1.22x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 71.4 ms: 1.22x faster                                                           |
| sympy_sum                | 122 ms                                                          | 101 ms: 1.21x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 14.1 ms: 1.18x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 40.8 ms: 1.18x faster                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.16 sec: 1.18x faster                                                          |
| tomli_loads              | 1.91 sec                                                        | 1.62 sec: 1.18x faster                                                          |
| json                     | 4.76 ms                                                         | 4.09 ms: 1.17x faster                                                           |
| pprint_safe_repr         | 658 ms                                                          | 570 ms: 1.16x faster                                                            |
| sympy_str                | 229 ms                                                          | 198 ms: 1.15x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 38.9 ms: 1.15x faster                                                           |
| deepcopy                 | 310 us                                                          | 270 us: 1.15x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 202 ms: 1.14x faster                                                            |
| 2to3                     | 265 ms                                                          | 233 ms: 1.14x faster                                                            |
| chameleon                | 6.42 ms                                                         | 5.65 ms: 1.14x faster                                                           |
| sympy_expand             | 391 ms                                                          | 344 ms: 1.14x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.61 sec: 1.14x faster                                                          |
| dask                     | 341 ms                                                          | 302 ms: 1.13x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.73 sec: 1.13x faster                                                          |
| deepcopy_reduce          | 2.68 us                                                         | 2.38 us: 1.13x faster                                                           |
| json_loads               | 22.4 us                                                         | 19.9 us: 1.13x faster                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 2.88 ms: 1.12x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 663 ms: 1.12x faster                                                            |
| nbody                    | 79.1 ms                                                         | 72.6 ms: 1.09x faster                                                           |
| fannkuch                 | 317 ms                                                          | 292 ms: 1.09x faster                                                            |
| scimark_fft              | 216 ms                                                          | 199 ms: 1.08x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 111 ms: 1.08x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.04 ms: 1.08x faster                                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 66.6 ms: 1.06x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 58.5 ms: 1.05x faster                                                           |
| meteor_contest           | 80.0 ms                                                         | 75.9 ms: 1.05x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 664 us: 1.05x faster                                                            |
| python_startup           | 22.9 ms                                                         | 23.1 ms: 1.01x slower                                                           |
| pickle_list              | 3.22 us                                                         | 3.24 us: 1.01x slower                                                           |
| pickle                   | 7.83 us                                                         | 7.92 us: 1.01x slower                                                           |
| unpickle                 | 9.82 us                                                         | 10.0 us: 1.02x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.2 ms: 1.03x slower                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                          |
| logging_format           | 7.91 us                                                         | 8.34 us: 1.06x slower                                                           |
| regex_dna                | 131 ms                                                          | 138 ms: 1.06x slower                                                            |
| logging_simple           | 7.29 us                                                         | 7.85 us: 1.08x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 71.9 ms: 1.08x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.41 ms: 1.10x slower                                                           |
| async_generators         | 241 ms                                                          | 265 ms: 1.10x slower                                                            |
| pathlib                  | 81.2 ms                                                         | 89.5 ms: 1.10x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.2 us: 1.10x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.4 ms: 1.13x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.98 ms: 1.19x slower                                                           |
| telco                    | 4.83 ms                                                         | 5.99 ms: 1.24x slower                                                           |
| coverage                 | 46.6 ms                                                         | 473 ms: 10.17x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.19x faster                                                                    |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1_win32-x86-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown