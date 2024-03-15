
# Results vs. 3.10.4

- fork: python
- ref: ae460d450ab854ca66d5
- machine: windows-x86
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 252 ms: 1.05x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.96 ms: 1.08x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                          |
| tornado_http   | 118 ms                                                          | 97.8 ms: 1.20x faster                                                           |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 511 ms: 1.81x faster                                                            |
| async_tree_io           | 940 ms                                                          | 611 ms: 1.54x faster                                                            |
| async_tree_none         | 394 ms                                                          | 256 ms: 1.54x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 320 ms: 1.46x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.58x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 200 ms: 2.51x faster                                                            |
| float          | 69.6 ms                                                         | 54.5 ms: 1.28x faster                                                           |
| nbody          | 79.1 ms                                                         | 92.6 ms: 1.17x slower                                                           |
| Geometric mean | (ref)                                                           | 1.40x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 108 ms: 1.08x faster                                                            |
| regex_dna      | 131 ms                                                          | 122 ms: 1.07x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.00x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.91 ms: 1.42x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 224 us: 1.25x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.61 sec: 1.19x faster                                                          |
| unpickle_pure_python | 189 us                                                          | 161 us: 1.18x faster                                                            |
| json_loads           | 22.4 us                                                         | 20.0 us: 1.12x faster                                                           |
| xml_etree_process    | 48.1 ms                                                         | 43.3 ms: 1.11x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 113 ms: 1.06x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.0 ms: 1.04x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.26 us: 1.01x slower                                                           |
| pickle               | 7.83 us                                                         | 8.08 us: 1.03x slower                                                           |
| unpickle_list        | 2.98 us                                                         | 3.08 us: 1.03x slower                                                           |
| unpickle             | 9.82 us                                                         | 10.3 us: 1.05x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.0 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.07x faster                                                                    |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.4 ms: 1.02x faster                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.4 ms: 1.13x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.31 ms: 1.25x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 98.1 us: 4.04x faster                                                           |
| pidigits                 | 502 ms                                                          | 200 ms: 2.51x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 511 ms: 1.81x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.57 ms: 1.57x faster                                                           |
| async_tree_io            | 940 ms                                                          | 611 ms: 1.54x faster                                                            |
| async_tree_none          | 394 ms                                                          | 256 ms: 1.54x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 66.7 ns: 1.47x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 320 ms: 1.46x faster                                                            |
| json_dumps               | 9.82 ms                                                         | 6.91 ms: 1.42x faster                                                           |
| richards_super           | 49.9 ms                                                         | 35.6 ms: 1.40x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 960 us: 1.39x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 61.5 ms: 1.32x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.21 ms: 1.31x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 69.1 ms: 1.30x faster                                                           |
| richards                 | 40.3 ms                                                         | 31.2 ms: 1.29x faster                                                           |
| float                    | 69.6 ms                                                         | 54.5 ms: 1.28x faster                                                           |
| generators               | 31.6 ms                                                         | 24.7 ms: 1.28x faster                                                           |
| raytrace                 | 303 ms                                                          | 237 ms: 1.27x faster                                                            |
| pickle_pure_python       | 280 us                                                          | 224 us: 1.25x faster                                                            |
| mako                     | 9.10 ms                                                         | 7.31 ms: 1.25x faster                                                           |
| comprehensions           | 17.7 us                                                         | 14.3 us: 1.24x faster                                                           |
| chaos                    | 74.4 ms                                                         | 60.0 ms: 1.24x faster                                                           |
| scimark_sor              | 115 ms                                                          | 94.1 ms: 1.22x faster                                                           |
| go                       | 146 ms                                                          | 120 ms: 1.21x faster                                                            |
| pycparser                | 1.04 sec                                                        | 861 ms: 1.21x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 1.89 us: 1.21x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 617 ms: 1.21x faster                                                            |
| tornado_http             | 118 ms                                                          | 97.8 ms: 1.20x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.61 sec: 1.19x faster                                                          |
| unpickle_pure_python     | 189 us                                                          | 161 us: 1.18x faster                                                            |
| coroutines               | 17.9 ms                                                         | 15.2 ms: 1.18x faster                                                           |
| pyflate                  | 422 ms                                                          | 370 ms: 1.14x faster                                                            |
| spectral_norm            | 80.2 ms                                                         | 70.6 ms: 1.14x faster                                                           |
| json                     | 4.76 ms                                                         | 4.19 ms: 1.14x faster                                                           |
| dask                     | 341 ms                                                          | 301 ms: 1.13x faster                                                            |
| sympy_sum                | 122 ms                                                          | 109 ms: 1.13x faster                                                            |
| json_loads               | 22.4 us                                                         | 20.0 us: 1.12x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 26.4 us: 1.12x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 43.3 ms: 1.11x faster                                                           |
| deepcopy                 | 310 us                                                          | 280 us: 1.11x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.01 ms: 1.11x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.45 us: 1.10x faster                                                           |
| regex_compile            | 117 ms                                                          | 108 ms: 1.08x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                          |
| chameleon                | 6.42 ms                                                         | 5.96 ms: 1.08x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 646 us: 1.07x faster                                                            |
| sympy_str                | 229 ms                                                          | 214 ms: 1.07x faster                                                            |
| regex_dna                | 131 ms                                                          | 122 ms: 1.07x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.7 ms: 1.06x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 113 ms: 1.06x faster                                                            |
| 2to3                     | 265 ms                                                          | 252 ms: 1.05x faster                                                            |
| sympy_expand             | 391 ms                                                          | 374 ms: 1.04x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.0 ms: 1.04x faster                                                           |
| fannkuch                 | 317 ms                                                          | 306 ms: 1.04x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 224 ms: 1.03x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 43.5 ms: 1.03x faster                                                           |
| python_startup           | 22.9 ms                                                         | 22.4 ms: 1.02x faster                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.20 ms: 1.01x faster                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| mdp                      | 1.83 sec                                                        | 1.82 sec: 1.01x faster                                                          |
| pickle_list              | 3.22 us                                                         | 3.26 us: 1.01x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                           |
| pickle                   | 7.83 us                                                         | 8.08 us: 1.03x slower                                                           |
| unpickle_list            | 2.98 us                                                         | 3.08 us: 1.03x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 84.3 ms: 1.04x slower                                                           |
| unpickle                 | 9.82 us                                                         | 10.3 us: 1.05x slower                                                           |
| meteor_contest           | 80.0 ms                                                         | 84.2 ms: 1.05x slower                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.45 sec: 1.06x slower                                                          |
| hexiom                   | 6.13 ms                                                         | 6.50 ms: 1.06x slower                                                           |
| pprint_safe_repr         | 658 ms                                                          | 703 ms: 1.07x slower                                                            |
| gc_traversal             | 1.28 ms                                                         | 1.37 ms: 1.07x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 71.2 ms: 1.07x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.0 us: 1.10x slower                                                           |
| scimark_fft              | 216 ms                                                          | 242 ms: 1.12x slower                                                            |
| python_startup_no_site   | 18.1 ms                                                         | 20.4 ms: 1.13x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.95 us: 1.13x slower                                                           |
| logging_simple           | 7.29 us                                                         | 8.25 us: 1.13x slower                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 70.2 ms: 1.13x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                           |
| nbody                    | 79.1 ms                                                         | 92.6 ms: 1.17x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 46.9 ns: 1.17x slower                                                           |
| async_generators         | 241 ms                                                          | 290 ms: 1.20x slower                                                            |
| telco                    | 4.83 ms                                                         | 6.11 ms: 1.26x slower                                                           |
| coverage                 | 46.6 ms                                                         | 483 ms: 10.38x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.10x faster                                                                    |

Benchmark hidden because not significant (2): nqueens, xml_etree_generate
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-ae460d4-JIT/bm-20240215-pythonperf1_win32-x86-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown