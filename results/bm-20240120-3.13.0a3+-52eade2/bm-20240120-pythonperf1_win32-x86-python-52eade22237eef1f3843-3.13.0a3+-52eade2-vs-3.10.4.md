
# Results vs. 3.10.4

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-x86
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.19x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 235 ms: 1.13x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.74 ms: 1.12x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.74 sec: 1.12x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.2 ms: 1.21x faster                                                           |
| Geometric mean | (ref)                                                           | 1.14x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 496 ms: 1.86x faster                                                            |
| async_tree_none         | 394 ms                                                          | 240 ms: 1.64x faster                                                            |
| async_tree_io           | 940 ms                                                          | 588 ms: 1.60x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 302 ms: 1.54x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.66x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.53x faster                                                            |
| float          | 69.6 ms                                                         | 54.8 ms: 1.27x faster                                                           |
| nbody          | 79.1 ms                                                         | 81.8 ms: 1.03x slower                                                           |
| Geometric mean | (ref)                                                           | 1.46x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 96.3 ms: 1.21x faster                                                           |
| regex_dna      | 131 ms                                                          | 118 ms: 1.11x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                           |
| Geometric mean | (ref)                                                           | 1.04x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.75 ms: 1.46x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 204 us: 1.37x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 140 us: 1.36x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.61 sec: 1.18x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 40.9 ms: 1.18x faster                                                           |
| json_loads           | 22.4 us                                                         | 20.1 us: 1.12x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 65.0 ms: 1.09x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 58.8 ms: 1.05x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.91 us: 1.03x faster                                                           |
| pickle               | 7.83 us                                                         | 7.72 us: 1.01x faster                                                           |
| unpickle             | 9.82 us                                                         | 9.91 us: 1.01x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 19.7 us: 1.08x slower                                                           |
| pickle_list          | 3.22 us                                                         | 3.64 us: 1.13x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 18.1 ms                                                         | 20.6 ms: 1.14x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 6.96 ms: 1.31x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 90.6 us: 4.37x faster                                                           |
| pidigits                 | 502 ms                                                          | 198 ms: 2.53x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 496 ms: 1.86x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.19 ms: 1.84x faster                                                           |
| logging_silent           | 97.9 ns                                                         | 55.9 ns: 1.75x faster                                                           |
| async_tree_none          | 394 ms                                                          | 240 ms: 1.64x faster                                                            |
| async_tree_io            | 940 ms                                                          | 588 ms: 1.60x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 852 us: 1.56x faster                                                            |
| chaos                    | 74.4 ms                                                         | 47.7 ms: 1.56x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 302 ms: 1.54x faster                                                            |
| comprehensions           | 17.7 us                                                         | 11.6 us: 1.53x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 53.4 ms: 1.52x faster                                                           |
| richards_super           | 49.9 ms                                                         | 32.8 ms: 1.52x faster                                                           |
| raytrace                 | 303 ms                                                          | 201 ms: 1.51x faster                                                            |
| go                       | 146 ms                                                          | 97.6 ms: 1.49x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 60.3 ms: 1.49x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.75 ms: 1.46x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.09 ms: 1.45x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 4.31 ms: 1.42x faster                                                           |
| generators               | 31.6 ms                                                         | 22.3 ms: 1.41x faster                                                           |
| richards                 | 40.3 ms                                                         | 29.2 ms: 1.38x faster                                                           |
| scimark_sor              | 115 ms                                                          | 83.7 ms: 1.38x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 204 us: 1.37x faster                                                            |
| pyflate                  | 422 ms                                                          | 310 ms: 1.36x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 140 us: 1.36x faster                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 46.3 ms: 1.34x faster                                                           |
| pycparser                | 1.04 sec                                                        | 793 ms: 1.31x faster                                                            |
| mako                     | 9.10 ms                                                         | 6.96 ms: 1.31x faster                                                           |
| float                    | 69.6 ms                                                         | 54.8 ms: 1.27x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.83 us: 1.25x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 23.8 us: 1.24x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.5 ms: 1.23x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 70.9 ms: 1.23x faster                                                           |
| sympy_sum                | 122 ms                                                          | 101 ms: 1.22x faster                                                            |
| regex_compile            | 117 ms                                                          | 96.3 ms: 1.21x faster                                                           |
| tornado_http             | 118 ms                                                          | 97.2 ms: 1.21x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 66.5 ms: 1.21x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.61 sec: 1.18x faster                                                          |
| fannkuch                 | 317 ms                                                          | 269 ms: 1.18x faster                                                            |
| xml_etree_process        | 48.1 ms                                                         | 40.9 ms: 1.18x faster                                                           |
| sympy_str                | 229 ms                                                          | 196 ms: 1.17x faster                                                            |
| json                     | 4.76 ms                                                         | 4.10 ms: 1.16x faster                                                           |
| deepcopy                 | 310 us                                                          | 267 us: 1.16x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 38.6 ms: 1.16x faster                                                           |
| sqlglot_normalize        | 230 ms                                                          | 199 ms: 1.16x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.58 sec: 1.15x faster                                                          |
| pprint_pformat           | 1.37 sec                                                        | 1.19 sec: 1.15x faster                                                          |
| sympy_expand             | 391 ms                                                          | 340 ms: 1.15x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 14.5 ms: 1.15x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.35 us: 1.14x faster                                                           |
| dask                     | 341 ms                                                          | 299 ms: 1.14x faster                                                            |
| pprint_safe_repr         | 658 ms                                                          | 582 ms: 1.13x faster                                                            |
| asyncio_tcp              | 744 ms                                                          | 659 ms: 1.13x faster                                                            |
| 2to3                     | 265 ms                                                          | 235 ms: 1.13x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.74 sec: 1.12x faster                                                          |
| chameleon                | 6.42 ms                                                         | 5.74 ms: 1.12x faster                                                           |
| json_loads               | 22.4 us                                                         | 20.1 us: 1.12x faster                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 2.91 ms: 1.12x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 108 ms: 1.11x faster                                                            |
| regex_dna                | 131 ms                                                          | 118 ms: 1.11x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 65.0 ms: 1.09x faster                                                           |
| bench_thread_pool        | 1.12 ms                                                         | 1.03 ms: 1.08x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 654 us: 1.06x faster                                                            |
| meteor_contest           | 80.0 ms                                                         | 75.7 ms: 1.06x faster                                                           |
| unpack_sequence          | 40.0 ns                                                         | 38.1 ns: 1.05x faster                                                           |
| scimark_fft              | 216 ms                                                          | 206 ms: 1.05x faster                                                            |
| xml_etree_generate       | 61.6 ms                                                         | 58.8 ms: 1.05x faster                                                           |
| unpickle_list            | 2.98 us                                                         | 2.91 us: 1.03x faster                                                           |
| pickle                   | 7.83 us                                                         | 7.72 us: 1.01x faster                                                           |
| unpickle                 | 9.82 us                                                         | 9.91 us: 1.01x slower                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.3 sec: 1.02x slower                                                          |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                           |
| nbody                    | 79.1 ms                                                         | 81.8 ms: 1.03x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.66 us: 1.05x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.36 us: 1.06x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 87.5 ms: 1.08x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 71.6 ms: 1.08x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.7 us: 1.08x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.39 ms: 1.09x slower                                                           |
| async_generators         | 241 ms                                                          | 266 ms: 1.10x slower                                                            |
| pickle_list              | 3.22 us                                                         | 3.64 us: 1.13x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.6 ms: 1.14x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                           |
| telco                    | 4.83 ms                                                         | 5.76 ms: 1.19x slower                                                           |
| coverage                 | 46.6 ms                                                         | 474 ms: 10.17x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.19x faster                                                                    |

Benchmark hidden because not significant (1): python_startup
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1_win32-x86-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown